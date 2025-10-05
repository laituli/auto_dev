# INSTRUCTION
1. **Create Git-Based Modification Workspace**
   - Create a git clone of the project: `git clone . modification_workspace`
   - Navigate to the workspace: `cd modification_workspace`

2. **Execute Modification Process**
   - Follow the instructions in `workflow/modification/README.md` to perform meta-development tasks
   - This includes understanding constraints, selecting tasks, and implementing improvements

3. **Execute Review Subworkflow**
   - Follow the instructions in `workflow/review/README.md` to present and apply changes
   - Use `git diff` to review modifications
   - Use `git cherry-pick` for selective integration

# MOTIVATION
A separate workspace folder enables clean separation between meta-development as a function (the process) and meta-development as an argument (the content being developed). This isolation prevents interference with the main workflow during development and allows for safe experimentation.

# IMPROVEMENT ROADMAP

## Git-Based Workspace Workflow
**Current State**: Manual folder-based workspace approach with direct file copying
**Target State**: Git-based workflow using diffs instead of copying, automated review with git diff, selective integration with git cherry-pick
**Steps**: 
- [x] Research git clone workflow patterns for temporary workspaces
- [x] Design git diff-based review process
- [x] Implement git cherry-pick for selective integration
- [x] Test git workflow with existing modification process
- [x] Update workspace instructions to reference git workflow
**Constraints**: Maintain instructive format, follow complexity constraints, backward compatibility, support remote/local merge
**Progress**: Completed
