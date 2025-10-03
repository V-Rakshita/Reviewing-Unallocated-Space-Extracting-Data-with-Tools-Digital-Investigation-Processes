# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:

Create a VHD file.

<img width="628" height="116" alt="image" src="https://github.com/user-attachments/assets/a90d463e-83c3-48b2-8d49-aafdf33aa068" />

Assign a drive letter to it.

<img width="397" height="116" alt="image" src="https://github.com/user-attachments/assets/8ff0d868-fac3-4f28-851a-8d8ca22a9ab4" />

Add some files inside that drive and delete some.

<img width="491" height="190" alt="image" src="https://github.com/user-attachments/assets/56f54bde-39ba-4a04-a33a-7bf4fecac69c" />

Then detach the VHD

<img width="551" height="142" alt="image" src="https://github.com/user-attachments/assets/30ad242b-2d0d-42f1-8843-047e44dc6565" />


<img width="434" height="167" alt="image" src="https://github.com/user-attachments/assets/77bd5506-5167-4062-8470-43dc2d1df16d" />

Perform the following commands in sleuth kit tool

<img width="434" height="167" alt="image" src="https://github.com/user-attachments/assets/aa20e0c6-4df0-4124-98ed-ceeff0a3c626" />

<img width="614" height="123" alt="image" src="https://github.com/user-attachments/assets/e6224fa6-b858-429f-b837-86fd52f6718f" />

<img width="628" height="30" alt="image" src="https://github.com/user-attachments/assets/66d1bc57-275d-4174-8fae-d6ce07642777" />

<img width="269" height="41" alt="image" src="https://github.com/user-attachments/assets/b60fdeb5-7290-4b10-8830-375b407071c7" />

<img width="628" height="707" alt="image" src="https://github.com/user-attachments/assets/361bbe50-d2b5-47fe-b3ab-afd23179a89d" />

<img width="628" height="429" alt="image" src="https://github.com/user-attachments/assets/bcbe4c2c-71df-4e52-82df-da548b11146c" />

<img width="628" height="25" alt="image" src="https://github.com/user-attachments/assets/0b686c60-d4c5-40c7-8758-b8ef056cf84a" />

<img width="628" height="74" alt="image" src="https://github.com/user-attachments/assets/1e96028b-5017-4e1d-8453-ad4ecc0e2618" />

<img width="628" height="353" alt="image" src="https://github.com/user-attachments/assets/9b4479f4-10a0-4ea6-8f0b-8636d745c6bf" />














## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

