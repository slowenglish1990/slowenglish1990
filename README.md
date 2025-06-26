services:
  - type: worker
    name: slowenglish1990
    runtime: python
    repo: https://github.com/slowenglish1990/slowenglish1990
    plan: free
    region: oregon
    buildCommand: pip install -r requirements.txt
    startCommand: python app.py
    autoDeployTrigger: commit
version: "1"
