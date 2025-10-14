# Digital Forensics – File Recovery & Investigation

# Objective
Investigate and recover deleted or hidden files from a digital image using forensic tools to understand data recovery, validation, and evidence documentation procedures.

# Tools Used
- **Autopsy** – GUI-based forensic platform for analyzing and recovering data from disk images.  
- **OSForensics** – Used to compare results and validate data recovery.  
- **WinHex** – For low-level disk and hex inspection.  
- **Kali Linux (VirtualBox)** – Environment for running Autopsy and forensic utilities.

# Steps Performed
1. Downloaded and installed Autopsy and OSForensics on Kali Linux via VirtualBox.  
2. Loaded the evidence image file (`charlie-2009-12-07.E01`) into both Autopsy and OSForensics.  
3. Created a new forensic case in Autopsy, configured case number and examiner details.  
4. Performed keyword searches (`project2400`, `craigslist`) to identify relevant files.  
5. Recovered and tagged deleted or hidden files for analysis and reporting.  
6. Used **WinHex** to manually inspect file headers and confirm partial recoveries.  
7. Generated HTML reports from both tools and compared findings for consistency.  
8. Validated results using hashing to ensure data integrity.

# Key Observations
- Autopsy successfully indexed and identified deleted files from the evidence image.  
- Some files found in Autopsy were not detected by OSForensics due to index errors.  
- Hex-level inspection using WinHex verified the file headers and metadata consistency.  
- Timestamp analysis showed deletion events related to user activity sessions.  
- Validation via hashing (MD5) confirmed data integrity of recovered files.

# What I Learned
- Fundamentals of **digital evidence handling and file recovery**.  
- How to cross-check results between multiple forensic tools.  
- Use of **hashing (MD5/SHA)** to ensure evidence integrity.  
- How deleted files can still leave forensic traces within image sectors.  
- The importance of chain of custody and structured documentation.

# Screenshots
- Evidence image loaded in Autopsy  
- Keyword search & recovered file list  
- Hex data view in WinHex  
- HTML report comparison results  

---
examine the file
<img width="1013" height="744" alt="image" src="https://github.com/user-attachments/assets/9cb9b689-6d67-4b2c-b7f1-92a7d9148b89" />
<img width="1013" height="1271" alt="image" src="https://github.com/user-attachments/assets/1f7ee583-ee0d-43a7-9478-2bbbfe911284" />
<img width="1013" height="1280" alt="image" src="https://github.com/user-attachments/assets/a2a9daed-6358-42a4-bb70-c7da877fee59" />
<img width="1013" height="1280" alt="image" src="https://github.com/user-attachments/assets/4ada446f-f127-48a1-aede-bb22d72bb3c3" />

create new case
<img width="1013" height="680" alt="image" src="https://github.com/user-attachments/assets/688ba3bf-9d92-4d45-8100-240c2fc97713" />
<img width="1013" height="1193" alt="image" src="https://github.com/user-attachments/assets/4dac06be-088b-4b8f-b0e4-b6510cf57eb9" />
<img width="1013" height="1280" alt="image" src="https://github.com/user-attachments/assets/6fc8a46a-2d30-46d2-bb19-6c265b1f0a9a" />
<img width="1013" height="383" alt="image" src="https://github.com/user-attachments/assets/5a64b29d-108d-47ed-8764-96d239c73ea3" />
<img width="1013" height="878" alt="image" src="https://github.com/user-attachments/assets/707661fd-1938-4eea-a6d5-c2c568c561ae" />
<img width="1013" height="878" alt="image" src="https://github.com/user-attachments/assets/2b872e1a-ca7e-4172-ba8b-44682c52ecf6" />
<img width="1013" height="878" alt="image" src="https://github.com/user-attachments/assets/eb69ee72-85d3-4c90-bfca-fd994aa52bc4" />
<img width="1013" height="878" alt="image" src="https://github.com/user-attachments/assets/d0f4148f-0f1c-4fd1-b2ac-9fc09b8d1a8d" />
<img width="1013" height="878" alt="image" src="https://github.com/user-attachments/assets/6ab91dee-d48a-48da-bd0f-bca748d3bc03" />
<img width="1013" height="878" alt="image" src="https://github.com/user-attachments/assets/ccf30059-e517-4426-bfb3-5215b33f29e1" />

locate and extract JPEG with altered extention
<img width="1362" height="860" alt="image" src="https://github.com/user-attachments/assets/f69ae9c7-5593-4233-9fca-18377f7e0f6c" />
<img width="1424" height="899" alt="image" src="https://github.com/user-attachments/assets/d208747e-3a47-4694-b775-bbb86bbe6a00" />
<img width="1378" height="870" alt="image" src="https://github.com/user-attachments/assets/35737b30-998b-4f6c-859c-1fc5cee166ff" />

recover files
<img width="707" height="893" alt="image" src="https://github.com/user-attachments/assets/e46f84da-7ba2-4cc6-8b54-752351c8d560" />
<img width="610" height="771" alt="image" src="https://github.com/user-attachments/assets/32be5f57-dd87-4a97-8a9c-29d0dd89bead" />

bit shifting
<img width="1306" height="825" alt="image" src="https://github.com/user-attachments/assets/29868aa3-fadf-4678-a99f-66bbc6457c79" />
<img width="878" height="469" alt="image" src="https://github.com/user-attachments/assets/79e1d297-a41d-4c09-adb0-ab3a2bfa1268" />
<img width="876" height="891" alt="image" src="https://github.com/user-attachments/assets/15c0109e-ea73-4bd1-8b82-309df73cd514" />
<img width="705" height="891" alt="image" src="https://github.com/user-attachments/assets/aa4fa841-80e5-4940-9122-a910541c2b98" />
<img width="876" height="891" alt="image" src="https://github.com/user-attachments/assets/3990ece6-fef3-4326-a29d-67cb96b4aca4" />
<img width="1306" height="139" alt="image" src="https://github.com/user-attachments/assets/e1d11941-76ab-4fb2-a754-6308e278ede1" />
<img width="681" height="420" alt="image" src="https://github.com/user-attachments/assets/cf814138-27ad-466a-acf2-294d48f06e86" />
<img width="1306" height="375" alt="image" src="https://github.com/user-attachments/assets/72a165e3-0885-4276-a072-57e9331aa0d7" />
<img width="1306" height="375" alt="image" src="https://github.com/user-attachments/assets/7eab7295-b447-4b18-9f8e-d8a615a96db1" />
<img width="1306" height="375" alt="image" src="https://github.com/user-attachments/assets/3babfe31-6d77-4334-bea2-d083283bcac2" />
<img width="903" height="375" alt="image" src="https://github.com/user-attachments/assets/bde61975-c5fc-4a74-be1c-0318c287f061" />

