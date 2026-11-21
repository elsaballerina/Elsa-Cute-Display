# 🌸 Elsa-Cute-Display v1.0 ✨

![Fedora](https://img.shields.io/badge/Fedora-Workstation-51A2DA?style=for-the-badge&logo=fedora&logoColor=white)
![GNOME](https://img.shields.io/badge/GNOME-Wayland-4A86CF?style=for-the-badge&logo=gnome&logoColor=white)
![GTK4](https://img.shields.io/badge/GTK4-Libadwaita-4A86CF?style=for-the-badge&logo=gtk&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-ff69b4?style=for-the-badge)

A lightweight, cute, native **GTK4 + Libadwaita** display profile manager for **Fedora Workstation (GNOME on Wayland)**.

Built to solve the frustration of DisplayLink docking stations and multi-monitor setups resetting their positions, rotations, and primary display every time you reboot, unplug, or switch docks.

---

## ✨ Features

* **Serial-Number Aware Capture:** Uses GNOME's `gdctl` to match monitors by their unique hardware serial numbers—so DisplayLink virtual port shuffling never breaks your layout.
* **One-Click Capture & Save As:** Save any monitor arrangement as a standalone, reusable `.sh` profile in `~/bin/display-profiles`.
* **⚡ Instant Quick-Apply Dropdown:** Switch between multiple docking stations or solo laptop setups in one click.
* **⌨️ Live Keyboard Shortcut Capture:** Press your actual key combination (e.g., `Ctrl+Alt+4`) to bind it directly in GNOME Settings, complete with a **Duplicate Shortcut Warning (Yes/No overwrite)**.
* **📂 Profile Management:** Apply, rebind shortcuts, delete profiles, open your profiles folder directly in your file manager, or refresh the list.
* **🌙 Light & Dark Mode Toggle:** Native Libadwaita adaptive styling.
* **Offline & Lightweight:** Runs natively on Fedora Workstation with zero background daemons.

---

## 📸 Screenshots

*(Tip: Drag and drop a screenshot of Elsa-Cute-Display in Light and Dark mode right here in the GitHub editor!)*
<img width="580" height="751" alt="Elsa-Cute-Display-Screenshot-Dark" src="https://github.com/user-attachments/assets/81512e83-30aa-4932-b359-ccbd25299ce6" />
<img width="580" height="751" alt="Elsa-Cute-Display-Screenshot-Light" src="https://github.com/user-attachments/assets/a8051b84-90da-442c-92f0-de5d07f6bd7f" />

---

## 🚀 Quick Start (Download & Run)

1. Download the latest compiled **`Elsa-Cute-Display`** binary from the [Releases](../../releases) page.
2. Right-click the file in GNOME Files → **Properties** → turn on **Executable as Program** (or run `chmod +x Elsa-Cute-Display` in terminal).
3. Double-click (or right-click → **Run as a Program**) to launch!

---

## 🛠️ How to Use

1. **[1]** Arrange your screens manually in **Fedora Settings → Displays**.
2. **[2]** Open **Elsa-Cute-Display** and click **💾 Capture & Save As...** to save your profile (e.g., `home-dock-4screens.sh`).
3. **[3]** Use the **⚡ Quick-Apply** dropdown or click **Apply** anytime your layout resets.
4. **[4]** Click **⌨️ Shortcut** next to any profile and press your desired key combo to trigger it instantly from anywhere.

---

## 💻 Run From Source

### Prerequisites
Fedora Workstation (GNOME on Wayland) includes everything needed out of the box (`python3`, `python3-gobject`, `gtk4`, `libadwaita`, and `gdctl`). On minimal installs, run:
```bash
sudo dnf install python3 python3-gobject gtk4 libadwaita
