# **These are best used in Kali Linux**

## **Reverse Engineering**
  ### To ananlyse ELF files:
    - https://elfy.io/
  ### To dissamble ELF:
    - https://onlinedisassembler.com/odaweb/

## **For steganography and Forensics:**

  ### For general files:
    - exiftool (filename)
    - binwalk -e (filename)
    - file (filename)
    - foremost -v filename
    - cat filename ----{to read executables}
  ### For images:
    - strings filename | grep (stringtosearch)
    - steghide --extract -sf <filename>
    - zsteg -a <filename.png>
    - https://www.aperisolve.com/ (all in one steg tool)
    
  ### Useful links:
    - https://fareedfauzi.gitbook.io/ctf-checklist-for-beginner/steganography
    - https://infosecwriteups.com/beginners-ctf-guide-finding-hidden-data-in-images-e3be9e34ae0d

  ### Gcode simulator : https://nraynaud.github.io/webgcode/
  
  
  ## **For hashes**
  
  ### - https://hashtoolkit.com/
  
  ## **Decode an unidentified encoding**
  ### - https://2cyr.com/decode/?lang=en
