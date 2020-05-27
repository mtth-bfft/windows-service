# Minimal Windows Service

Just a template of Windows service, with logging and interactive debugging boilerplate.

## Usage

Actual work goes into DoWork(argc, argv).

Service can be installed using `.\minimal_service.exe /install` (or `sc create MySvc binPath= C:\...\minimal_service.exe`)

Then the service can be run in the background using `sc start MySvc` (it will log to the `szLogPath` file), or interactively using `.\minimal_service.exe`

