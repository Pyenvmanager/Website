# What's New in PyEnvManager v0.5.6

**Release Date:** January 31, 2026

## 🐛 Bug Fixes

### Git-Based Project Grouping - Fixed
- **Fixed:** Environments now properly group by Git repository without requiring a refresh
- **Impact:** Immediate project-based organization on app launch and after scans
- **Details:** Git context is now properly saved to cache files and loaded on startup, enabling consistent grouping across sessions

### Cache Persistence Enhancement
- **Improved:** Git repository metadata now persisted in environment caches
- **Impact:** Faster startup times with accurate project grouping from cached data
- **Details:** 
  - Deep scan cache now includes `gitContext` property
  - Integrated scan properly extracts and saves git metadata
  - Cache loading preserves git repository information

---

## Feedback

We'd love to hear your thoughts on this release! Report issues or suggest features through our GitHub repository.

---

**Version:** 0.5.6  
**Platform:** Windows, macOS, Linux  
**License:** See LICENSE.txt
