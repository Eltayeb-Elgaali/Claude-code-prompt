```bash
write a bash script that prints how much free disk space is left
```
```bash
why does 'permission denied' show up when I run ./deploy.sh
```
```bash
explain this command: find . -name '*.log' -mtime +7 -delete
```
```bash
Explain what the command tar -xzf backup.tar.gz does, in two sentences, for someone new to Linux
```
```bash
You are a terse Linux tutor. Answer in one sentence, no preamble.
```
```bash
In two sentences, explain what git rebase does and when to use it, for someone who already knows git merge
```
```bash
You are a senior Linux server administrator. How do I find what is using disk space?
```
```bash
Write a bash script that lists the five biggest files in the current folder
```
```bash
mkdir -p /root/scripts
claude -p "Write a bash script that prints how much free disk space is left on this machine. Reply with only the raw script text, starting with #!/bin/bash, and no markdown code fences." > /root/scripts/diskcheck.sh
sed -i '/^`\{3\}/d' /root/scripts/diskcheck.sh
chmod +x /root/scripts/diskcheck.sh
bash /root/scripts/diskcheck.sh
```
```bash
explain this command: find . -name '*.log' -mtime +7 -delete
```


