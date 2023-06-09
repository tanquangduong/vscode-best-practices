# vscode-best-practices
VScode is amazing!! Let's get its best practice to make our dev life easier

# Good extensions to install
- Bracket Pair Colorizer 2: for color bracket
- Prettier: for better color syntax 
- Cobalt: For color theme
- Material Icon Theme: for File icon theme
- Git History
- GitLens
- HF Code Autocomplete
- ESLint

# Good setting and shorcut to know
- Douple click on file to keep it on tab, 
- Open Editors: we can close all the file in single click
- On Git: 
    - M: modified.
    - U: Untracked
-  AutoSave: 1000 ms
- Switch between editor and terminal:
    - Ctr + !: focus to terminal
    - Ctr + M: focus to Editor
- Good shortcut keyboard
    - Ctr + :: Commend a line
    - Ctr + Shift + K: Delete a code line
- Add code shell command to Path
    - Open the repository from terminal: code .

- Write text in multiple place in Vscode: presse 'Alt' key
- Move one line of code up and dow: Alt + Up/Down arrows

# Pylint and Black for Python code formater
- Create requirement_dev.txt:
    - Pylint
    - Black
    - pycodestyle

# Configure in settings.json
```
{
    "editor.tabSize": 2,
    "eslint.validate": [
        "html",
        "javascipt",
        "javascriptreact"
    ],
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    },
    "python.linting.pycodestyleEnabled": true,
    "python.linting.pycodestyleArgs": [
        "--max-line-length=120"
    ],
    "python.linting.pylintEnabled": true,
    "python.formatting.provider": "none",
    "[python]": {
        "editor.formatOnSave": true,
        "editor.defaultFormatter": "ms-python.black-formatter"
    }
}
```