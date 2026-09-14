This is a program written in C by me, i wrote stereoxopya only for see how good i am in Windows Internals and C programming.<br>
In this project i used very common and simple libraries like: windows.h, mmsystem.h, math.h, string.h, stdio.h and time.h <br>
I highly recommend to compile the code with MSVC (because all the windows libs are installed by default) <br>

# ⚠️ How it works
This program is a Windows C application that uses the Graphics Device Interface (GDI) to manipulate the screen in real-time, creating visual glitches, screen melting effects, geometric shapes, and audio tones via the WinMM API. It features a continuous loop that polls a local web endpoint (http://127.0.0.1:80/rce) via curl to fetch remote commands. Depending on the received trigger, it executes specific visual shaders, displays localized custom message boxes, runs a timer countdown, or executes system commands locally using system().

# How use it
Prerequisites: You need a Windows environment (like a safe virtual machine or cybersecurity lab) with Microsoft Visual Studio installed.<br>
Compile: Open the x64 Native Tools Command Prompt for VS, and compile the code using: <br>
<br>
cl filename.c /O2 /link gdi32.lib user32.lib winmm.lib (or download the release)<br>
<br>
Then:<br>
Set up a local server on port 80 with apache2 and create a file named "rce" in the root of the server (like this: http://x.x.x.x/rce).<br>
Inside "rce" you can write the following stuff (only one at a time):<br>
<br>
"1" - Start a bunch of visual effects;<br>
"2" - Start vertical glitches<br>
"3" - Start horizontal glitches<br>
"4" - Tunnel effect<br>
"5" - Circolar effect<br>
"6" - Another Tunnel effect<br>
"7" - Some square<br>
"8" - Screen melter<br>
"9" - Atom bomb<br>
"10" - Some square stuff<br>
"11" - Predictable melter<br>
"Lulu" - Spawn my dog photos in the screen<br>
"Pixy" - Downscale the resolution<br>
"CHOOSE" - Spawn a question box then start some fx<br>
"IDLE" - Start idle effect<br>
"cmd: your_command_here" - Tiny windows shell here<br>
"CleanDWM" - Restart DWM.exe (Only if u run as Admin)<br>
"RandomMSGs" - Show random msg already written<br>
"Timer: custom_timer_here" - U can set a countdown to the fx show<br>
<br>
<br>
# ⚠️ Important Disclaimer

This software is:
- **non-destructive**
- created strictly for **education and research**
- intended for:
  - virtual machines
  - malware analysis labs
  - sandbox environments
  - Windows internals study

The software does **NOT**:
- delete files
- encrypt data
- damage boot sectors
- spread through networks
- bypass security intentionally
- attempt privilege escalation

Its purpose is to demonstrate concepts related to:
- graphical rendering
- API interaction
- behavioral analysis
- defensive cybersecurity understanding


# Why This Project Exists

Modern cybersecurity is not only about writing secure code.

It is also about understanding:
- how malicious software behaves
- how antivirus engines analyze processes
- how suspicious patterns are detected
- how graphical payloads historically worked

Studying these concepts helps:
- malware analysts
- reverse engineers
- software developers
- cybersecurity students
- defensive security researchers

build a deeper understanding of modern systems.

You cannot properly defend systems without understanding how they are made, right?.


# Recommended Environment

Is recommended to run inside:
- VirtualBox
- Vmware
- Hyper-V
- isolated environments

I tested on:
- Windows 10
- Windows 11

Using virtual machines is optional because:
- This program doesn't harm your pc or your file
- This program create only visual fx
- You can control behaviors

# How compile the code?
<code>cl "path/to/stereoxopya.c" /O2 /link gdi32.lib user32.lib</code><br>
*Obv you need Visual Studio with C compiler!*

# Author

Created by **ElektroWindows**

Focused on:
- Windows internals
- cybersecurity education
- reverse engineering
- graphical subsystem experimentation
- defensive security research

  PS: The original source contains comments written in Italian. An English-commented version may be released separately.
