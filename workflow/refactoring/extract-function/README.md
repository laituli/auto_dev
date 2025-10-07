# INSTRUCTION
Usage: Execute with parameters for function extraction

1. Receive input parameters:
   - `target_file`: File containing code to extract
   - `start_line`: Starting line of code block
   - `end_line`: Ending line of code block  
   - `function_name`: Name for new function
   - `parameters`: Optional parameter list for function

2. Analyze code block dependencies and variable usage
3. Create function signature based on analysis
4. Extract specified code block into new function
5. Replace original code with function call
6. Verify no behavioral changes occurred
7. Ensure function follows naming conventions and style guidelines

# MOTIVATION
Extracting functions improves code readability, reusability, and maintainability by breaking large methods into smaller, focused units with clear responsibilities.

# PARAMETER SPECIFICATION
- `target_file`: Path to source file (required)
- `start_line`: Integer line number (required)
- `end_line`: Integer line number (required)
- `function_name`: Valid identifier name (required)
- `parameters`: Comma-separated parameter names (optional)

# EXAMPLE USAGE
Execute with: `extract-function target_file=src/main.py start_line=10 end_line=25 function_name=calculate_total parameters=items,tax_rate`
