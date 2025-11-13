# PyEnvManager - Feature List

**Current Version:** v0.5.1  
**Last Updated:** November 14, 2025

This document lists the features available in PyEnvManager, organized by category and tier.

---

## 🎯 Core Features (Free Tier)

### Environment Discovery & Management
- ✅ **Multi-Type Environment Detection**
  - Conda environments
  - Mamba environments
  - Micromamba environments (bundled)
  - Python venv (virtualenv)
  - Poetry environments
  - UV environments
  - Automatic type classification based on project structure

- ✅ **Environment Scanning**
  - CLI-based scanning (conda/mamba/micromamba)
  - Directory scanning fallback
  - Home directory venv detection (up to 3 levels deep)
  - Deduplication across multiple tools
  - Case-insensitive path handling on Windows

- ✅ **Dashboard Overview**
  - Total environment count
  - Total disk usage across all environments
  - Cleanup potential calculation
  - Environment type breakdown
  - Real-time statistics

- ✅ **Environment Information**
  - Python version detection
  - Environment path and name
  - Environment type classification
  - Last used timestamp
  - Disk space usage per environment
  - Base environment protection indicators

- ✅ **Search & Filter**
  - Search environments by name
  - Filter by environment type
  - Sort by name, size, or Python version
  - Real-time search results

### User Experience Features
- ✅ **Interactive Tutorial System** (v0.5.1)
  - Step-by-step walkthrough for new users
  - Separate tutorials for free and Pro features
  - Visual indicators and tooltips
  - Completion tracking

- ✅ **YouTube Tutorial Integration** (v0.5.1)
  - Links to official YouTube channel (https://www.youtube.com/@pyenvmanager)
  - Minimalist design with red YouTube icons
  - Integrated into tutorial modal at strategic steps
  - Opens videos in new browser tab

- ✅ **Feedback System** (v0.5.1)
  - In-app feedback button in top navigation
  - Direct link to GitHub Issues page
  - Guided templates for bug reports
  - Feature request guidelines
  - Best practices for effective feedback

- ✅ **Version Display** (v0.5.1)
  - App version number visible in top bar
  - Subtle monospace styling
  - Easy version verification for support

### Environment Operations (Free)
- ✅ **Jupyter Notebook Launching**
  - One-click Jupyter launch in correct environment
  - Automatic browser opening
  - Token extraction and URL building
  - Support for all environment types
  - Graceful error handling

- ✅ **Basic Environment Creation**
  - Create new environments with specific Python versions
  - Name validation
  - Python version selection
  - Support for conda/mamba/micromamba/venv
  - Creation progress tracking

- ✅ **Size Calculation & Caching**
  - Background size calculation with caching
  - Manual rescan capability (60-second timeout)
  - Quick scan mode (10-second timeout)
  - Size cache persistence
  - Human-readable size formatting (B, KB, MB, GB, TB)
  - Timeout handling for large environments

### Data Persistence
- ✅ **Metadata Management**
  - Automatic metadata saving after scans
  - Environment metadata persistence
  - Scan ID and host information tracking
  - Summary statistics storage
  - Protected environment flagging

- ✅ **Size Cache System**
  - Persistent size cache across sessions
  - Background cache updates
  - Force refresh capability
  - Cache invalidation on demand

---

## 💎 Pro Features ($45/year Early Bird)

### Advanced Environment Management
- ✅ **Secure Environment Deletion** (v0.3.0)
  - Safe deletion with confirmation dialogs
  - Disk space preview before deletion
  - Protection for base environments
  - Recursive directory removal
  - Error handling and rollback

- ✅ **Environment Creation with Packages** (v0.3.0)
  - Create environments with initial package sets
  - Multiple package installation
  - Template-based creation
  - Progress tracking during creation

- ✅ **Pre-configured Templates** (v0.3.0)
  - Machine Learning template (NumPy, Pandas, Scikit-learn, etc.)
  - Data Science template (Jupyter, Matplotlib, Seaborn, etc.)
  - Web Development template (Flask, Django, FastAPI, etc.)
  - Scientific Computing template (SciPy, SymPy, etc.)
  - TensorFlow/PyTorch specialized templates
  - Custom package installation

- ✅ **Package Installation in Existing Environments** (v0.3.0)
  - Add packages to any existing environment
  - Support for conda and pip packages
  - Version specification
  - Progress tracking

### Security & Vulnerability Management

#### Package Scanning (v0.3.0)
- ✅ **Comprehensive Package Detection**
  - Conda package scanning
  - Pip package scanning
  - Package version tracking
  - Dependency list generation
  - Package count statistics

- ✅ **Vulnerability Scanning with OSV Integration**
  - Real-time CVE detection using OSV.dev API
  - Package-level vulnerability analysis
  - Version-specific vulnerability matching
  - Comprehensive vulnerability database access

#### CVE Severity Classification (v0.5.0)
- ✅ **Accurate Severity Detection** (Critical Fix v0.5.0)
  - CRITICAL severity identification
  - HIGH severity identification
  - MEDIUM severity identification
  - LOW severity identification
  - Proper severity grouping in reports
  - Fixed misclassification bug (all CVEs showing as LOW)

#### Automated Full System Scanning (v0.5.0)
- ✅ **Comprehensive Automated Scans**
  - Multi-phase scanning process:
    - Phase 1: Environment discovery
    - Phase 2: Package scanning with caching
    - Phase 3: Vulnerability detection with caching
    - Phase 4: SBOM generation for all formats
    - Phase 5: Report generation
  - Progress tracking with percentage completion
  - Real-time status updates
  - Automatic error recovery

- ✅ **Scan Duration Tracking** (v0.5.0)
  - Live elapsed time display (updates every 100ms)
  - Human-readable duration format (e.g., "2m 34s")
  - Duration notice with time estimates:
    - Small setups (5-10 envs): 10-30 seconds
    - Large setups (20+ envs): 1-3 minutes
  - First scan vs. cached scan timing information
  - Final duration display on completion

- ✅ **Scan Statistics Export** (v0.5.0)
  - `scan-statistics.json` file generation
  - Self-contained scan directories
  - Complete environment metadata
  - Package count per environment
  - Vulnerability count per environment
  - Severity breakdown (Critical, High, Medium, Low)
  - Analytics-ready JSON structure
  - Perfect for PostHog integration
  - Portable compliance packages

- ✅ **HTML Report Generation** (v0.5.0)
  - Comprehensive vulnerability reports with professional styling
  - Executive summary dashboard with key metrics:
    - Total environments and scanned count
    - Total packages discovered
    - Vulnerabilities by severity (Critical/High/Medium/Low)
    - SBOM files generated
  - Environment details table with:
    - Package counts (Fixed v0.5.0)
    - Vulnerability counts (Fixed v0.5.0)
    - Severity breakdowns (Fixed v0.5.0)
    - Active/Inactive status indicators
  - Scan phase completion tracking:
    - Phase 1: Environment Discovery
    - Phase 2: Package Scanning
    - Phase 3: Vulnerability Scanning
    - Phase 4: SBOM Export
    - Phase 5: Report Generation
  - SBOM export results summary table
  - Recommendations section with priority-based alerts
  - Scan metadata (timestamp, duration, scan ID)
  - Professional formatting with color-coded severity indicators
  - Zero-vulnerability environment tracking
  - Shareable standalone HTML file (includes embedded logo)

- ✅ **Scan History Management** (v0.5.1)
  - Scan registry with metadata
  - Quick scan listing
  - Scan deletion capability
  - Total size calculation
  - Format detection
  - Environment count tracking
  - Vulnerability statistics

#### SBOM Export (v0.3.0)
- ✅ **CycloneDX Format Support**
  - JSON format export
  - XML format export
  - Industry-standard compliance
  - Complete component metadata
  - Dependency tracking

- ✅ **SPDX Format Support**
  - JSON format export
  - XML format export
  - Software Package Data Exchange standard
  - License information inclusion
  - Package relationship mapping

- ✅ **SBOM Metadata**
  - Timestamp and version tracking
  - Host information
  - Environment details
  - Component lists
  - Dependency relationships
  - License detection

### Deep Scanning & Discovery

#### Standard Deep Scan (v0.3.0)
- ✅ **Deep Scan Cache System**
  - Persistent deep scan results
  - Cache loading on startup
  - Integration with regular scans
  - Cache clearing capability
  - Timestamp tracking

#### Advanced Deep Scan (v0.4.0)
- ✅ **Rust-Based Scanner Integration**
  - High-performance Rust-based file scanning
  - Cross-platform binary bundling
  - Automatic platform detection (Windows/macOS)
  - ARM64 and x64 support
  - Development and production binary paths
  - Fallback to system tools if bundled version unavailable

- ✅ **Comprehensive Filesystem Scanning**
  - Multi-drive scanning on Windows (local drives only)
  - Volume scanning on macOS (/Volumes)
  - Smart mount point detection
  - Network drive exclusion
  - Temporary mount filtering
  - Accessibility pre-checks

- ✅ **Intelligent pyvenv.cfg Detection**
  - Recursive file search across entire system
  - Hidden directory support (.venv, .virtualenv)
  - .gitignore-aware scanning
  - System directory exclusion (Windows, Program Files, etc.)
  - Timeout handling for slow drives (15-30 second limits)

- ✅ **Virtual Environment Type Detection**
  - UV environment detection via pyvenv.cfg metadata
  - UV project file detection (uv.lock, pyproject.toml)
  - Poetry environment detection via path patterns
  - Standard venv classification
  - Creator tool identification

- ✅ **pyvenv.cfg Metadata Parsing**
  - Python version extraction from multiple fields
  - UV version detection
  - Creator command parsing
  - Home path analysis
  - Installation metadata preservation

- ✅ **Integrated Deep Scan** (v0.4.0)
  - Combines CLI scanning with advanced deep scan
  - Intelligent deduplication
  - Single-click comprehensive discovery
  - Progress tracking for deep operations
  - Active scan state management

### UI/UX Enhancements

#### Design Improvements (v0.5.0 - v0.5.1)
- ✅ **Enhanced Pricing Card Visibility** (v0.5.1)
  - Monthly plan: Bright blue border (border-2 border-blue-400)
  - Yearly plan: Bright green border for early bird special
  - Improved shadow effects (shadow-lg hover:shadow-blue-400/30)
  - Better visual hierarchy for purchasing decisions

- ✅ **Windows 11 Rendering Fix** (v0.5.1 - Critical)
  - Fixed button color issues in Windows Light mode
  - Removed CSS media query override (prefers-color-scheme: light)
  - Added `forced-color-adjust: none` for OS-level prevention
  - Added `-webkit-text-fill-color: currentColor` for proper text rendering
  - All button colors (blue, green, purple, orange) now work in both themes
  - Thanks to [@vmiengineering](https://github.com/Pyenvmanager/pyenvmanager-releases/issues/1)

- ✅ **Improved Pro Feature Discoverability** (v0.5.1)
  - SBOM export button clickable for free users
  - Upgrade preview modal for free users
  - Better user guidance throughout interface
  - Enhanced tooltips and messaging

---

## 🔒 Security & Privacy

### Privacy-First Design
- ✅ **Local Processing**
  - All data stays on user's machine
  - No cloud uploads required
  - Local vulnerability database caching
  - Offline operation support (after initial CVE database download)

- ✅ **Secure External API Usage**
  - OSV.dev API for vulnerability data
  - HTTPS-only connections
  - No telemetry or tracking (privacy-first)
  - User consent for external requests

### Security Features
- ✅ **Base Environment Protection**
  - Automatic detection of base environments
  - Deletion prevention for system environments
  - Protection indicators in UI
  - Safe operation defaults

- ✅ **Path Validation**
  - Scan path security checks
  - Directory traversal prevention
  - Whitelist-based path validation
  - Secure file operations

---

## 🛠️ Technical Features

### Cross-Platform Support
- ✅ **Windows Support**
  - Windows 10/11 (x64)
  - PowerShell integration
  - Drive detection and scanning
  - Path normalization (case-insensitive)
  - Windows-specific binary bundling

- ✅ **macOS Support**
  - macOS (Intel x64)
  - macOS (Apple Silicon arm64)
  - Universal binary support
  - App notarization and stapling
  - Volume scanning
  - Gatekeeper compliance

### Bundled Tools
- ✅ **Micromamba Integration**
  - Bundled micromamba binary
  - Platform-specific binaries (Windows/macOS)
  - Automatic fallback to system micromamba
  - Development and production support

- ✅ **Rust-Based Scanner**
  - High-performance Rust-based file scanning
  - Bundled scanner binary for efficient deep scans
  - Cross-platform support
  - ASAR unpacking for executables

### Licensing System
- ✅ **Dodo Payments Integration**
  - Secure license activation
  - License deactivation
  - Plan verification (Free/Pro/Pro+/Enterprise)
  - Feature gating based on plan
  - License info display
  - Early bird pricing support

- ✅ **Feature Gating**
  - Dynamic feature availability checks
  - `canUse()` API for feature checks
  - Plan-specific capability enforcement
  - Graceful degradation for free users
  - Upgrade prompts and modals

### Logging & Diagnostics
- ✅ **Comprehensive Logging**
  - Application logs with timestamps
  - License operation logs (separate file)
  - Error tracking
  - Performance logging
  - Log file rotation by date
  - Log directory: `~/.pyenvmanager/logs/`

- ✅ **Error Handling**
  - Uncaught exception handlers
  - Unhandled promise rejection tracking
  - Graceful error recovery
  - User-friendly error messages
  - Detailed error logging

### Configuration Management
- ✅ **Environment Configuration**
  - Development vs. production modes
  - Configurable API endpoints
  - Product ID management
  - App metadata (name, version)
  - Environment-specific settings

### Performance Optimizations
- ✅ **Background Processing**
  - Async size calculations
  - Non-blocking scans
  - Deferred cache updates
  - Progressive UI updates

- ✅ **Caching Strategy**
  - Size cache persistence
  - Deep scan cache
  - Package scan cache
  - Vulnerability scan cache
  - Smart cache invalidation

- ✅ **Timeout Management**
  - Quick scan mode (10s timeout)
  - Manual rescan mode (60s timeout)
  - Drive scan timeouts (15-30s)
  - Deep scan operation timeouts
  - Graceful timeout handling

---

## 📊 Analytics & Reporting

### Scan Statistics (v0.5.0)
- ✅ **Comprehensive Metrics**
  - Total environments scanned
  - Total packages detected
  - Total vulnerabilities found
  - Severity breakdown
  - Scan duration tracking
  - Host information
  - Timestamp metadata

### Report Formats
- ✅ **HTML Reports**
  - Professional styling
  - Summary statistics
  - Environment detail tables
  - CVE listings
  - Severity badges
  - Export capability

- ✅ **JSON Reports**
  - Machine-readable format
  - Complete scan data
  - Analytics-ready structure
  - Easy integration
  - Version tracking

---

## 🚀 Upcoming Features (Roadmap)

### Near-Term (v0.6.0 - v0.7.0)
- 🔜 **Cleanup Wizard**
  - Bulk environment deletion
  - Orphan environment detection
  - Duplicate package analysis
  - Cache cleanup tools

- 🔜 **Analytics Dashboard**
  - CVE trends over time
  - Duplicate package identification
  - Environment growth tracking
  - Usage statistics

- 🔜 **Package Update Checker**
  - Identify outdated packages
  - Bulk update capabilities
  - Version comparison
  - Update recommendations

### Future Enhancements
- 🔜 **Environment Cloning**
  - Duplicate environments with all packages
  - Cross-platform environment export
  - Environment templates from existing setups

- 🔜 **Dependency Tree Visualization**
  - Interactive dependency graphs
  - Package relationship mapping
  - Conflict detection

- 🔜 **Undo/Quarantine Delete**
  - Safety net for deletions
  - Quarantine period before permanent removal
  - Restore capability

- 🔜 **Local Restore Points**
  - Environment snapshots
  - Rollback functionality
  - State preservation

---

## 📈 Version History

### v0.5.1 (November 14, 2025) - Current Release
- ✅ User feedback system with GitHub Issues integration
- ✅ YouTube tutorial integration
- ✅ Windows 11 Light mode rendering fix (Critical)
- ✅ Enhanced pricing card visibility
- ✅ Version number display
- ✅ Improved Pro feature discoverability

### v0.5.0 (November 11, 2025)
- ✅ Automated full system scan improvements
- ✅ Scan statistics file generation
- ✅ Real-time scan duration tracking
- ✅ CVE severity classification fix (Critical)
- ✅ Scan data population in reports

### v0.4.0
- ✅ Advanced deep scan with Rust-based scanner
- ✅ Integrated deep scan combining CLI with advanced scanning
- ✅ UV environment detection
- ✅ Cross-platform binary bundling for Rust-based scanner

### v0.3.0 (Initial Public Release)
- ✅ Core environment discovery
- ✅ Dashboard overview
- ✅ Jupyter launching
- ✅ Basic environment creation
- ✅ Pro features: Templates, deletion, package scanning, SBOM export

---

## 🤝 Community & Support

### Feedback Channels
- **In-App Feedback**: Click the Feedback button in top navigation
- **GitHub Issues**: https://github.com/Pyenvmanager/pyenvmanager-releases/issues
- **YouTube Channel**: https://www.youtube.com/@pyenvmanager

### Documentation
- **Tutorial System**: Built-in interactive tutorial
- **Video Tutorials**: Available on YouTube channel
- **Release Notes**: Comprehensive changelog for each version
- **Roadmap**: Transparent feature planning and prioritization

---

**Note**: This feature list is maintained and updated with each release. For the most current information, please check the release notes or visit our GitHub repository.

**Last Updated**: November 14, 2025  
**Version**: 0.5.1  
**Repository**: https://github.com/Pyenvmanager/pyenvmanager
