## Coding Preferences
- For filter and map, use 'e' as the element parameter, unless nested within another functional method
- For reduce, call the accumulator 'acc'
- Use ternaries for simple conditionals
- Don't include comments in code
- Don't introduce myself

## Workspace
- Put files I create/work on for tasks inside the `projects/` folder (it's in .gitignore)

## Git Workflows

### New Repository Setup
Commands for pushing code to a new GitHub repo:
```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:lucy-the-lobster/<repo-name>.git
git push -u origin main
```

