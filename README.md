# One-Hour-Shutdown-Timer
One-Hour Shutdown Timer Tool

!https://img.shields.io/badge/Platform-Windows-0078D6?logo=windows&logoColor=white
!https://img.shields.io/badge/License-MIT-green
!https://img.shields.io/badge/Language-Batch-blue

A simple timed shutdown tool based on Windows Batch script that automatically powers off your computer after a set duration. Ideal for parental controls, productivity management, and automated shutdown after downloads.

✨ Features

• ⏱️ Precise Timing - Supports accurate delayed shutdown from minutes to hours

• 🔄 Flexible Scheduling - Offers preset times (30min/1hr/2hr) and fully customizable durations

• 🔔 Smart Notifications - Displays customizable warning messages before shutdown

• 🚫 One-Click Cancel - Cancel scheduled shutdown anytime with a simple command

• 📱 Interactive Menu - Advanced version provides a user-friendly command-line interface

• 🛡️ System-Native - Built on Windows native shutdown command for maximum compatibility

🚀 Quick Start

Basic Version (1-Hour Timer)

1. Download the basic_timer.bat file
2. Right-click and select "Run as administrator"
3. The system will automatically shut down after 1 hour

Code Preview:
@echo off
echo Setting timed shutdown...
echo Notice: Computer will shut down in 1 hour
shutdown -s -t 3600 -c "Time is up. Please save your work."
echo Timed shutdown has been set!
pause


Advanced Version (Custom Timing)

1. Download the advanced_shutdown_tool.bat file
2. Double-click to run (recommended: Run as administrator)
3. Follow the menu prompts to select shutdown time

📁 Project Structure


shutdown-timer-tool/
├── README.md                 # Project documentation
├── basic_timer.bat           # Basic version (fixed 1-hour timer)
├── advanced_shutdown_tool.bat # Advanced version (interactive menu, customizable)
├── LICENSE                   # MIT License
└── examples/                 # Usage examples
    └── pomodoro_timer.bat    # Pomodoro technique extension example


🔧 Parameter Reference

Parameter Description Example

shutdown Windows system shutdown command -

-s Shut down the computer shutdown -s

-t Set delay time in seconds -t 3600 (1 hour)

-c Display a custom message -c "Please save your work!"

-a Abort scheduled shutdown shutdown -a

💡 Use Cases

👨👩👧👦 Parental Controls

Limit children's daily computer usage time and establish healthy routines.

⏰ Productivity Management

• Pomodoro Technique: Set 25-minute work + 5-minute break cycles

• Anti-Procrastination: Prevent marathon work sessions with scheduled breaks

📥 Download Management

Automatically shut down the computer after large file downloads complete.

🏢 Lab/Office Management

Automatically power off public computers after work/school hours.

🧪 Laboratory Environments

Automated system shutdown after long-running experimental tasks.

⚠️ Important Notes

1. Administrator Privileges: Some operations require running as administrator
2. Data Safety: Force shutdown doesn't wait for application responses. Always save your work first
3. Cancel Shutdown: Execute shutdown -a anytime before the countdown ends
4. Enterprise Environments: Group policies in domain-controlled networks may restrict shutdown commands
5. Background Tasks: Ensure no critical background tasks are running

🛡️ Safety Advisory

Warning: This tool performs system shutdown operations. Please note:

- Avoid running before saving important documents

- Test in a safe environment first

- Use cautiously before long-running tasks (rendering, compilation)

- Store scripts in areas with low accidental-click risk

🔄 Extended Usage

Custom Shutdown Messages

Edit the text after the -c parameter to customize user notifications:
shutdown -s -t 1800 -c "Meeting starting soon! Please save work and shut down."


Create Desktop Shortcut

1. Right-click BAT file → Send to → Desktop (create shortcut)
2. Right-click shortcut → Properties → Advanced → Check "Run as administrator"

Integrate with Task Scheduler

Use Windows Task Scheduler to automate daily shutdowns at fixed times.

❓ Frequently Asked Questions

Q: Can I skip the shutdown countdown?  
A: The 1-minute full-screen prompt cannot be skipped, but you can click "Cancel" during it.

Q: Does it support scheduled restart?  
A: Yes, replace -s with -r: shutdown -r -t 3600

Q: What's the minimum delay time?  
A: Minimum is 1 second, but very short times are not recommended.

Q: How to check for active shutdown schedules?  
A: Run: shutdown /a. If a schedule is active, it will show a prompt.

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

🤝 Contributing

Issues and Pull Requests are welcome! This includes but is not limited to:
• Feature suggestions

• Code optimizations

• Documentation improvements

• Bug reports

⭐ Support the Project

If you find this tool useful, please give it a Star!
