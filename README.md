$ python3 << 'PYEOF'
doc = """AIXFY - Setup Guide
===================
Aixfy is a rebranded development tool for building MIT App Inventor 2 Extensions.
It is based on the FAST-CLI engine with all premium features unlocked.

---

1.  SYSTEM REQUIREMENTS
    -------------------
    - Java 11 or later (JRE or JDK)
    - Windows / Linux / macOS
    - Internet connection (for first-time dependency downloads)

2.  INSTALLATION
    ------------
    
    Option A: Direct JAR Usage (Quick Start)
    
    1. Place the "Aixfy.jar" file anywhere on your system.
    2. Open a terminal/command prompt.
    3. Run:
           java -jar path/to/Aixfy.jar -v
       You should see:
           Aixfy v6.1.0 (Premium)
           AIXFY_HOME: ...
    
    Option B: Environment Setup (Recommended)
    
    1. Create a folder for Aixfy, e.g.:
           C:\\Aixfy    (Windows)
           ~/aixfy      (Linux/macOS)
    
    2. Set the AIXFY_HOME environment variable:
       Windows (Command Prompt):
           setx AIXFY_HOME "C:\\Aixfy"
       Windows (PowerShell):
           [Environment]::SetEnvironmentVariable("AIXFY_HOME", "C:\\Aixfy", "User")
       Linux/macOS (add to ~/.bashrc or ~/.zshrc):
           export AIXFY_HOME="$HOME/.aixfy"
    
    3. (Optional) Create an alias for convenience:
       Windows:
           doskey aixfy=java -jar C:\\Path\\To\\Aixfy.jar $*
       Linux/macOS:
           alias aixfy='java -jar ~/aixfy/Aixfy.jar'
       Or create a batch/shell script:
           # aixfy.bat (Windows)
           @echo off
           java -jar "C:\\Path\\To\\Aixfy.jar" %*
           
           # aixfy.sh (Linux/macOS)
           #!/bin/bash
           java -jar "$HOME/aixfy/Aixfy.jar" "$@"

3.  USAGE
    ------
    
    Command structure:
        java -jar Aixfy.jar [command] <arguments>
    
    Available commands:
        create    Create a new project
        sync      Synchronize project dependencies and resources
        build     Build the project
        clean     Clean build caches
        jetify    Migrate Android support libraries to AndroidX
        migrate   Migrate other projects to Aixfy
        upgrade   Update Aixfy to latest version
    
    Global arguments:
        -d       Enable verbose logging
        -dir     Manually specify project directory
        -v       Show version information
    
    Examples:
        java -jar Aixfy.jar create MyExtension
            Creates a new project named "MyExtension" in the current directory.
        
        java -jar Aixfy.jar build
            Builds the project in the current directory.
        
        java -jar Aixfy.jar -dir "C:\\MyProject" build
            Builds a project in a specific directory.
        
        java -jar Aixfy.jar -d build
            Builds with verbose logging.

4.  PROJECT STRUCTURE
    -----------------
    When you create a project with "aixfy create", the following structure
    is generated:
    
        MyExtension/
        |-- fast.yml          # Project configuration
        |-- src/              # Source files
        |-- libs/             # Library dependencies
        |-- assets/           # Resources
        +-- .aixfy/           # Aixfy internal cache and logs

5.  NOTES
    ------
    - All premium features are unlocked
    - No license key required
    - The internal engine still references "FAST" in some areas but
      the tool is fully functional under the Aixfy name
"""

import os
path = r'C:\Users\Admin\Downloads\AIXFY_SETUP_GUIDE.txt'
with open(path, 'w') as f:
    f.write(doc)
print(f'Documentation created: {path}')
PYEOF
<stdin>:30: SyntaxWarning: invalid escape sequence '\A'
Documentation created: C:\Users\Admin\Downloads\AIXFY_SETUP_GUIDE.txt
