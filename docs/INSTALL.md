# Install Polpo Claude Skills

This guide explains how to install selected skills either globally (`~/.claude/skills/`) or per project (`.claude/skills/`).

## Security warning

Do **not** store secrets in skill files.

Never include:
- credentials
- API keys
- tokens
- private client data
- production secrets

Skills are instruction files, not secret stores.

## Linux/macOS

### Copy selected skills to global Claude skills

```bash
mkdir -p ~/.claude/skills
cp -R skills/polpo-technical-operator ~/.claude/skills/
cp -R skills/polpo-claude-prompt-auditor ~/.claude/skills/
```

### Symlink selected skills to global Claude skills

```bash
mkdir -p ~/.claude/skills
ln -s "$(pwd)/skills/polpo-n8n-architect" ~/.claude/skills/polpo-n8n-architect
ln -s "$(pwd)/skills/polpo-client-delivery" ~/.claude/skills/polpo-client-delivery
```

### Copy selected skills to a project-local Claude folder

```bash
mkdir -p .claude/skills
cp -R skills/polpo-frontend-implementation .claude/skills/
```

### Symlink selected skills to a project-local Claude folder

```bash
mkdir -p .claude/skills
ln -s "$(pwd)/skills/polpo-technical-operator" .claude/skills/polpo-technical-operator
```

## Windows PowerShell

### Copy selected skills to global Claude skills

```powershell
New-Item -ItemType Directory -Force "$HOME/.claude/skills" | Out-Null
Copy-Item -Recurse -Force "skills/polpo-technical-operator" "$HOME/.claude/skills/"
Copy-Item -Recurse -Force "skills/polpo-claude-prompt-auditor" "$HOME/.claude/skills/"
```

### Symlink selected skills to global Claude skills

```powershell
New-Item -ItemType Directory -Force "$HOME/.claude/skills" | Out-Null
New-Item -ItemType SymbolicLink -Path "$HOME/.claude/skills/polpo-n8n-architect" -Target "$(Get-Location)\skills\polpo-n8n-architect" | Out-Null
New-Item -ItemType SymbolicLink -Path "$HOME/.claude/skills/polpo-client-delivery" -Target "$(Get-Location)\skills\polpo-client-delivery" | Out-Null
```

### Copy selected skills to a project-local Claude folder

```powershell
New-Item -ItemType Directory -Force ".claude/skills" | Out-Null
Copy-Item -Recurse -Force "skills/polpo-frontend-implementation" ".claude/skills/"
```

### Symlink selected skills to a project-local Claude folder

```powershell
New-Item -ItemType Directory -Force ".claude/skills" | Out-Null
New-Item -ItemType SymbolicLink -Path ".claude/skills/polpo-technical-operator" -Target "$(Get-Location)\skills\polpo-technical-operator" | Out-Null
```
