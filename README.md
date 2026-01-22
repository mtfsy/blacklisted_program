this is simple exe for windows to enable stopping background task that annoy user like forced upgrade or other telemetry program on windows

Usage

stopper.exe --interval-svc 0 --interval-exe 0 --delay 86400

--interval-svc is schedule for interval for svc program to be stopped. default is 180
--interval-exe is schedule for interval for exe program to be stopped. default is 180
--delay is schedule for wipping log on activity_log.txt. default is 86400

you can set this in task scheduler on system startup so it always run everytime you boot windows.

for exe or svc that need to be blocked refer to text_program_to_be_blocked.txt for exe you should add .exe to filename otherwise it will recognize as svc program