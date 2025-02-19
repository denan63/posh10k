# Posh10k - Theme for oh-my-posh inspired by the Powerlevel10k's Rainbow theme

![posh10k_preview](https://github.com/user-attachments/assets/0594eaf5-9066-4eab-a6d6-55bc768130f3)

**Important:** This theme primarily relies on the terminal color scheme, so it may look different from the screenshot above!

## Windows Terminal Setup

1. Install a [compatible font](https://github.com/romkatv/powerlevel10k#manual-font-installation)
2. Open Terminal settings by pressing `Ctrl + ,` and set a Nerd Font in `Profiles > Defaults > Appearance > Font face`
3. Install [oh-my-posh](https://ohmyposh.dev/)
4. Install [posh-git](https://github.com/dahlbyk/posh-git)

```powershell
Install-Module posh-git -Scope CurrentUser -Force
```

5. Run the following command to save this theme configuration file in your home directory:

```powershell
curl https://raw.githubusercontent.com/denan63/posh10k/main/posh10k_rainbow.omp.json -o "$HOME\posh10k_rainbow.omp.json"
```

6. Open `$PROFILE` in your preferred text editor (e.g., `nvim $PROFILE`) and add the following lines:

```powershell
Import-Module posh-git
oh-my-posh init pwsh --config ~/posh10k_rainbow.omp.json | Invoke-Expression
```

7. Restart the terminal.

## Customization
If you want to customize this theme, edit the `.json` file in a text editor of your choice.
The full tutorial is available [here](https://ohmyposh.dev/docs/installation/customize).

## Credits
File [`posh10k_rainbow.omp.json`](./posh10k_rainbow.omp.json) is a modified version of the original [Jan De Dobbeleer's theme](https://github.com/JanDeDobbeleer/oh-my-posh/blob/main/themes/powerlevel10k_rainbow.omp.json) (MIT License).
