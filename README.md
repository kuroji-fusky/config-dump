# Kuro's Config Dump and dotfiles

Here are my scripts I need for my machines to keep an optimal and consistent workflow

----

> **Note**
> Running `bootstrap.ps1` will require admin privilages and allow the script by
> bypassing its Execution Policy:

```powershell
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser; .\bootstrap.ps1
```

## Todo


### `bootstrap.ps1`
- [ ] The script needs to check for additonal files so it can run on its own and
  download them via `Invoke-WebRequest`
- [ ] Remove Windows 11 bloat
- [ ] When the script is ran on fresh install on Win10/11, make it run `winget`,
  after that, include a `--skip-winget` param to source it with `. .\bootstrap.ps1`
  - [ ] add PATH variables since winget for some goddamn reason won't do it 
    automatically
  - [ ] Include O&O ShutUp10++ and `Invoke-WebRequest` the config file on this repo