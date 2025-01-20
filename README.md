# alacritty-

Your favorite color schemes now in alacritty  🎨

To install we have two options, install manually or import the theme file, we will show you both options. Let's start with the simplest one, which is to clone the repository and import the theme file directly into your dotfile.

```shell
mkdir -p ~/.config/alacritty/themes
git clone https://github.com/neko-night/alacritty ~/.config/alacritty/themes
```

Add an import to your alacritty.toml (Replace {theme} with your desired colorscheme):

```toml 
[general]
import = [
    "~/.config/alacritty/themes/themes/{theme}.toml"
]
```

If you want to install it manually, you will have to copy the theme content and paste it into your dotfile, let's put an example dotfile.

```toml 
[window]

opacity = 0.6

padding.x = 10
padding.y = 10

decorations = "Full"
decorations_theme_variant = "Dark"

[font]

normal.family = "JetBrains Mono"
bold.family = "JetBrains Mono"
italic.family = "JetBrains Mono"
bold_italic.family = "JetBrains Mono"

size = 15.0

[terminal]

[terminal.shell]
program = "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
args = ["-NoLogo", "-NoExit", "-Command", "Set-Location -Path 'C:\\Users\\Usuario'"]

# -----------------------------------------------------------------------------
# nekonight Alacritty Colors
# Theme: Neko Night
# Upstream: https://github.com/BrunoCiccarino/nekonight/raw/main/extras/alacritty/nekonight_night.toml
# -----------------------------------------------------------------------------

[colors.primary]
background = '#262835'
foreground = '#c0caf5'

[colors.cursor]
cursor = '#c0caf5'
text = '#1a1b26'

[colors.normal]
black = '#15161e'
red = '#f7768e'
green = '#9ece6a'
yellow = '#e0af68'
blue = '#7aa2f7'
magenta = '#bb9af7'
cyan = '#7dcfff'
white = '#a9b1d6'

[colors.bright]
black = '#414868'
red = '#ff899d'
green = '#9fe044'
yellow = '#faba4a'
blue = '#8db0ff'
magenta = '#c7a9ff'
cyan = '#a4daff'
white = '#c0caf5'

[[colors.indexed_colors]]
index = 16
color = '#ff9e64'

[[colors.indexed_colors]]
index = 17
color = '#db4b4b'
```

<img src="https://raw.githubusercontent.com/BrunoCiccarino/nekonight/refs/heads/main/img/line-gradient.svg" alt="line break" width="100%" height="3px">
