# INSTRUCTION
1. Check if a folder has no README.md file
   - If missing, create a README.md following project practise.
2. For any .md file that is not a README:
   - Create a corresponding folder with the same name (without .md extension)
   - Move the .md file into that folder and rename it to README.md
3. If a subworkflow file references another workflow that is not in the same folder:
   - Move the referenced workflow file into the caller's folder
   - Update any file references to maintain proper structure

# MOTIVATION
1. Maintain consistent project structure across all workflows
2. Ensure every folder has clear documentation through README files
3. Keep related workflows together for better organization and maintainability
4. Follow the principle that each folder should be self-contained with its documentation
