# **These are best used in Kali Linux**

## **For steganography:**

  ### For general files:
    - exiftool (filename)
    - binwalk -e (filename)
    - file (filename)
    - foremost -v filename
  ### For images:
    - strings filename | grep (stringtosearch)
    - steghide --extract -sf <filename>
    - zsteg -a <filename.png>
    
  ### Useful links:
    - https://fareedfauzi.gitbook.io/ctf-checklist-for-beginner/steganography
    - https://infosecwriteups.com/beginners-ctf-guide-finding-hidden-data-in-images-e3be9e34ae0d

  ### Gcode simulator : https://nraynaud.github.io/webgcode/
