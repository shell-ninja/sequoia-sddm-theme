<h1 align='center'>Updated Sequoia SDDM Theme</h1>

I have updated the base [Sequoia](https://codeberg.org/minMelody/sddm-sequoia) sddm theme for myself. <br>
Download the original from [pling](https://www.pling.com/p/2191680/).

### Dependencies

> [!NOTE]
> Package names used below are for Arch Linux, packages may vary for your distro

- sddm
- a [Nerd Font](https://www.nerdfonts.com/font-downloads) installed system-wide >= v3.0
- qt6 >= 6.6
  - qt6-declarative
  - qt6-5compat

### Installation

Clone this repository:

```bash
git clone --depth=1 https://github.com/shell-ninja/sequoia-sddm-theme.git

sudo cp -r sequoia-sddm-theme /usr/share/sddm/themes/
```

Now follow these steps:

```bash
sudo mkdir -p /etc/sddm.conf.d/
sudo nvim /etc/sddm.conf.d/theme.conf.user

echo -e "[Theme]\nCurrent=sequoia-sddm-theme" | sudo tee /etc/sddm.conf.d/theme.conf.user
```

Now logout and see the changes.
