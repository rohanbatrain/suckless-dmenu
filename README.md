# suckless-dmenu (Dynamic Menu)

![2](https://github.com/user-attachments/assets/a09bb93c-0aab-43e2-9386-eaca37f62c5d)

A personal fork of the [suckless dmenu](https://tools.suckless.org/dmenu/) — a dynamic menu for X — enhanced with modular builds, aesthetic improvements, and key usability patches.

---

## 🧩 About

This repository contains a customized version of `dmenu` designed to align with my workflow. While preserving the core suckless principles — minimalism, speed, and clarity — this fork adds enhancements to improve daily usability without bloating the codebase.

### Key Goals

- Keep `dmenu` lightweight and minimal  
- Add essential patches (fuzzy matching, centering, Xresources)  
- Maintain upstream compatibility  
- Modularize versions for clean updates and experimentation

---

## 🚀 Features

- **Fuzzy match** support  
- **Centered layout** with customizable width  
- **Xresources** theming support  
- **Emoji & Unicode** compatibility  
- **Clean versioning** (e.g., `v5.2`) for tracking config and patch combinations  
- **Minimal and fast**, true to suckless design  

---

## 🛠️ Installation

### Prerequisites

Ensure the following dependencies are installed:

```bash
make
gcc
libX11
libXft
fontconfig
```

### Clone and Build

```bash
git clone https://github.com/rohanbatrain/suckless-dmenu.git
cd suckless-dmenu
sudo make clean install
```

To install for your user only (no `sudo`):

```bash
make clean install PREFIX=$HOME/.local
```

---

## 🧪 Usage

To run `dmenu`:

```bash
dmenu_run
```

Or pipe a list into it:

```bash
ls | dmenu
```

To bind `dmenu_run` to a key (e.g., in dwm):

```c
{ MODKEY, XK_p, spawn, SHCMD("dmenu_run") },
```

---

## 🧬 Customization

Tweak options in `config.h` to change:

- Fonts and font size  
- Color schemes  
- Menu width, alignment, position  
- Prompt string and layout  
- Matching style (fuzzy, exact, etc.)

Rebuild with:

```bash
sudo make clean install
```

---

## 🧾 Version History

| Version | Description                 | Date        |
|---------|-----------------------------|-------------|
| v5.2    | Fuzzy match + center layout | May 3, 2023 |

---

## 📜 License

Licensed under the MIT License, same as the original suckless `dmenu`.

---

## 🤝 Credits

- [suckless.org](https://suckless.org) for the original `dmenu`
- Community patch maintainers for their minimalist brilliance

---

> _"Simple. Fast. Yours."_


 
