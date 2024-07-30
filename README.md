# Nixos Minimal Dev Setup
 
## NixOS Configuration ReadMe

### Overview
This document describes the configuration settings for a NixOS system. The configuration includes language settings, included packages, system settings, and other relevant configurations.

### Language Settings
- **Default Locale:** `en_US.UTF-8`
- **Extra Locale Settings:**
  - `LC_ADDRESS`: `de_DE.UTF-8`
  - `LC_IDENTIFICATION`: `de_DE.UTF-8`
  - `LC_MEASUREMENT`: `de_DE.UTF-8`
  - `LC_MONETARY`: `de_DE.UTF-8`
  - `LC_NAME`: `de_DE.UTF-8`
  - `LC_NUMERIC`: `de_DE.UTF-8`
  - `LC_PAPER`: `de_DE.UTF-8`
  - `LC_TELEPHONE`: `de_DE.UTF-8`
  - `LC_TIME`: `de_DE.UTF-8`

### Keymap Settings
- **Console Keymap:** `de`
- **X11 Keymap:** `de`

### Time Zone
- **Time Zone:** `Europe/Berlin`

### Included Packages
The system is configured to include the following packages:
- `librewolf`
- `vscode-fhs`
- `vesktop`
- `openrgb-with-all-plugins`
- `docker-compose`
- `steam-run`
- `thunderbird`
- `git`
- `wget`

### Other Relevant Settings
- **Nix Settings:**
  - Auto-optimise store enabled
  - Experimental features: `nix-command`, `flakes`
  - Automatic garbage collection set to weekly with options to delete older than 7 days

- **Boot Loader:**
  - Systemd-boot enabled
  - EFI variables accessible

- **Networking:**
  - Hostname: `nixos`
  - NetworkManager enabled

- **Desktop Environment:**
  - X11 enabled
  - GNOME Desktop Environment enabled

- **Flatpak:** Enabled

- **Virtualisation:** Docker enabled

- **Firefox:** Disabled

- **Unfree Packages:** Allowed

- **Steam:** Enabled with remote play and dedicated server firewall options

- **Fonts:**
  - Packages:
    - Source Code Pro
    - Noto Fonts
    - Noto Fonts CJK
    - Twitter Color Emoji
    - Font Awesome
    - Powerline Fonts
    - Nerd Fonts Symbols Only
  - Fontconfig: Autohint enabled

### Disclaimer
This configuration is tailored for a specific setup and may require adjustments to fit your particular use case. It is not recommended to use this configuration without understanding and modifying it to meet your own system requirements.

### License
This configuration is licensed under the GNU General Public License. For more details, refer to the full license text at [GNU's official website](https://www.gnu.org/licenses/gpl-3.0.en.html).

---

Feel free to reach out for any further clarifications or modifications regarding this configuration.
