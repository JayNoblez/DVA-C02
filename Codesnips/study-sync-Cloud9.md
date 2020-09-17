**Commands to set up environment in Cloud9**
---

- `npm i c9 -g`
- `c9 README.md`
- `mkdir ~/environment/study-sync`
- `cd study-sync/`
- `npm init -y` (Creates a package.json file)
- `npm i express --save`
- `touch index.js index.html app.js style.css`
- `curl -s http://169.254.169.254/latest/meta-data`
- `curl -s http://169.254.169.254/latest/meta-data/network/interfaces/macs/`
- `curl -s http://169.254.169.254/latest/meta-data/network/interfaces/macs/16:32:e6:48:f6:8f/security-group-ids/`
- `aws ec2 authorize-security-group-ingress --group-id sg-03d6exxxxx --port 8080 --protocol tcp --cidr x.x.x.x/32`
- `aws ec2 describe-security-groups --group-ids sg-03d6exxxxx --output text --filters Name=ip-permission.to-port,Values=8080`
- `curl -s http://169.254.169.254/latest/meta-data/public-ipv4`
- `PORT=8080;npm start`

Server is listening on Port 8080. Now can run http:x.x.x.x/8080 to view app
Code to follow along in https://github.com/ExamProCo/TheFreeAWSDeveloperAssociate

Use this link to check your IP to configure for Security Group IP: https://checkip.amazonaws.com/

---
Creating a git repo
cd ~/environment/study-sync/
touch .gitignore
c9 .gitignore (Add node_modules to your .gitignore file.)
