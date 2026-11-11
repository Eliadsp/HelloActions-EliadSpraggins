# HelloActions-EliadSpraggins

- The `on` section lists the events that start the workflow. This one runs when code is pushed to `main`.
- `workflow_dispatch` lets someone start the workflow manually from GitHub’s Actions tab.
- `runs-on` selects the machine that runs the job. This workflow uses `ubuntu-latest`.
- `actions/checkout` checks out the repository so the runner can access its files.
- A language setup action installs or selects a language version when needed. This Python workflow uses the Python already available on the runner, so it does not need a separate setup action.
- Compiling translates source code into an executable form; running executes the program. Python is interpreted, so this workflow runs `hello.py` directly.
- The program's output appears in the workflow run log in the Actions tab.
- A workflow contains one or more jobs. Each job contains steps that run in sequence.