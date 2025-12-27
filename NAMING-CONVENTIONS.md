# Naming Conventions for Prompt Library

**Version:** 1.0  
**Last Updated:** December 27, 2025  
**Maintained by:** Deputy Chief of Staff, Montana VA Health Care System

## Overview

This document establishes consistent file naming conventions for the Prompt Library repository. These standards ensure files are discoverable, maintainable, and properly organized across all categories.

---

## Core Principles

1. **Clarity**: File names should clearly indicate content and purpose
2. **Consistency**: Use standardized patterns across all folders
3. **Discoverability**: Names should be searchable and self-documenting
4. **Compatibility**: Follow cross-platform naming standards
5. **Versioning**: Include version identifiers when tracking iterations

---

## General Rules

### Character Standards
- **Use hyphens (`-`)** to separate words in file names
- **Use underscores (`_`)** to separate logical components (category, date, version)
- **Capitalize** the first letter of each major component
- **No spaces** in file names
- **Avoid special characters**: `/ \ : * ? " < > |`

### File Extensions
- **Markdown files**: `.md` (primary format for prompts and documentation)
- **Text files**: `.txt` (for code snippets, templates, or plain text)
- **Configuration files**: As appropriate (`.json`, `.yaml`, etc.)

### Length Guidelines
- Keep file names **under 100 characters** when possible
- Use abbreviations for common VA terms (CPRS, EMG, NCS, TBI, SAIL)
- Balance descriptiveness with brevity

---

## Naming Patterns by File Type

### 1. Monthly Prompt Collections

**Pattern:** `[Category]_Prompts_[MonthYear].md`

**Components:**
- `[Category]`: Title case category name (Clinical, Administrative, Data_Analysis)
- `[MonthYear]`: Three-letter month + four-digit year (Dec2025, Jan2026)

**Examples:**
```
Clinical_Prompts_Dec2025.md
Administrative_Prompts_Jan2026.md
Data_Analysis_Prompts_Feb2026.md
```

**Purpose:** Monthly archives of prompts organized by work category

---

### 2. Project-Specific Standalone Files

**Pattern:** `[Project-Name]-[Descriptor]-v[Version].[ext]`

**Components:**
- `[Project-Name]`: Descriptive project identifier (hyphen-separated)
- `[Descriptor]`: Optional clarifying term (Deterministic, Dictation, Implementation)
- `v[Version]`: Version number (v1.0, v2.1, v3.0-FINAL)
- `[ext]`: File extension (.txt, .md)

**Examples:**
```
CPRS-Ambient-Deterministic-v2.1.txt
CPRS-Ambient-Dictation-MCP.txt
CPRS-Ambient-v3.0-FINAL.txt
CPRS-Implementation-Code.txt
```

**Purpose:** Specific project files that are version-tracked or component-specific

---

### 3. Tool/Process Documentation Files

**Pattern:** `[tool-name]-[function].md`

**Components:**
- `[tool-name]`: Name of the tool or platform (lowercase with hyphens)
- `[function]`: Purpose of the document (instructions, configuration, guide)

**Examples:**
```
perplexity-instructions.md
chatgpt-claude-instructions.md
perplexity-multi-role-document-analyzer.md
dragon-medical-transcription-simulator.md
```

**Purpose:** Documentation for tools, integrations, or processes

---

### 4. Subfolder Organization

**When to Create Subfolders:**
- Projects with **3+ related files**
- Clear component separation needed
- Version history tracking required

**Subfolder Naming Pattern:** `[Project_Name]/`

**Examples:**
```
Ambient_Scribe/
├── CPRS-Ambient-Deterministic-v2.1.txt
├── CPRS-Ambient-Deterministic-v2.txt
├── CPRS-Ambient-Dictation-MCP.txt
├── CPRS-Ambient-v3.0-FINAL.txt
└── CPRS-Implementation-Code.txt
```

---

## Category-Specific Conventions

### Clinical Folder

**Typical File Types:**
- Monthly prompt collections
- EMG/NCS documentation templates
- Clinical workflow tools
- Evidence-based medicine prompts
- Patient communication templates

**Naming Examples:**
```
Clinical_Prompts_Dec2025.md
EMG-Report-Template-Carpal-Tunnel.md
TBI-Assessment-Framework.md
Patient-Education-Ulnar-Neuropathy.md
Spasticity-Management-Template.md
```

---

### Administrative Folder

**Typical File Types:**
- Monthly prompt collections
- Leadership communication templates
- Quality improvement documentation
- Meeting management tools
- Policy compliance prompts

**Naming Examples:**
```
Administrative_Prompts_Dec2025.md
Staff-Communication-Template.md
SAIL-Metrics-Briefing-Guide.md
Executive-Meeting-Agenda-Template.md
Policy-Compliance-Checklist.md
perplexity-multi-role-document-analyzer.md
```

---

### Data Analysis Folder

**Typical File Types:**
- Monthly prompt collections
- SQL query templates
- Power BI/Excel analysis tools
- Statistical analysis frameworks
- Automation scripts documentation

**Naming Examples:**
```
Data_Analysis_Prompts_Dec2025.md
SQL-Wait-Time-Analysis-Query.md
Power-BI-Quality-Metrics-DAX.md
Statistical-Analysis-Patient-Outcomes.md
CDW-Query-Template-Utilization.md
```

---

## Version Control Conventions

### Version Number Format

**Pattern:** `v[Major].[Minor].[Patch]`

**Semantic Versioning:**
- **Major** (v2.0): Significant changes, breaking changes, complete rewrites
- **Minor** (v2.1): Feature additions, enhancements, non-breaking changes
- **Patch** (v2.1.1): Bug fixes, minor corrections, typo fixes

**Special Designators:**
- `-FINAL`: Approved final version
- `-DRAFT`: Work in progress
- `-TEST`: Testing version
- `-BACKUP`: Archive copy

**Examples:**
```
CPRS-Ambient-v1.0.txt           # Initial release
CPRS-Ambient-v2.0.txt           # Major revision
CPRS-Ambient-v2.1.txt           # Enhanced version
CPRS-Ambient-v3.0-FINAL.txt     # Approved final
CPRS-Ambient-v3.1-DRAFT.txt     # Development version
```

---

## Commit Message Conventions

### Format Structure

**Pattern:** `[Category]: [Action] - [Brief Description]`

**Action Verbs:**
- `Add`: New file or feature
- `Update`: Modify existing content
- `Fix`: Correct errors or issues
- `Refactor`: Reorganize without changing functionality
- `Remove`: Delete file or content
- `Merge`: Combine changes

**Examples:**
```
Clinical: Add - EMG report template for carpal tunnel syndrome
Administrative: Update - SAIL metrics briefing with Q4 2025 data
Data-Analysis: Fix - SQL syntax error in wait time query
Clinical: Refactor - Reorganize spasticity management prompts
Administrative: Remove - Deprecated policy compliance checklist
```

### Detailed Commit Message Format

```
[Category]: [Action] - [Brief Description]

Changes:
- [Specific change 1]
- [Specific change 2]
- [Specific change 3]

Context: [Why this change was made]
File: [path/to/file.md]
Date: [YYYY-MM-DD]
```

**Example:**
```
Clinical: Update - CPRS-Ambient-v3.0-FINAL.txt

Changes:
- Enhanced execution directives for deterministic output
- Added confirmation requirements for sensitive actions
- Improved error handling in edge cases
- Updated documentation with usage examples

Context: Implementing feedback from pilot testing phase to improve
reliability and user confidence in automated clinical documentation.

File: clinical/CPRS-Ambient-v3.0-FINAL.txt
Date: 2025-12-24
```

---

## Deprecated Patterns (Do Not Use)

❌ **Avoid These Patterns:**

```
file name with spaces.md          # Use hyphens instead
FileNameInCamelCase.md            # Use hyphens or underscores
file_name_all_underscores.md      # Mix hyphens and underscores appropriately
VERYLONGFILENAMETHATISHARDTOREAD.md  # Too long, no separation
temp.md                           # Not descriptive
test123.md                        # Not descriptive
New Document (1).md               # Auto-generated name
```

---

## Migration Guide

### Renaming Existing Files

**When renaming files:**
1. Update references in documentation
2. Note the change in commit message
3. Consider leaving a redirect or note if widely referenced
4. Use descriptive commit: `Refactor: Rename [old-name] to [new-name] for consistency`

**Example Migration:**
```
Old: cprs ambient v3.txt
New: CPRS-Ambient-v3.0-FINAL.txt

Commit: "Refactor: Rename cprs ambient v3.txt to follow naming conventions
- Applied standard hyphenation
- Added proper version format
- Included FINAL designator"
```

---

## Automated System Integration

### Perplexity Save Commands

When instructing Perplexity to save content, the system will:

1. **Parse your command** to identify category and project
2. **Check existing files** for naming patterns
3. **Apply conventions** automatically:
   - Monthly logs: Use `[Category]_Prompts_[MonthYear].md`
   - New projects: Use `[project-name]-[descriptor].md`
   - Updates: Match existing file naming pattern
4. **Generate commit message** following standard format

**Command Examples:**
```
"Save this to clinical"                    → Clinical_Prompts_Dec2025.md
"Save as new project: EMG Report Builder"  → EMG-Report-Builder.md
"Update CPRS Ambient version 3.1"          → CPRS-Ambient-v3.1.txt
```

---

## Maintenance Schedule

### Monthly Review
- Check for naming inconsistencies
- Archive old versions if needed
- Update monthly prompt files

### Quarterly Audit
- Reorganize large projects into subfolders
- Consolidate duplicate or similar files
- Update this document if new patterns emerge

### Annual Cleanup
- Remove deprecated files
- Archive historical versions
- Review and update conventions based on usage patterns

---

## Quick Reference Table

| File Type | Pattern | Example |
|-----------|---------|----------|
| Monthly Log | `[Category]_Prompts_[MonthYear].md` | `Clinical_Prompts_Dec2025.md` |
| Project File | `[Project-Name]-[Descriptor]-v[Version].[ext]` | `CPRS-Ambient-v3.0-FINAL.txt` |
| Tool Doc | `[tool-name]-[function].md` | `perplexity-instructions.md` |
| Template | `[Type]-[Purpose]-Template.md` | `EMG-Report-Template.md` |
| Subfolder | `[Project_Name]/` | `Ambient_Scribe/` |

---

## Examples by Scenario

### Scenario 1: Creating a New Clinical Template
**Task:** Create an EMG report template for radiculopathy  
**File Name:** `EMG-Report-Radiculopathy-Template.md`  
**Location:** `clinical/`  
**Commit:** `Clinical: Add - EMG report template for radiculopathy diagnosis`

### Scenario 2: Updating an Existing Project
**Task:** Update CPRS Ambient Scribe to version 3.2  
**File Name:** `CPRS-Ambient-v3.2.txt`  
**Location:** `clinical/Ambient_Scribe/`  
**Commit:** `Clinical: Update - CPRS-Ambient-v3.2 with enhanced error handling`

### Scenario 3: Adding a Monthly Entry
**Task:** Save new administrative prompt for staff communication  
**File Name:** `Administrative_Prompts_Dec2025.md` (append)  
**Location:** `administrative/`  
**Commit:** `Administrative: Update - Added staff communication template for policy changes`

### Scenario 4: Creating Documentation
**Task:** Document Power BI integration process  
**File Name:** `power-bi-integration-guide.md`  
**Location:** `data-analysis/`  
**Commit:** `Data-Analysis: Add - Power BI integration guide with DAX examples`

---

## Support and Questions

For questions about naming conventions or edge cases not covered:
1. Review existing files in the relevant category
2. Apply the core principles (clarity, consistency, discoverability)
3. Document your decision in the commit message
4. Update this guide if a new pattern emerges

---

## Revision History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | 2025-12-27 | Initial naming conventions established | Seth Chandler |

---

**Note:** This is a living document. As the repository grows and new patterns emerge, this guide should be updated to reflect best practices and lessons learned.
