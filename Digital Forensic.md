---
title: Digital Forensic
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:33:20Z
---

What is Digital Forensics?

- Process of collecting, analyzing, and preserving digital evidence for legal or investigative purposes.
- Also called computer forensics, often associated with law enforcement seizing computers.
- Used by security teams during incident investigations (DFIR = Digital Forensics & Incident Response).
- Focuses on Windows and Linux systems with practical tools and scenarios.

Digital Forensics Process

1. Identification

- Find potential evidence sources (devices, data locations, custodians).

3. Preservation

- Protect crime/incident scene and evidence. Document and capture visuals.

5. Collection

- Acquire data by imaging, copying, or extracting from devices.

7. Analysis

- Systematic examination of evidence to find relevant data and draw conclusions.

9. Reporting

- Produce detailed reports that others can replicate using proven methods.

Important Concepts

- Exhibit = digital media seized for investigation.
- Use the scientific method to validate evidence.
- Contemporaneous notes are critical—document actions immediately to ensure reproducibility.
- Chain of custody must be maintained throughout to protect evidence integrity. 

Fundamentals

Introduction to Data Representation

Data can be represented in various formats essential to digital forensics and cybersecurity. This lesson covers:

- Binary
- Base64
- Hexadecimal (Hex)
- Octal
- ASCII

We also look at tools like CyberChef from GCHQ for encoding and decoding data efficiently.

Binary

- The simplest form of data representation, using only 0s and 1s.
- In hardware, 0 = no electric current (OFF), 1 = electric current (ON).
- Binary digits (bits) form the foundation of all digital data.
- 1 bit = single 0 or 1, represents True/False in Boolean logic.
- 1 byte = 8 bits, allowing 256 different values (2^8).
- Large files and applications are just sequences of binary digits.
- Binary is efficient because:

- It’s easy to detect electrical signals.
- Matches physical properties of storage media (magnetic poles).
- Controls digital logic circuits effectively.

Base64

- A reversible encoding method that converts binary data into ASCII text.
- Useful because older systems supported only text (e.g., early email), making it impossible to send images or files directly.
- Base64 converts any data (images, videos, binaries) into a text string, which can be decoded back.
- Forensics use: malicious users may hide media content by encoding it in Base64, making it look like random characters to the untrained eye.

Example string:

VGhpcyBzZW50ZW5jZSBkb2Vzbid0IHJlYWxseSBtZWFuIGEgbG90LiBTb3JyeS4=

Hexadecimal (Hex)

- Base 16 numbering system using digits 0-9 and letters A-F.
- Provides a compact way to represent binary data because 1 hex digit = 4 bits.
- Commonly used in programming and debugging.
- Example: Hex digit ‘A’ corresponds to decimal 10 and binary 1010.

Octal

- Base 8 numbering system.
- Groups binary digits in threes, converting them to single octal digits.
- Example: Binary 10011111 → grouped as (0)10-011-111 → octal 237.
- Used historically to shorten binary numbers (more common in early computing).
- Today, it’s often seen in Linux/Unix for file permission settings (e.g., chmod).

ASCII

- American Standard Code for Information Interchange.
- Maps characters (letters, numbers, punctuation) to 8-bit binary codes.
- Widely used for text files in UNIX and DOS.
- Windows uses Unicode (more extensive).
- Example:

- ‘A’ = decimal 65
- ‘a’ = decimal 97

- ASCII allows computers to exchange readable text data.

Hard Disk Drive (HDD) Basics

Hard drives are primary data storage devices, crucial for forensic evidence.

Platters

- Circular, rigid disks coated with magnetic material.
- Store data magnetically on both sides.
- Multiple platters are stacked on a spindle inside the HDD.

Sectors

- The smallest physical storage unit on a disk.
- Traditionally 512 bytes per sector; modern HDDs use 4096 bytes (4 KiB).
- Each sector includes:

- Header (ID)
- Data area (user data, sync bytes, error-correcting code)

- Files occupy full sectors; leftover space in the last sector is zero-padded.

Clusters

- Groups of sectors that form the minimum allocation unit.
- Clusters make file storage efficient by managing space in groups.
- Each cluster has a unique ID for tracking.

Slack Space

- Leftover space in a cluster when a file doesn’t fill it entirely.
- Can contain remnants of previously deleted files.
- Important in forensics for recovering deleted or hidden data.

Solid State Drive (SSD) Basics

SSDs use flash memory and differ from HDDs in structure and behavior.

Garbage Collection

- SSDs clean up unused pages to maintain free blocks for fast writing.
- Moves valid data to new blocks and erases old blocks.
- Happens in the background automatically.
- Forensics risk: Garbage collection can erase evidence if the system stays powered on.

Trim

- Command telling the SSD which data blocks are no longer in use.
- Allows the SSD to erase data immediately, preventing recovery.
- Forensics risk: TRIM can make deleted data unrecoverable.
- Forensic best practice: Power off SSD systems immediately via hard shutdown or unplug to avoid garbage collection/TRIM operations.

Wear Leveling

- Distributes write/erase cycles evenly across the SSD to prevent premature wear.
- Two types:

- Dynamic: Moves frequently rewritten blocks only.
- Static: Also moves static blocks when needed for better longevity.

- Performed by SSD controller firmware.

File Systems

A file system organizes and manages data storage on devices.

Key Functions

- Controls data storage and retrieval.
- Organizes files and directories hierarchically.
- Manages metadata.
- Enables data recovery and navigation.

Popular File Systems

FAT16

- Early file system for DOS and Windows 3.x.
- Limited to small partitions.
- Data inaccessible if File Allocation Table is corrupted.

FAT32

- Improved version of FAT16.
- Supports larger partitions and long file names.
- Compatible with many devices and OSs (Windows 95+ to Windows 10, macOS, Linux).
- Limitations:

- Max file size < 4 GB.
- Max partition size 8 TB.
- No built-in security or compression.
- Vulnerable to data loss on power failure.

NTFS

- Microsoft’s proprietary journaling file system.
- Default for Windows NT family onward.
- Features:

- Advanced metadata support.
- Security with Access Control Lists (ACLs).
- File system journaling for data integrity.

- Linux supports NTFS via NTFS-3G (read/write).
- macOS supports NTFS read-only by default.

EXT3 and EXT4

- Linux journaling file systems.
- EXT3: Added journaling to predecessor EXT2, improving recovery.
- EXT4: Improved performance with extents (reducing fragmentation), supports huge file and volume sizes (up to exbibytes).
- Linux filesystem architecture:

- User space (applications)
- Kernel space (OS core)
- Disk space (hardware storage)

File System Identification

- Tools like FTK Imager allow investigators to open disk images and identify file systems.
- Important to recognize file systems when collecting digital evidence.

Digital Evidence and Handling

What is Digital Evidence?

- Digital evidence = any probative information stored or transmitted in digital form.
- Similar to trace evidence in physical forensics (like dirt on shoes), digital trace evidence is left when systems interact.
- Example: Visiting a website leaves IP logs on the server and may drop cookies on your device.
- Important caution: Digital evidence can be easily manipulated. Always verify with corroborating evidence before trusting.

Common Forms of Digital Evidence

- Emails: Written communications, often with attachments.
- Digital Photographs: May include metadata (location, device info).
- Logs: System logs (e.g., Windows Event logs showing user login times).
- Files: Notes, code, images, software — user activity context.
- Messages: SMS, iMessage, WhatsApp, Messenger chats.
- Browser History: Websites accessed and timestamps.
- Backups: May contain deleted files, useful for recovery.
- Video/Audio Files: Content plus metadata.

Can We Trust Digital Evidence?

- Digital evidence is:

- Large in volume
- Difficult to destroy completely
- Easily modified or duplicated
- More expressive and available than physical evidence

- Courts may question authenticity due to easy modification, but without proof of tampering, this objection is often rejected.
- Hash values (checksums) are critical to verify evidence integrity.

Evidence Handling Best Practices

1. Do Not Alter Original Evidence

- Avoid accessing running systems unnecessarily.
- If alteration is unavoidable, document it fully with justifications.

3. Use Write-Blockers

- Prevents changes to original media during acquisition.
- Software write blockers operate at OS level (OS-specific).
- Physical write blockers intercept hardware signals, OS-independent.

5. Document Everything

- “If you didn’t write it down, it didn’t happen.”
- Detailed notes, diagrams, and photographs help maintain evidence integrity and chain of custody.

Order of Volatility (OoV)

Volatility indicates how quickly evidence can be lost or changed. Collect evidence in this priority order:

|   |   |   |
|---|---|---|
|Rank|Evidence Type|Notes|
|1|Registers & Cache|Most volatile, changes constantly, collect immediately.|
|2|Memory (RAM)|Lost on power-off, contains running processes & network info.|
|3|Disk Storage (HDD, SSD)|Less volatile once offline. SSDs have risks of Garbage Collection and TRIM.|
|4|Remote Logging & Monitoring|Volatile but less critical than disk data.|
|5|Physical Config, Network Topology, Archival Media|Least volatile, useful for context and archived data.|

Note: Always prioritize capturing volatile data first and move it quickly to non-volatile media (external hard drive).

Metadata and File Carving

What is Metadata?

- Metadata = “data about data.”
- Example: A Word document’s metadata includes author, creation date, last modified date.
- Photos can include camera settings, GPS location, resolution.

Viewing Metadata

- Windows: Right-click file > Properties > Details tab.
- Linux: Use commands ls -lisap <file>, stat <file>.
- ExifTool: A powerful CLI tool for extracting metadata from various file types.

- Install with sudo apt-get install exiftool
- Use: exiftool <filename>

File Carving

- File carving is recovering deleted or hidden files from disk images by searching data patterns.
- Tool: Scalpel

- Configured by editing /etc/scalpel/scalpel.conf to enable file types (e.g., jpg).
- Run with:  
    scalpel -o <output_directory> <disk_image_file>
- Output includes recovered files and audit logs.

- Custom profiles can be created to carve specific file types by defining headers/footers.

Linux Command: chown

Purpose

- Change ownership of files or directories.
- Important for managing access permissions in forensic investigations.

Syntax

bash

CopyEdit

chown [options] new_owner[:new_group] file(s)

Example

- Change owner of q3.conf to user ubuntu:

bash

CopyEdit

chown ubuntu q3.conf

- Verify ownership:

bash

CopyEdit

ls -l q3.conf