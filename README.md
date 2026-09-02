# 🛡️ BlackCatOfficial's Blocking Trash Ads (Made in VN)

Specialized ad-blocking filter list for **uBlock Origin** and **uBlock Origin Lite**, created by a Vietnamese developer to block ads that standard lists miss — especially on Vietnamese websites.

> [!IMPORTANT]
> **This list is designed EXCLUSIVELY for [uBlock Origin](https://github.com/gorhill/uBlock) and [uBlock Origin Lite](https://github.com/uBlockOrigin/uBOL-home).**
>
> It uses `!#include` directives and filter syntax not supported by Adblock Plus (ABP) or AdGuard.
>
> **Disable Adblock/Adblock Plus/AdGuard before installing** (unless using the direct import URL below).

---

## 🚀 Quick Install

### Option 1: One-click subscribe (recommended)
[![Subscribe to uBlock Origin](https://img.shields.io/badge/Subscribe-uBlock%20Origin-green?style=for-the-badge&logo=ublockorigin)](https://subscribe.adblockplus.org/?location=https://github.com/BlackCatOfficialytb/BlackCatOfficial-ubo-filter/raw/refs/heads/main/filter.txt)

### Option 2: Manual import
In uBlock Origin → Settings → Filter lists → Import → paste:
```
https://github.com/BlackCatOfficialytb/BlackCatOfficial-ubo-filter/raw/refs/heads/main/filter.txt
```

---

## 📦 Filter Modes

| Mode | File | Description |
|------|------|-------------|
| **Standard** | `filter.txt` | Balanced blocking — safe for daily use |
| **Extreme** | `extreme_filter.txt` | Aggressive blocking — may break sites |

> **Extreme mode** includes everything in Standard plus `filter5_d3ward.txt` and `filter9_vn_adlink_ads_extreme.txt`. Use with caution.

---

## 🛠️ Modular Structure

```
filter.txt (Standard Loader)
├── filter1_clickadu.txt              # Clickadu ad network
├── filter2_ez4short.txt              # Ez4short URL shortener ads
├── filter3_scriptlet_antiadblockdetection.txt  # Anti-adblock scripts
├── filter4_malware.txt               # Malware domains
├── filter6_misc.txt                  # Miscellaneous filters
├── filter7_banner.txt                # Banner ads
├── filter8_vn_adlink_ads_standard.txt # VN adlink ads (standard)

extreme_filter.txt (Extreme Loader)
├── filter.txt                        # All standard modules
├── filter5_d3ward.txt                # D3ward anti-adblock
└── filter9_vn_adlink_ads_extreme.txt # VN adlink ads (aggressive)
```

Each module can be inspected or disabled individually in uBlock Origin's logger.

---

## 📋 Requirements

- uBlock Origin (Chrome/Firefox/Edge/Safari)
- **OR** uBlock Origin Lite (MV3 — limited `!#include` support)

---

## 🚩 Report Issues

Found a Vietnamese site still showing ads or broken by the filter?
[Open an issue](https://github.com/BlackCatOfficialytb/for-ublock-with-love/issues) with:
- Site URL
- Screenshot
- uBlock Origin logger export (if possible)

---

## 📄 License

Apache 2.0 — free to use, modify, and distribute.

---

## 🙏 Credits

- [ABPVN](https://github.com/abpvn/abpvn) — Vietnamese filter base
- [uBlock Origin](https://github.com/gorhill/uBlock) — The best ad blocker
- Community reporters