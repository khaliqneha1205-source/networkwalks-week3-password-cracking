# NetworkWalks Academy — Week 3: PDF Password Cracking Lab (Modules 1 & 2)

## Overview
This repository documents the completion of the **Week 3 Essential Project Modules** (`W3-PM1` and `W3-PM2`) for the NetworkWalks Cybersecurity & Ethical Hacking curriculum. Both labs focus on password-protected PDF security—extracting password hashes, running cracking attacks to recover plaintext passwords, and verifying document access—alongside key concepts such as one-way hashing versus two-way encryption.

* **Environment:** Kali Linux (Virtualized Sandbox)
* **Tools Used:** John the Ripper (`john`), `pdf2john`, NetworkWalks Hash Calculator (`https://networkwalks.com/hash-calculator/`), NetworkWalks Password Cracker (`https://networkwalks.com/password-cracker/`)

---

## Module 1 (`W3-PM1`): Password Cracking with John the Ripper (JTR)

### Target File
* `My Locked PDF1.pdf`

### Steps Performed
1. **Hash Extraction:**
   Moved `My Locked PDF1.pdf` into the working directory and extracted its `$pdf$` hash into `hash1.txt` using `pdf2john`:
   ```bash
   pdf2john "My Locked PDF1.pdf" > hash1.txt
