# Uzbek (Latin) Keyboard Layout for Windows

This project provides a complete **Uzbek (Latin)** keyboard layout for Microsoft Windows.  
Windows currently includes a built-in layout for **Uzbek Cyrillic**, but does not offer an equivalent for the **Uzbek Latin alphabet**.  
This project fills that gap with an official-standard Latin layout that installs system-wide, works in all applications, and behaves consistently with Windows’ existing Uzbek Cyrillic layout.

---

## ✨ Features

### ✔ Follows the Official Uzbek Latin Alphabet  
The layout implements the standard Uzbek Latin alphabet without deviations or substitutions.  
In particular, the letters **Oʻ**, **Gʻ**, and the modifier letter **ʼ** use the correct Unicode characters:

| Letter | Unicode | Notes |
|--------|---------|-------|
| Oʻ     | U+004F + U+02BB | O with a proper modifier letter turned comma above |
| Gʻ     | U+0047 + U+02BB | G with a proper modifier letter turned comma above |
| ʼ      | U+02BC           | Modifier letter apostrophe (not U+0027 or U+2019) |

These ensure correct search behavior, collation, and text compatibility.

### ✔ Matches the Windows Uzbek Cyrillic Layout  
All non-letter keys (digits, punctuation, symbols) follow the placement of the built-in **Uzbek Cyrillic** layout as closely as possible.  
Any ASCII characters that do not exist in the Cyrillic layout are placed on:

- unused key positions, or  
- **AltGr** (Right Alt) combinations.

### ✔ System-wide Installer  
The layout is built with **Microsoft Keyboard Layout Creator (MSKLC)** and includes:

- `EXE` installer  
- the original `.KLC` source file

### ✔ Includes Diagrams  
Two diagrams are included:

- the **Uzbek Latin layout itself**  
- a **dual-labeled comparison layout** showing both Latin and Cyrillic

All images are in `.webp` format for clarity and small file size.

---

## 📥 Download

The latest (and final) release is available under **GitHub Releases**:

👉 **[Download the installer](../../releases/latest)**

Choose the `.exe` installer.

---

## 🛠 Installation

1. Download the installer from the link above.  
2. Run `setup.exe`.  
3. Log out and back in (or restart Windows) if required.  
4 Select **Uzbek (Latin)** from the keyboard list if it did not happen automatically.

The layout will now be available system-wide.

---

## 📁 Included Files

```
diagrams/
  uzbek-latin.webp              # Main layout diagram
  dual-labeled.webp             # Latin + Cyrillic comparison diagram
  
src/
  uzlatn.klc                    # Keyboard Layout Creator source file

uzlatn/
  setup.exe                       # Install executable
  uzLatn_amd64.msi               
  uzLatn_i386.msi
  uzLatn_ia64.msi
  amd64/
    uzLatn.dll  
  i386/
    uzLatn.dll
  ia64/
    uzLatn.dll
  wow64/
    uzLatn.dll

```

---

## 🔧 Technical Notes

- Built using **Microsoft Keyboard Layout Creator (MSKLC)**.  
- Fully compatible with all modern Windows versions (Windows 7 → Windows 11).  
- Behaves identically to the built-in Uzbek Cyrillic layout for all non-letter keys.  
- Additional punctuation and ASCII symbols are provided via `AltGr`.

---

## 📜 License

This project is released under the **MIT License**.

---

## 🤝 Contributions

This layout is considered complete, but suggestions and issues are welcome.  
If you notice a character placement problem, feel free to open an issue.

---

## 📷 Screenshots

### Uzbek (Latin) Layout  
![Uzbek (Latin) keyboard layout](diagrams/uzlatn.webp)

### Latin–Cyrillic Comparison Layout  
![Dual-labeled Uzbek Latin-Cyrillic keyboard layouts](diagrams/dual-labeled.webp)

---

## 🧩 Background

Windows users working in Uzbek often switch between:

- the **English (US) keyboard layout** Windows defaults to for Latin-script Uzbek
- **built-in Uzbek Cyrillic layout**, and  
- **custom or improvised Latin solutions** using incorrect apostrophe characters, or mismatched punctuation.

This project provides a formal, MSKLC-based, Unicode-correct implementation of the Latin alphabet that:

- avoids inconsistent apostrophes  
- keeps symbol positions familiar  
- and matches user expectations from the Cyrillic layout.

