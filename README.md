# Notes App — Pipeline-ready repo

This repository skeleton contains the minimal files to get started with:
GitHub → CodePipeline → CodeBuild → CodeDeploy → EC2 (with CloudWatch agent).

Files included:
- index.html
- css/style.css
- js/app.js
- appspec.yml
- buildspec.yml
- scripts/clean_old.sh
- scripts/restart_server.sh

**After cloning** run:
```bash
chmod +x scripts/*.sh
git add .
git commit -m "Add pipeline + codedeploy config"
git push origin main
```

The EC2 user-data provided in this package uses **ap-south-1** (Mumbai). Replace the region string if you will launch instances in a different region.
