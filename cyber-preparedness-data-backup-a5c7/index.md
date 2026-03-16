# Cyber Preparedness & Data Backup

> **Protect Your Digital Life Before the Lights Go Out** - In an emergency, your digital information can be as critical as food and water. Medical records, contacts, maps, insurance documents, and communication tools all live on devices that need power and protection.

## Why Digital Preparedness Matters

Modern life depends on digital systems. When those systems go down -- whether from a power outage, cyberattack, natural disaster, or infrastructure failure -- you lose access to:

- **Financial accounts** (banking, payments)
- **Communication** (phone, email, messaging)
- **Navigation** (GPS, online maps)
- **Medical information** (prescriptions, health records, provider contacts)
- **Identity verification** (digital IDs, account recovery)
- **Essential contacts** (phone numbers you have not memorized)

**The goal:** Have your critical digital information accessible **offline, encrypted, and on devices you can keep charged**.

---

## Backing Up Important Digital Files

### What to Back Up

**Priority 1: Identity and Legal**
- Government-issued ID (scans of driver's license, passport, birth certificates)
- Social Security cards
- Marriage/divorce certificates
- Property deeds and vehicle titles
- Will and power of attorney documents
- Immigration documents

**Priority 2: Financial**
- Bank account numbers and routing numbers
- Insurance policies (health, home, auto, life) with policy numbers and agent contacts
- Credit card numbers and customer service phone numbers
- Tax returns (last 3 years minimum)
- Loan documents

**Priority 3: Medical**
- Prescription list (medication names, dosages, prescribing doctors)
- Medical history summary
- Allergies and blood type
- Health insurance cards
- Vaccination records
- Advance directives and medical power of attorney
- Copies of eyeglass/contact lens prescriptions

**Priority 4: Practical**
- Emergency contact list (printed AND digital)
- Offline maps of your area and evacuation routes
- Family photos (irreplaceable memories)
- Home inventory (for insurance claims)
- Pet records (vaccination, microchip numbers)
- Password database (encrypted)

### The 3-2-1 Backup Rule

- **3** copies of your data
- **2** different storage media types
- **1** copy stored off-site (at a family member's home, in a safe deposit box, or in a secure cloud service)

---

## Encrypted USB Drives

An encrypted USB drive is one of the best ways to keep critical documents portable and secure.

### Hardware-Encrypted vs. Software-Encrypted

| Feature | Hardware-Encrypted | Software-Encrypted |
|---------|-------------------|-------------------|
| **Security** | Encryption chip built into drive | Uses software on host computer |
| **Ease of use** | Enter PIN on drive itself, works on any computer | Requires specific software installed |
| **Cost** | $50-150 | Free (software) + cost of any USB drive |
| **Tamper resistance** | Physical protection against brute force | Depends on software strength |
| **Recommendation** | Best for primary backup | Good for secondary copies |

### Recommended Approach

1. **Get a quality encrypted USB drive** (hardware-encrypted preferred)
2. **Organize files in clear folders:**
   ```
   /EMERGENCY-DOCS/
     /Identity/
     /Financial/
     /Medical/
     /Insurance/
     /Contacts/
     /Maps/
     /References/
   ```
3. **Update quarterly** -- set a calendar reminder
4. **Test regularly** -- plug it in and verify files are readable
5. **Store in your go-bag** or a fireproof/waterproof container
6. **Use a strong PIN** (hardware) or passphrase (software) -- at least 8 characters

### Software Encryption Option (Free)

If using a regular USB drive, encrypt it with **VeraCrypt** (free, open-source):

1. Download and install VeraCrypt on your computer
2. Create an encrypted volume on the USB drive
3. Mount the volume with your password to access files
4. Dismount when done
5. **Important:** You will need VeraCrypt installed on any computer to access the files, or carry the portable version of VeraCrypt on the unencrypted portion of the drive

---

## Offline Password Management

When the internet is down, you cannot access cloud-based password managers. **KeePass** solves this.

### Why KeePass?

- **Fully offline** -- database stored locally, no internet required
- **Free and open-source**
- **Cross-platform** (KeePassXC for desktop, KeePassDX for Android, Strongbox for iOS)
- **Strong encryption** (AES-256)
- **Portable** -- database file can be carried on USB drive

### Setting Up KeePass for Emergencies

1. **Install KeePassXC** on your computer (keepassxc.org)
2. **Create a new database** with a strong master password
3. **Organize entries into groups:**
   - Financial (banking, investments)
   - Insurance
   - Medical portals
   - Email accounts
   - Government services
   - Utilities
   - Social media
4. **For each entry, store:**
   - Username
   - Password
   - URL
   - Recovery codes
   - Security question answers
   - Customer service phone numbers
5. **Copy the database file (.kbdx) to:**
   - Your encrypted USB drive
   - Your phone (using the mobile KeePass app)
   - A secondary backup location
6. **Memorize your master password** -- write nothing down

### Critical Password Security

- Use a **unique, strong master password** (at least 16 characters)
- **Never reuse** your master password anywhere else
- Consider a **key file** in addition to your password for extra security (store the key file separately from the database)
- Update your database whenever you change a password

---

## Protecting Identity Documents Digitally

### Scanning Best Practices

- Scan at **300 DPI minimum** (legible when zoomed)
- Save as **PDF** (universal format)
- Use **color scans** for IDs and important documents
- Name files clearly: `passport-john-smith-2025.pdf`
- Store in encrypted container (never unencrypted on a device)

### Additional Protections

- **Watermark scans** with "COPY - NOT ORIGINAL" to reduce identity theft risk if files are stolen
- **Keep originals** in a fireproof/waterproof safe or safety deposit box
- **Share encrypted copies** with a trusted family member (and give them the password separately, in person)
- **Review and update** scans when documents are renewed

---

## Phone Hardening Basics

Your phone is likely your most important emergency device. Harden it now.

### Essential Settings

- [ ] **Enable full-device encryption** (enabled by default on modern iOS and Android)
- [ ] **Set a strong lock screen** (6+ digit PIN or passphrase, not pattern or 4-digit)
- [ ] **Enable biometrics** (fingerprint/face) for convenience, but know that a PIN/password is legally stronger
- [ ] **Turn off lock screen previews** for sensitive apps (messages, email)
- [ ] **Enable Find My Device** (helps locate or remotely wipe if stolen)
- [ ] **Disable USB debugging** (Android) unless actively needed
- [ ] **Review app permissions** -- revoke access to camera, microphone, location for apps that do not need them
- [ ] **Keep your OS updated** -- security patches fix known vulnerabilities
- [ ] **Install apps from official stores only**

### Emergency-Specific Phone Setup

- [ ] **Download offline maps** (Google Maps, OsmAnd, or Organic Maps all support offline areas)
- [ ] **Save critical contacts** to the device (not just cloud)
- [ ] **Install KeePass mobile app** and sync your password database
- [ ] **Download essential reference apps** that work offline
- [ ] **Set up ICE (In Case of Emergency) contacts** on your lock screen
- [ ] **Take screenshots of insurance cards** and store in a secure folder
- [ ] **Enable battery saver mode** settings so you know how to activate them quickly

---

## Keeping Devices Charged

### Device Prioritization During Power Outages

When power is limited, prioritize charging in this order:

1. **Phone** (communication, maps, flashlight, references)
2. **Emergency radio** (if rechargeable)
3. **Medical devices** (CPAP, glucose monitors, etc.)
4. **Secondary phone or tablet** (backup communication, entertainment for children)
5. **Laptop** (only if needed for specific tasks)

### Extending Battery Life

**Immediate actions when power goes out:**
- Enable **airplane mode** if cell service is down (stops the radio from searching for towers, which drains battery fast)
- Reduce **screen brightness** to minimum usable level
- Turn off **Wi-Fi, Bluetooth, NFC, and location services** if not in use
- Close **background apps**
- Disable **push notifications** and email auto-sync
- Switch to **dark mode** (saves battery on OLED screens)
- Turn the phone **off** when not actively using it

**Expected battery life with conservation:**

| Usage Pattern | Typical Smartphone Battery Life |
|---------------|-------------------------------|
| Normal use | 8-14 hours |
| Light use, screen dim | 24-36 hours |
| Airplane mode, minimal use | 3-5 days |
| Powered off, brief checks only | 7-14 days |

### Charging Options Without Grid Power

- **Portable power bank** (10,000-20,000 mAh provides 2-5 full phone charges)
- **Solar charger** (foldable panel + power bank)
- **Car charger** (12V outlet; run engine briefly to charge, conserve fuel)
- **Hand-crank charger** (slow but reliable, no fuel or sunlight needed)
- **AA battery pack** (USB charger that accepts AA batteries)

---

## Alternative Communication Methods

When cell towers and internet go down, you need other ways to communicate.

### Mesh Networking: Meshtastic

**Meshtastic** is an open-source project that turns inexpensive LoRa radio modules into a mesh communication network.

- **Range:** 1-10+ miles depending on terrain and antenna
- **Cost:** $25-50 per device
- **No cell service or internet required**
- **Encrypted messaging**
- **Mesh capability:** Messages hop through intermediate devices, extending range
- **GPS position sharing** with group members
- **Pairs with your phone** via Bluetooth

**Getting started:**
1. Purchase a compatible LoRa device (Heltec, LILYGO T-Beam, or RAK WisBlock)
2. Flash Meshtastic firmware
3. Install the Meshtastic app on your phone
4. Pair via Bluetooth
5. Share devices with family/neighbors to build your mesh network

### Briar Messaging App

**Briar** is a messaging app designed for emergencies and censorship resistance.

- Works over **Wi-Fi, Bluetooth, and Tor** -- no internet infrastructure needed
- **End-to-end encrypted**
- Can sync messages when two phones are within **Bluetooth range** (approximately 30 feet)
- Also works over **local Wi-Fi** (no internet required, just a router or phone hotspot)
- Available for **Android** (iOS version in development)
- **No phone number or email** required to create an account

### Two-Way Radios

- **FRS radios:** No license required, 1-2 mile range, available at any outdoor store
- **GMRS radios:** Requires FCC license ($35, no exam), 5-25+ mile range with repeaters
- **Ham radio (amateur):** Requires license (exam required), virtually unlimited range capabilities
- **CB radio:** No license required, ~5 mile range, useful for vehicle-to-vehicle

---

## Data You Should Have Offline

Do not rely on being able to access the internet. Download and store these on your phone and encrypted USB drive.

### Essential Offline Data

- [ ] **Contact list** (printed copy AND on device -- do not rely on cloud sync)
- [ ] **Offline maps** of your region, evacuation routes, and bug-out locations
- [ ] **Medical records** (prescriptions, conditions, allergies, doctor contacts)
- [ ] **Insurance documents** (policy numbers, agent phone numbers, coverage details)
- [ ] **First aid reference guide**
- [ ] **Emergency frequency list** (local NOAA, emergency broadcast, ham repeaters)
- [ ] **Copies of ID documents** (encrypted)
- [ ] **Family emergency plan** (meeting points, communication plan, out-of-area contacts)
- [ ] **Local emergency resources** (shelter locations, hospitals, fire stations)
- [ ] **Utility account information** (for reporting outages and filing claims)

### Nice to Have Offline

- [ ] **Survival reference guides** (water purification, first aid, shelter building)
- [ ] **Field guides** (edible plants for your region, if relevant)
- [ ] **Radio programming files** (for ham radio or GMRS)
- [ ] **Entertainment** (ebooks, downloaded music, podcasts -- morale matters)
- [ ] **Educational materials** for children (if applicable)
- [ ] **Repair manuals** for your vehicle and major home systems

---

## Cyber Threats During Emergencies

Emergencies create opportunities for cyber criminals. Stay alert.

### Common Scams After Disasters

- **Phishing emails** posing as FEMA, Red Cross, or insurance companies
- **Fake charity websites** soliciting donations
- **Price-gouging scam sites** for emergency supplies
- **Fake government aid applications** designed to steal personal information
- **SMS scams** with urgent links about disaster relief

### Protection Measures

- **Never click links** in unsolicited emails or texts about disaster aid
- **Go directly to official websites** (fema.gov, redcross.org) by typing the URL
- **Do not share personal information** over the phone with unsolicited callers
- **Verify charity legitimacy** at charitynavigator.org or give.org before donating
- **Use multi-factor authentication** on critical accounts (email, banking)
- **Monitor financial accounts** closely after a disaster (identity theft increases)

---

## Checklist: Cyber Preparedness

### Backup Setup

- [ ] Encrypted USB drive prepared with all critical documents
- [ ] KeePass database created and synced to phone and USB
- [ ] 3-2-1 backup rule implemented
- [ ] Printed copy of essential contacts and account numbers stored with emergency supplies
- [ ] Offline maps downloaded for your region

### Device Preparedness

- [ ] Phone encryption verified
- [ ] Strong lock screen PIN/password set
- [ ] OS and apps updated
- [ ] Offline maps and reference apps installed
- [ ] ICE contacts configured on lock screen
- [ ] At least one portable power bank fully charged
- [ ] Car charger cable in vehicle

### Communication Alternatives

- [ ] At least one non-cell-network communication method available (FRS radio, Meshtastic, Briar)
- [ ] Family communication plan established (meeting points, check-in schedule, out-of-area contact)
- [ ] NOAA weather radio frequencies noted for your area
- [ ] Contact list printed on paper as a backup

### Maintenance Schedule

- [ ] Monthly: Charge power banks and verify charge level
- [ ] Quarterly: Update encrypted USB drive with current documents
- [ ] Quarterly: Update KeePass database with any changed passwords
- [ ] Quarterly: Refresh offline maps
- [ ] Annually: Review and update all backed-up documents
- [ ] Annually: Test all backup devices and verify file integrity
- [ ] Annually: Review and update family emergency communication plan

---

*Last updated: March 2026*
*License: CC-BY-SA 4.0*
