# Color Scheme Update

This is a step by step guide to updating the color scheme of my Arch Linux Setup.
Color schemes should come from [base16](https://github.com/chriskempson/base16) so that
management and unification of color schemes will be easy.

## Sway

- Download theme from [base16-sway](https://github.com/rkubosz/base16-sway)
- Place in $XDG_CONFIG_HOME/sway
- Add `include ~/.config/sway/${theme-name}` to the config file.

## Kitty

- Download theme from [base16-kitty](https://github.com/kdrag0n/base16-kitty)
- Copy contents to kitty.conf, which is found in $XDG_CONFIG_HOME/kitty

## Fish

Setting the color scheme for the shell is not enough for fish as the syntax-highlighting
colors are not correctly set. This is fixed by explicitly setting color variables using
[base16-fish](https://github.com/tomyun/base16-fish)

- Install base16-fish by `fisher add tomyun/base16-fish`
- run `base16-${theme-name}`
- Uninstall base16-fish by `fisher rm tomyun/base16-fish`
-- base16-fish is uninstalled because a flash of text with errors due to base16-fish
appears on startup
