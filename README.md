# 🔐 OInteg

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OForensics%20%2F%20File%20Integrity-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **OInteg** is a fast and reliable file integrity verifier. It computes MD5, SHA1, SHA256, and SHA512 hashes, verifies files against known values, compares two files, performs batch hashing of directories, and exports clean reports.

---

## 📌 Overview

OInteg helps forensic examiners, system administrators, and security teams verify that files have not been tampered with. It supports single-file hashing, hash verification, file comparison, and full directory batch processing.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Hash File**           | Compute MD5 / SHA1 / SHA256 / SHA512 for a single file |
| **[2]** | **Verify Hash**         | Compare file hash against a known value |
| **[3]** | **Compare Two Files**   | Check if two files are bit-for-bit identical |
| **[4]** | **Batch Hash Directory**| Hash all files in a directory (with optional extension filter) |
| **[5]** | **Quick Hash**          | Fast single-algorithm hash with minimal output |

---

## 📊 Key Features

- **Multiple Hash Algorithms** — MD5, SHA1, SHA256 (recommended), SHA512
- **Automatic Algorithm Detection** — When verifying, detects type by hash length
- **Progress Bar** — Visual feedback during hashing of large files
- **Batch Processing** — Recursive directory scanning with extension filtering
- **File Comparison** — Quick SHA256 comparison between any two files
- **Clean Reports** — Timestamped TXT reports saved to `ointeg_reports/`
- **Standalone** — No external dependencies (pure standard library)

---

## ⚙️ Requirements

- **Linux or Windows**
- **No additional dependencies** — uses only Python standard library

---

## 🚀 Usage

```bash
./OInteg

📁 Output

Live Results — Color-coded hashes with progress bars
Verification Status — Clear MATCH / MISMATCH messages
Batch Summary — List of files with SHA256 and sizes
TXT Reports — Saved automatically in ointeg_reports/ with full details


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED FILE INTEGRITY VERIFICATION AND FORENSIC USE ONLY
