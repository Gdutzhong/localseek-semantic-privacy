# Privacy Policy — LocalSeek Semantic

**Last updated:** June 2026 (app version **1.0.3**)  
**Publisher:** Phoenix X ("we", "us")  
**Contact:** [lqzforlyman@outlook.com](mailto:lqzforlyman@outlook.com)

This Privacy Policy describes how **LocalSeek Semantic** (the "App") handles information when you install and use the App distributed through the **Microsoft Store**.

---

## Summary

LocalSeek Semantic is a **local desktop search utility** for Windows. Your documents are indexed and searched **on your device**. We do **not** collect, store, or transmit your file contents, search queries, or indexes to Phoenix X.

- **Free tier:** filename, path, extension, and date search — always available on-device.  
- **Pro tier:** semantic / content search inside documents (15-day in-app trial, then optional one-time purchase via Microsoft Store).  
- **Embedding model** (BGE-small-en-v1.5) is **bundled with the App**. No model download from our servers is required for normal use.  
- **License, trial, and purchase** flows are handled by **Microsoft** through the Microsoft Store.  
- **No advertising SDKs** and **no third-party analytics SDKs** are included.

---

## Information processed on your device

The App reads and stores the following **locally** to provide search:

| Data | Purpose | Sent to Phoenix X? |
|------|---------|-------------------|
| **Folders you choose** (via Folder Picker) | Scope indexing and search | No |
| **File metadata** (name, path, size, dates, extension) | Free filename search | No |
| **Document text chunks & vector embeddings** (Pro) | Semantic / content search | No |
| **Search queries you type** | Run search on-device | No |
| **In-app preferences** (see below) | Remember your settings | No |
| **Local diagnostic logs** (optional, on errors/startup) | Troubleshooting on your PC | No |

### In-app preferences stored locally

Preferences are saved in Windows **Application Data** (`LocalSettings`) on your device, including:

- Watched folders and indexing options  
- Custom / disabled file extensions (Pro)  
- License UI state and trial reminder flags  
- Onboarding and in-app coach-mark state  
- **Minimize to system tray on close** (Settings → General; default: on)  
- **Global shortcut** settings (enabled/disabled, key combination, shortcut type)

We do **not** require you to create a Phoenix X account to use the App.

### Pro trial timestamp (Microsoft account roaming)

For Store builds, the App records a **Pro trial start time** in Windows **roaming settings** (synced by Microsoft to your Microsoft account, like other Store app settings). This is used only to enforce the **15-day in-app Pro trial**. Phoenix X does not receive this timestamp.

---

## System tray and background operation

When **Minimize to tray on close** is enabled (default), closing the window hides it to the **system tray** instead of quitting. The App may continue running locally so you can restore it from the tray icon.

- Tray menu actions (Show, Settings, Exit) are handled on your device.  
- **No additional background network activity** is added for tray operation.  
- To fully quit, use **Exit** from the tray menu or turn off **Minimize to tray** in Settings → General and close the window again.

---

## Global keyboard shortcut

In **Settings → General**, you can enable a **global shortcut** to show or hide the App (default: **Ctrl+Shift+S**; Free and Pro users).

How it works:

| Shortcut type | Windows mechanism | What we access |
|---------------|-------------------|----------------|
| Modifier + key (e.g. Ctrl+Shift+S) | `RegisterHotKey` | **Only** your chosen combination |
| Double-tap modifier (e.g. Ctrl+Ctrl) | Low-level keyboard hook | **Only** the selected modifier key, to detect a double-press |

- We do **not** log, record, or transmit other keystrokes or clipboard content.  
- Shortcut preferences are stored **only on your device**.  
- You can disable the shortcut at any time in Settings → General.

---

## Local diagnostic logs

If the App encounters errors or during startup, it may append **local log files** on your device (for example `startup.log`, `diagnostics.log`, or `crash.log`) under:

- `%LocalAppData%\...\LocalSeekSemantic\` (primary), or  
- fallback folders under Documents / Temp if the primary path is unavailable.

These logs may contain **technical messages, file paths, and exception details**. They are **not uploaded automatically**. You may delete them by removing the App data folder or using **Settings → Clear all local data**.

---

## Where data is stored

| Location | Contents |
|----------|----------|
| `%LocalAppData%\...\LocalSeekSemantic\index\` | Metadata database, Pro content index, vector index files |
| Windows `LocalSettings` | App preferences (folders, shortcuts, UI state) |
| Windows `RoamingSettings` | Pro trial start time (Store builds) |

Exact paths depend on your Windows user profile and MSIX package install location.

---

## Network use

The App is designed for **offline search**. Network access is limited to:

| Activity | When | Data involved | Recipient |
|----------|------|---------------|-----------|
| **Microsoft Store** — purchase, restore, license check | Upgrade, restore, or license refresh | Microsoft account & purchase status (Microsoft's policy) | Microsoft |
| **Opening links you choose** | e.g. Privacy policy, support email, third-party license page in browser | Depends on the link you open | Respective site / your email provider |

The App does **not** upload your documents, indexes, or search history to Phoenix X servers. We do not operate cloud sync or user analytics for this App.

---

## Permissions and capabilities

The Store package declares **`runFullTrust`** so the App can run as a full desktop application on Windows. This is required for:

- Local folder indexing and file access you approve  
- System tray icon and menu  
- Global keyboard shortcut registration  

This capability does **not** grant Phoenix X remote access to your device. It only allows the App to use standard Windows desktop APIs on your PC.

The App requires **Microsoft .NET** and the **Windows App Runtime** (as disclosed in the Store listing). Those components are provided by Microsoft.

---

## Microsoft Store

Purchase, billing, and account-related data are handled under Microsoft's policies:

- [Microsoft Privacy Statement](https://privacy.microsoft.com/en-us/privacystatement)  
- [Microsoft Store Terms](https://www.microsoft.com/en-us/store/b/terms-of-sale)

---

## Data retention and deletion

You can remove local App data at any time:

- **Settings → Clear all local data** — removes indexes and related local databases  
- **Uninstall** — removes the MSIX package; app data under `%LocalAppData%\...\LocalSeekSemantic\` may remain until you delete it or use in-app clear  

Roaming trial settings may persist in your Microsoft account until cleared through Windows / account sync behavior.

---

## Open-source components

LocalSeek Semantic includes open-source software, including **BGE-small-en-v1.5** (MIT) for on-device embeddings. See **Settings → About → Open source licenses** in the App and `docs/third-party-licenses.md` in the repository.

---

## Children

The App is not directed at children under 13. We do not knowingly collect personal information from children.

---

## Changes to this policy

We may update this Privacy Policy when the App changes (for example, new local features or Store requirements). The **Last updated** date at the top will change accordingly. Material changes will be reflected in the published policy URL used in the Microsoft Store listing.

**Changes in version 1.0.3:** clarified system tray behavior, global keyboard shortcut handling (including optional double-tap modifier shortcuts), local diagnostic logs, and Pro trial roaming timestamp.

---

## Contact

Questions about this Privacy Policy or the App's data practices:

**Email:** [lqzforlyman@outlook.com](mailto:lqzforlyman@outlook.com)
