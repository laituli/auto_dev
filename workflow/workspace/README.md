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

# IMPROVEMENT ROADMAP

## Git-Based Workspace Workflow
**Current State**: Manual folder-based workspace approach with direct file copying
**Target State**: Git-based workflow using diffs instead of copying, automated review with git diff, selective integration with git cherry-pick
**Steps**: 
- [ ] Research git clone workflow patterns for temporary workspaces
- [ ] Design git diff-based review process
- [ ] Implement git cherry-pick for selective integration
- [ ] Test git workflow with existing modification process
- [ ] Update workspace instructions to reference git workflow
**Constraints**: Maintain instructive format, follow complexity constraints, backward compatibility, support remote/local merge
**Progress**: Not Started
