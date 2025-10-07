# INSTRUCTION
Usage: Execute with parameters for variable introduction

1. Receive input parameters:
   - `target_file`: File containing expression to replace
   - `line_number`: Line containing target expression
   - `expression`: Expression to extract into variable
   - `variable_name`: Name for new variable
   - `variable_type`: Optional type annotation

2. Analyze expression complexity and dependencies
3. Extract specified expression into variable
4. Replace original expression with variable reference
5. Verify no behavioral changes occurred
6. Ensure variable follows naming conventions and scope rules

# MOTIVATION
Introducing variables improves code readability by giving meaningful names to complex expressions, making code self-documenting and easier to understand.

# PARAMETER SPECIFICATION
- `target_file`: Path to source file (required)
- `line_number`: Integer line number (required)
- `expression`: Exact expression to extract (required)
- `variable_name`: Valid identifier name (required)
- `variable_type`: Optional type annotation (optional)

# EXAMPLE USAGE
Execute with: `introduce-variable target_file=src/main.py line_number=15 expression="user.get_age() * 365" variable_name=days_alive variable_type=int`
