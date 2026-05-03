# Project Analysis Tool

## Overview

The `analyze_project.py` script is an automated project analysis tool that provides comprehensive insights into the Galaxium Travels booking system codebase. It's designed to help new developers quickly understand the project structure, architecture, and potential issues.

## Purpose

This tool automatically:
1. **Analyzes the entire codebase** - Examines backend, frontend, and deployment configurations
2. **Provides a clear summary** - Explains what the code accomplishes in plain language
3. **Documents architecture** - Highlights key patterns and critical implementation details
4. **Identifies problems** - Lists potential issues, outdated code, and areas for improvement
5. **Offers quick start guide** - Helps new developers get up to speed quickly

## Usage

### Basic Usage

Simply run the script from the project root directory:

```bash
python analyze_project.py
```

### What You'll Get

The script outputs five main sections:

#### 1. PROJECT OVERVIEW
- High-level description of the system
- Technology stack summary
- Project purpose and scope

#### 2. WHAT THE CODE ACCOMPLISHES
- Flight booking functionality
- MCP server integration
- User management features
- Data management approach
- Frontend capabilities
- Deployment options
- Testing infrastructure

#### 3. ARCHITECTURE & KEY POINTS
- Backend architecture breakdown
- Critical backend patterns (MCP lifecycle, session management, etc.)
- Frontend architecture overview
- Critical frontend patterns (env vars, error handling, etc.)
- Deployment scripts organization
- Testing patterns and requirements

#### 4. POTENTIAL PROBLEMS & ISSUES
- Security concerns
- Data persistence issues
- Architecture limitations
- Code quality issues
- Testing gaps
- Deployment issues
- Documentation gaps
- Dependency management problems
- Scalability concerns

#### 5. QUICK START FOR NEW DEVELOPERS
- Local development setup
- How to run tests
- Key files to understand first
- Common commands
- Environment variables
- Important notes and warnings

### Interactive Mode

After displaying the analysis, the script enters interactive mode with three options:

1. **Exit** - Complete the analysis and exit
2. **Get more details** - Guidance on investigating specific problems
3. **Start fixing problems** - Instructions for using Bob AI to fix issues

## When to Use This Tool

### For New Developers
- **First day onboarding** - Run this before diving into the code
- **Understanding architecture** - Get a bird's-eye view of the system
- **Identifying entry points** - Learn which files to read first

### For Code Reviews
- **Pre-review analysis** - Understand what to look for
- **Problem identification** - Get a checklist of known issues
- **Architecture validation** - Verify patterns are being followed

### For Maintenance
- **Technical debt assessment** - See all known problems in one place
- **Refactoring planning** - Identify areas that need improvement
- **Documentation updates** - Ensure docs match current state

### For AI-Assisted Development
- **Context for Bob AI** - Provide comprehensive project context
- **Problem prioritization** - Choose which issues to fix first
- **Verification** - Confirm changes align with architecture

## Integration with Bob AI

This tool is designed to work seamlessly with Bob AI:

### Step 1: Run Analysis
```bash
python analyze_project.py
```

### Step 2: Review Output
Read through the analysis to understand the codebase and identify problems.

### Step 3: Request Fixes
Ask Bob AI to fix specific issues, for example:
- "Fix the authentication system to use JWT tokens"
- "Add health check endpoints to the FastAPI server"
- "Implement proper error logging throughout the backend"
- "Add frontend tests using React Testing Library"

### Step 4: Verify Changes
Bob AI will:
1. Analyze the relevant code
2. Make necessary changes
3. Run tests to verify the changes work
4. Report back with results

## Key Features

### Comprehensive Coverage
- Analyzes backend (Python/FastAPI)
- Analyzes frontend (React/TypeScript)
- Reviews deployment scripts (Docker, AWS, IBM)
- Examines test infrastructure

### Critical Pattern Detection
- Identifies non-obvious patterns from AGENTS.md
- Highlights architecture decisions
- Documents gotchas and edge cases

### Problem Categorization
Problems are organized by type:
- Security
- Data Persistence
- Architecture
- Code Quality
- Testing
- Deployment
- Documentation
- Dependencies
- Scalability

### Windows Compatible
- Handles Unicode encoding issues
- Works with PowerShell and CMD
- No external dependencies required

## Requirements

- Python 3.7 or higher
- No additional packages required (uses only standard library)
- Must be run from project root directory

## Output Format

The script outputs plain text with:
- Clear section headers
- Bullet-point lists for easy scanning
- Bold text for emphasis (using markdown syntax)
- Consistent formatting throughout

## Customization

You can modify the script to:
- Add new analysis sections
- Change the problem categories
- Adjust the output format
- Add file-specific analysis
- Include metrics and statistics

## Troubleshooting

### Script Won't Run
- Ensure Python 3.7+ is installed: `python --version`
- Run from project root: `cd c:/Users/puvva/OneDrive/Desktop/galaxium-travels`
- Check file permissions

### Encoding Errors
- The script automatically handles Windows encoding
- If issues persist, try: `chcp 65001` before running

### Missing Information
- The script analyzes the current state of the repository
- Ensure all files are present and up-to-date
- Pull latest changes if working in a team

## Best Practices

1. **Run regularly** - Execute after major changes or before starting new work
2. **Share with team** - Include output in onboarding documentation
3. **Update as needed** - Modify script when architecture changes
4. **Use with Bob AI** - Leverage AI assistance to fix identified problems
5. **Document fixes** - Update AGENTS.md when resolving critical issues

## Example Workflow

```bash
# 1. Run analysis
python analyze_project.py

# 2. Review output and identify a problem
# Example: "No authentication/authorization system"

# 3. Ask Bob AI to fix it
# "Add JWT-based authentication to the FastAPI backend"

# 4. Bob AI will:
#    - Read relevant files
#    - Implement authentication
#    - Add tests
#    - Verify everything works

# 5. Run analysis again to confirm fix
python analyze_project.py
```

## Contributing

To improve this tool:
1. Add new analysis functions to the `ProjectAnalyzer` class
2. Update problem categories as issues are discovered
3. Enhance the interactive mode with more options
4. Add metrics and statistics gathering
5. Create visualizations of the architecture

## Support

For questions or issues:
- Review the output carefully - it contains detailed information
- Check AGENTS.md for critical patterns
- Ask Bob AI for clarification or assistance
- Consult the project README files

## License

This tool is part of the Galaxium Travels project and follows the same license.