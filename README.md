# Setup

1. Install and enable Sync Setting extension - [zokugun.sync-settings](https://open-vsx.org/vscode/item?itemName=zokugun.sync-settings)
2. `cmd/ctrl+shift+p` and run `Sync Settings: Open the profile settings.`
3. Copy/Paste the code below:

```yml
hostname: "AvellBook"
profile: main
repository:
  type: git
  url: git@github.com:AdsonCicilioti/vscode-settings.git
  branch: main
  messages:
    init: "profile({{profile}}): init -- {{now|date:iso}}"
    update: "profile({{profile}}): update -- {{now|date:iso}}"
```

4. Save it and run `cmd/ctrl+shift+p` > `Sync Settings: Download repository`
