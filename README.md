This git hook aborts a commit to a Python project if any unit test matching the pattern '*_test.py' in the project's test/ directory fails. This is useful to avoid broken commits and to facilitate bisection debugging.

To install the pre-commit hook simply copy it to a .git/hooks/ directory in your repository. You might have to create the directory if it does not exist.

- DO inspect the pre-commit script before installing it
- DO NOT symlink to the hook as this is a security risk
