# Changelog

All notable changes to this project will be documented in this file.

## [2026-05-6] - Deployment of Web Application

### Added
- `[Siege]` Created Virtual Machine for the WebApp
- `[Siege]` Nginx certification so that it would run on HTTPS Protocol
- `[Jp]` Added a domain name for the webapp
- `[Siege]` Service so that the webapp would run on startup
- `[Dexie]` Monitor Alerts so that the user can be notified if the chance of process fluctation
- `[Siege]` DevOps feature for continous deployment and integration
- `[Jp]` Created service on startup
- `[Jp]` Added more monitoring features such as active users

### Changed
- `[Siege]` Adjusted requirements.txt to fit the Linux Ecosystem
- `[Dexie]` Improved Nginx configuration
- `[Dexie]` Updated Nginx to the latest version after AI revealed a possible exploit

### Fixed
- `[Siege]` Fixed App entry to include a hardcoded PORT so that it can remain consistent

### Removed
- `[Jp]` Deleted Railway deprecated yml file
- `[Dexie]` Removed old Nginx certification

