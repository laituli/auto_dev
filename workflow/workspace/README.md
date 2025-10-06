# INSTRUCTION
1. Ensure dev folder
   - Ensure a project clone `git clone . dev`
   - Ensure git ignore dev
2. Ensure pickablity
   - main-to-sub: `git remote add dev dev`
   - sub-to-main: `git -C dev remote add main .`
3. Ensure sync:
   - Ensure main `git reset --hard master`
   - Ensure sub `git -C dev reset --hard main/master`
   - check git logs
4. Excecute `workflow/modification/README.md`
5. Excecute `workflow/review/README.md`
6. On reviewed:
   - Ensure exact 1 commit in sub.
   - Ensure pick without conflict `git pull dev master --no-ff`
   - Sync sub: `git -C dev pull main master --no-ff`

# MOTIVATION
A separate workspace folder enables clean separation between meta-development as a function (the process) and meta-development as an argument (the content being developed). This isolation prevents interference with the main workflow during development and allows for safe experimentation.
