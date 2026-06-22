# Privacy Policy — LocalSeek Semantic

**Last updated:** June 10, 2026  

**Publisher:** Phoenix X ("we", "us").

This Privacy Policy describes how **LocalSeek Semantic** (the "App") handles information when you install and use the App distributed through the **Microsoft Store**.

---

## Summary

LocalSeek Semantic is a **local desktop search utility**. Your documents are indexed and searched **on your device**. We do not collect, store, or transmit your file contents to Phoenix X.

The **embedding model** (BGE-small-en-v1.5) is **bundled with the app**. No model download from our servers is required for normal use.

**License, trial, and purchase** flows are handled by **Microsoft** through the Microsoft Store.

---

## Information processed on your device

- **Folders you select** for indexing (via Folder Picker — not full-disk access by default).
- **File metadata** (name, path, size, dates) for Free search.
- **Document text chunks and embeddings** (Pro) stored locally under `%LocalAppData%\...\LocalSeekSemantic\`.
- **In-app preferences** (watched folders, custom file types, license state cache).

This data is **not sent to Phoenix X** during normal operation.

---

## Network use

| Activity | When | Data sent |
|----------|------|-----------|
| Microsoft Store IAP | Purchase / trial | Microsoft account (Microsoft's policy) |

No third-party analytics or advertising SDKs are included.

---

## Microsoft Store

Please review:

- [Microsoft Privacy Statement](https://privacy.microsoft.com/en-us/privacystatement)
- [Microsoft Store Terms](https://www.microsoft.com/en-us/store/b/terms-of-sale)

---

## Data retention and deletion

Use **Settings → Clear all local data** to remove indexes. Uninstalling the App removes the MSIX package; app data under `%LocalAppData%\...\LocalSeekSemantic\` may remain until you delete it or use in-app clear.

---

## Open-source models

LocalSeek Semantic includes **BGE-small-en-v1.5** (MIT). See `docs/third-party-licenses.md` in the repository and **Settings → About** in the App.
