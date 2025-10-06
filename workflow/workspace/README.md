# INSTRUCTION
Usage: Execute with argument 'setup' or 'develop'

1. If argument is 'setup':
   - Ensure dev folder `git clone . dev`
   - Ensure git ignore dev
   - Ensure pickability:
     - main-to-sub: `git remote add dev dev`
     - sub-to-main: `git -C dev remote add main .`
   - Ensure sync:
     - Ensure main `git pull origin master --rebase`
     - Ensure sub `git -C dev pull main master --rebase`
     - check git logs

2. If argument is 'develop':
   - Execute `workflow/modification/README.md`
   - Execute `workflow/review/README.md`
   - On reviewed:
     - Ensure exact 1 commit in sub.
     - Ensure pick without conflict `git pull dev master --rebase`
     - Sync sub: `git -C dev pull main master --rebase`
     - Backup: `git push origin master`

# MOTIVATION
A separate workspace folder enables clean separation between meta-development as a function (the process) and meta-development as an argument (the content being developed). This isolation prevents interference with the main workflow during development and allows for safe experimentation.
