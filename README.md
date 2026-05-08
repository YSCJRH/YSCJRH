# YSCJRH

## Codex Pet

![Emerald Codex Guardian](assets/codex-pets/emerald-codex-guardian/profile-readme.gif)

**Emerald Codex Guardian** is my Codex pet: a white-haired, emerald-crowned chibi mage inspired by my GitHub avatar.

She is packaged for local Codex use and kept here with the source preview assets.

Working state:

![Emerald Codex Guardian casting a spell](assets/codex-pets/emerald-codex-guardian/running.gif)

### Files

- [Install package](assets/codex-pets/emerald-codex-guardian/emerald-codex-guardian.codex-pet.zip)
- [Spritesheet](assets/codex-pets/emerald-codex-guardian/spritesheet.webp)
- [All actions preview](assets/codex-pets/emerald-codex-guardian/all-actions.webp)
- [Working spell loop](assets/codex-pets/emerald-codex-guardian/running.gif)

### Local Install

```powershell
$pet = "$env:USERPROFILE\.codex\pets\emerald-codex-guardian"
New-Item -ItemType Directory -Force -Path $pet | Out-Null
Invoke-WebRequest `
  -Uri "https://raw.githubusercontent.com/YSCJRH/YSCJRH/main/assets/codex-pets/emerald-codex-guardian/emerald-codex-guardian.codex-pet.zip" `
  -OutFile "$env:TEMP\emerald-codex-guardian.codex-pet.zip"
Expand-Archive -Path "$env:TEMP\emerald-codex-guardian.codex-pet.zip" -DestinationPath $pet -Force
```

After installation, select `Emerald Codex Guardian` from Codex pet/avatar settings.
