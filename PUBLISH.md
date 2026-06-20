# Publish This Repository

GitHub CLI is installed, but it must be authenticated first.

Run this in PowerShell:

```powershell
$env:Path = [System.Environment]::GetEnvironmentVariable('Path','Machine') + ';' + [System.Environment]::GetEnvironmentVariable('Path','User')
gh auth login --hostname github.com --web --clipboard --git-protocol https
gh auth status
```

After authentication succeeds, publish:

```powershell
cd C:\Users\22381\Desktop\EARNMONEY\ai-batch-services
git init
git add .
git commit -m "Create AI batch services desk"
gh repo create ai-batch-services --public --source . --remote origin --push
```

The repository links have already been set to:

```text
https://github.com/ahshicr/ai-batch-services
```
