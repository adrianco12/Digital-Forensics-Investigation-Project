# Digital Forensics Semester Project Overview

## 🕵️ Project Summary
This team-based digital forensics project reinforced practical forensic techniques in a controlled Windows 10 environment. The project consisted of planting and obfuscating evidence on one system and investigating another team’s system to locate and attribute digital artifacts.

## Project Phases

## 🛠️ Phase 1 – Evidence Planting
- Installed Windows 10 and created multiple user accounts with progressively complex passwords.  
- Planted 10–20 pieces of evidence (Bible verses) using obfuscation techniques including:
  - File deletion  
  - Hidden files  
  - Altered file extensions  
  - Word macros  
  - Steganography  
  - Alternate data streams  
  - Unallocated disk space  
  - Password-protected Office documents  
- Documented evidence with timestamps, metadata, potential attribution, and hash values (MD5/SHA1).

### Timeline of Activities

### Table of Contents
- [February 11, 2026 – Initial Obfuscation Methods](Initial-Obfuscation-Methods.pdf)
- [February 23, 2026 – Alternate Data Streams](Alternate-Data-Streams.pdf)
- [February 27, 2026 – Passwords, File Extensions, and Deletions](Passwords-Extensions-Deletions.pdf)
- [March 18, 2026 – Additional Obfuscation Methods](Additional-Obfuscation-Methods.pdf)

---

#### February 11, 2026 – Initial Obfuscation Methods

**User #1 (DF)**  
- **System Time:** 4:17 PM  
- **Actual Time:** 2:17 PM  
- **Evidence Planted:** Bible verse hidden in an image shortcut with a changed icon (file obfuscation using Paint)

**User #2 (Landon Morrical)**  
- **System Time:** 4:30 PM  
- **Actual Time:** 2:30 PM  
- **Evidence Planted:** Bible verse embedded in an image via hex editing (steganography), stored in Photos folder  

**User #3 (Adrian)**  
- **System Time:** 4:43 PM  
- **Actual Time:** 2:43 PM  
- **Evidence Planted:** Text file containing a Bible verse, then logically deleted (removed from folder and recycle bin)  

---

#### February 23, 2026 – Alternate Data Streams

**User #1 (DF)**  
- **System Time:** 4:55 PM  
- **Actual Time:** 2:55 PM  
- **Evidence Planted:** Hidden data stream containing a Bible verse embedded in a desktop image (ADS)  

**User #2 (Landon Morrical)**  
- **System Time:** 4:23 PM  
- **Actual Time:** 2:23 PM  
- **Evidence Planted:** Bible verse stored in an Alternate Data Stream attached to a Microsoft Edge shortcut (plaintext via echo command)  

**User #3 (Adrian)**  
- **System Time:** 4:44 PM  
- **Actual Time:** 2:44 PM  
- **Evidence Planted:** Image of a Bible verse (VerseEvidence.png) hidden inside a text file using binary ADS  

---

#### February 27, 2026 – Passwords, File Extensions, Deletions

**User #1 (DF)**  
- **System Time:** 4:45 PM  
- **Actual Time:** 2:45 PM  
- **Evidence Planted:**  
  - Password-protected Microsoft Office document  
  - 2 additional evidence files  

**User #2 (Landon Morrical)**  

*Document Evidence*  
- **System Time:** 4:19 PM  
- **Actual Time:** 2:19 PM  
- **Evidence Planted:** Bible verse inside password-protected Word document (Verse.docx, numeric password)  

*Image File Evidence*  
- **System Time:** 4:32 PM  
- **Actual Time:** 2:32 PM  
- **Evidence Planted:** Bitmap image containing hidden data, renamed to installer.exe (file extension spoofing)  

*Deleted File Evidence*  
- **System Time:** 4:34 PM  
- **Actual Time:** 2:34 PM  
- **Evidence Planted:** Plaintext Bible verse in Evidence.txt, then deleted  

**User #3 (Adrian)**  
- **System Time:** 2:36 PM  
- **Actual Time:** 12:36 PM  
- **Evidence Planted:**  
  - Password-protected Word document (verseevidence.docx) containing a Bible verse  
  - index.html file containing evidence  
  - memorydump.dmp file containing evidence  

---

#### March 18, 2026 – Additional Obfuscation Methods

**User #1 (DF)**  
- **System Time:** 4:38 PM  
- **Actual Time:** 2:38 PM  
- **Evidence Planted:** Hidden folder (blank name, custom icon) in `C:\Users\Public\Libraries` containing a text file with a Bible verse  

**User #2 (Landon Morrical)**  
- **System Time:** 4:25 PM  
- **Actual Time:** 2:25 PM  
- **Evidence Planted:** Bible verse stored in Firefox search history; Firefox browser deleted after use  

**User #3 (Adrian)**  
- **System Time:** 4:16 PM  
- **Actual Time:** 2:16 PM  
- **Evidence Planted:** sneakyverse.txt (Bible verse) hidden in `C:\Windows\System32\Drivers` with system, hidden, and read-only attributes enabled  

---

## 🔍 Phase 2 – Forensic Analysis
- Received a system with evidence planted by another team.  
- Removed the hard drive and created a forensic disk image, validating integrity with MD5 and SHA1 hashes.  
- Analyzed artifacts including:
  - Files containing evidence  
  - Browser history and cookies  
  - Application prefetch files  
- Attributed evidence to user accounts based on metadata, file location, and system activity.  
- Maintained detailed chain-of-custody documentation and produced formal forensic reports.

## Skills & Techniques Applied
- Digital evidence planting and obfuscation  
- Disk imaging and hash verification (MD5, SHA1)  
- File system and artifact analysis  
- User activity reconstruction and evidence attribution  
- Forensic reporting and chain-of-custody management
