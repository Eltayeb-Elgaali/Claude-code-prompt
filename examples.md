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
Reverse engineer an existing web app from outside with REA, then rebuild its core as a new app.
Never copy its code, text, images, logo, name or exact visual design.
App to study: www.azerty.com
New: name: xxxx
Look: Arabic interface, right to left, font xx. Colour    
```
```bash
In /root/deploy.sh, the rsync command drops the trailing slash on $SRC so it
copies the folder instead of its contents. Fix that line and leave the rest
unchanged.
```
```bash
claude -p --permission-mode plan "Outline the steps to add config backups to /root/tool.sh. Do not change any files."
```
```bash
cat > /root/brief.md <<'EOF'
Goal: a greeting script for our servers.
Target file: /root/greet.sh
Done when: running it prints "Hello from <hostname>" using the real hostname,
and it exits 0.
EOF

claude -p --permission-mode acceptEdits "Build the script described in /root/brief.md"

chmod +x /root/greet.sh
/root/greet.sh > /root/greet.out
cat /root/greet.out
```
```bash
# Acme API

## Commands
- Build: `make build`
- Test: `pytest -q`
- Run locally: `make dev` (needs `DATABASE_URL`)

## Conventions
- 4-space indent, type hints on all public functions
- New routes go in `src/routes/`, one file per resource

## Gotchas
- `generated/` is rebuilt by `make build`; never edit it by hand
```
```bash
Running diskspace.sh gives: "line 5: DIR: unbound variable". Fix it so it runs cleanly.
Run the test and, if it fails, fix the cause and run it again until it passes.
```
```bash
You are a terse Linux tutor. Answer in one sentence, no preamble.
```
```bash
You are a terse Linux tutor. Answer in one sentence, no preamble.
```
```bash
You are a terse Linux tutor. Answer in one sentence, no preamble.
```
```bash
You are a terse Linux tutor. Answer in one sentence, no preamble.
```




