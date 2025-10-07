# INSTRUCTION
Usage: Execute with argument specifying refactoring type

1. If argument is 'extract-function':
   - Execute `extract-function/README.md` with function extraction parameters
2. If argument is 'introduce-variable':
   - Execute `introduce-variable/README.md` with variable introduction parameters  
3. If argument is 'if-statement-null':
   - Execute `if-statement-null/README.md` with conditional scaffolding parameters
4. If argument is 'rename-identifier':
   - Execute `rename-identifier/README.md` with renaming parameters
5. Verify atomicity of changes
6. Ensure bi-sync with main workflow

# MOTIVATION
Parameterized refactoring workflows enable centralized user specification while maintaining atomic, instructive refactoring operations. This supports future integration with automated refactoring selection systems.

# REFACTORING PRINCIPLES
- **Parameterized**: All refactorings accept input arguments for specification
- **Atomic**: Each refactoring is complete and testable in isolation
- **Reversible**: Changes can be easily rolled back if needed
- **Centralized**: User specifications concentrated in single configuration file
