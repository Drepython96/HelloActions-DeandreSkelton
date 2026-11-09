# HelloActions-DeandreSkelton
This project runs a Python greeting program using GitHub Actions
## How the workflow works

1. The `on` section defines what starts the workflow. In this project, a push to `main` starts it automatically.
2. `workflow_dispatch` lets me start the workflow manually from the Actions tab.
3. `runs-on` specifies the runner for the job. This workflow uses a GitHub-hosted Ubuntu runner.
4. `actions/checkout` copies the repository files onto the runner so it can access `hello.py`.
5. `actions/setup-python` makes Python 3.12 available on the runner.
6. Compiling translates source code into another form, such as bytecode or machine code. Running executes the program. This workflow runs the script directly with `python hello.py`, so it needs no separate compile step.
7. The program output appears in the Actions tab. Open a workflow run, select the job, and expand the `Run the Python program` step.
8. A workflow is the whole automated process. A job is a group of steps that run on the same runner. A step is one action or command in a job.

## AI use

I used ChatGPT for step-by-step guidance and help drafting the Python script, workflow, and README explanation. I created the repository, committed the files, and ran the workflow in GitHub.
