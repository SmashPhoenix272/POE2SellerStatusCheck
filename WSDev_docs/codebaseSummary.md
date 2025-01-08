# Codebase Summary

## Key Components
### Userscript
- Main script for POE trade site monitoring
- Alert button implementation
- Status checking logic (including Online, Offline, and AFK)
- Notification system (with repeated alerts)
- Configuration panel (with volume control and warning)

## Data Flow
1. Script loads on POE trade site
2. Monitors DOM for trade listings
3. Adds alert buttons to each listing
4. Periodically checks seller status
5. Triggers notifications on status change (from Offline/AFK to Online)
6. Repeats notification every 5 minutes if the seller is still online

## External Dependencies
- Userscript manager (Tampermonkey/Violentmonkey)

## Recent Changes
- Initial project setup and documentation
- Implemented volume control enhancement with warning
- Implemented repeated alert functionality
