# grub-theme-stylishgrid

A simple grub theme with patterned squares background.

I created this theme in July 2020, amid of COVID lockdowns and personal issues. I tried to create a similar visual language for all my 3 laptops back then.

Icons are based on `papirus-icon-theme`.

## How to install it

1. Clone this repo:

```bash
git clone https://github.com/manu-creative-411/grub-theme-stylishgrid.git
```

2. Move the directory somewhere in your disk:

```bash
sudo mkdir -p /boot/grub/themes
sudo mv grub-theme-stylishgrid /boot/grub/themes/stylishgrid
```

⚠️ Have a second look on the final path. You will need it on the next step.

3. Config `grub` to use the theme:

```bash
sudo nano /etc/default/grub
```

```
# ADD/EDIT THIS LINE AND SET THE CORRECT PATH FOR THE THEME'S theme.txt:
GRUB_THEME=/boot/grub/themes/stylishgrid/theme.txt
```

4. Save, exit and update `grub`

```bash
sudo update-grub # Debian/Ubuntu
# or
sudo grub2-mkconfig -o /boot/grub2/grub.cfg # Fedora
```

5. Reboot. That's all.
