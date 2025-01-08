# Technology Stack

## Frontend
- JavaScript (ES6+)
- Userscript
  - Tampermonkey/Violentmonkey compatibility
  - DOM manipulation
  - MutationObserver for dynamic content
  - GM_getValue and GM_setValue for storing configuration

## External Dependencies
- Browser extension: Tampermonkey/Violentmonkey
- Web Audio API for notifications
  - Note: Volume typically ranges from 0 to 1; values above 1 may cause distortion

## Architecture Decisions
- Userscript chosen over browser extension for:
  - Simpler development and maintenance
  - Easier distribution
  - Lightweight implementation
  - Cross-browser compatibility
