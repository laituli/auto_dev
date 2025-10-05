# INSTRUCTION
1. **Present Changes**
   - Use `git diff` to show all modifications made in the modification workspace
   - Display changes in a clear, readable format

2. **Apply Changes**
   - Use `git cherry-pick` to selectively integrate changes from the modification workspace
   - Apply only the approved modifications to the main workflow

3. **Verify Integration**
   - Check that all constraints are maintained after integration
   - Ensure the workflow remains functional and instructive

# MOTIVATION
Provide a systematic way to review and integrate meta-development changes while maintaining project quality and constraints. The git-based approach enables selective integration and clear change tracking.

# IMPROVEMENT ROADMAP
**Current State**: Manual review process
**Target State**: Automated git diff review with selective cherry-pick integration
**Steps**: 
- [x] Create review subworkflow structure
- [ ] Implement git diff presentation
- [ ] Design cherry-pick selection process
- [ ] Test review workflow with existing modification process
- [ ] Update workspace instructions to reference git workflow
**Constraints**: Maintain instructive format, follow complexity constraints, backward compatibility
**Progress**: Initial structure created
