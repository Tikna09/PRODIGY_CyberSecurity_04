# Introduction

Keyloggers are one of the most common tools used by attackers to collect sensitive information by capturing user keystrokes. This project demonstrates how a keystroke monitoring tool works at a technical level.
The purpose of **this project is strictly educational—** to help students understand malware behavior, detection techniques, and cybersecurity defenses.

**The project is executed in a controlled lab environment using:**

* Windows Machine (victim simulation)
* Kali Linux Machine (listener/server)
* Python keylogger script converted to EXE
* Netcat listener for receiving captured keystrokes

# Objective of the Project

**The primary objectives are:**

* To understand how Windows APIs capture keyboard input.
* To analyze how keystroke data is transferred to a remote server.
* To convert a Python script into a Windows executable.
* To create a controlled simulation for monitoring keystrokes.
* To demonstrate how attackers use such techniques—and how defenders can detect them.

# Technologies Used

| Component                | Purpose                       |
| ------------------------ | ----------------------------- |
| **Python 3.10**          | Writing keylogger script      |
| **ctypes (Windows API)** | Capturing keystrokes          |
| **socket module**        | Sending data to server        |
| **PyInstaller**          | Converting Python file to EXE |
| **Kali Linux (Netcat)**  | Receiving keystrokes          |
| **Windows 11**           | Running EXE for test          |

# System Architecture

**Workflow of the Project**
* The keylogger script runs on the Windows machine.
* It captures keystrokes using the Windows API (GetAsyncKeyState).
* Each keystroke is converted into readable format.
* The data is sent to a remote listener server via a TCP socket.
* The Kali Linux Netcat listener receives and displays the keystrokes in real time.













