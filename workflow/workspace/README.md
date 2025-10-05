# INSTRUCTION
1. **Create Modification Workspace**
   - Create a dedicated folder named `modification_workspace` for temporary development work

2. **Execute Modification Process**
   - Follow the instructions in `workflow/modification/README.md` to perform meta-development tasks
   - This includes understanding constraints, selecting tasks, and implementing improvements

3. **Execute Review Subworkflow**
   - Follow the instructions in `review/README.md` to present and apply changes

# MOTIVATION
A separate workspace folder enables clean separation between meta-development as a function (the process) and meta-development as an argument (the content being developed). This isolation prevents interference with the main workflow during development and allows for safe experimentation.

# LONG-TERM TARGET
**Git-Based Workspace Technique**
- Target: Replace manual folder approach with git-based workflow
- Technique: Clone project temporarily into local subfolder, use commits/diffs for review, cherry-pick for integration
- Allow remoted or local merge (subfolder MR -> local pull + subfolder pull).