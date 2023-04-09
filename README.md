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
    - https://lukeslytalker.pythonanywhere.com/deepscan
    
  ### Dictionary attack on zip files:
    - fcrackzip tool 
      fcrackzip -u -D -p ~/rockyou.txt ~/zipfilename.zip
    

  ### Gcode simulator : https://nraynaud.github.io/webgcode/
  
  
  ## **For hashes**
  
  ### - https://hashtoolkit.com/
  ### - https://www.cmd5.org/
  
  ## **Decode an unidentified encoding**
  ### - https://2cyr.com/decode/?lang=en
  
  ## **Barcode Reader/Detector**
  ### - https://products.aspose.app/barcode/recognize#/recognized
  
  ## **WEB forensics**
  ### Wayback machine
    - https://archive.org/web/
    
  ## **OSINT**
  ### - https://osintframework.com/
  ### - https://nixintel.info/osint/12-osint-resources-for-e-mail-addresses/
  ### Googel Dorking: https://infosecwriteups.com/finding-vulnerable-info-using-google-dorks-ethical-hacking-23f358117ceb
  
  
  ### Useful links and repos:
    - https://fareedfauzi.gitbook.io/ctf-checklist-for-beginner/steganography
    - https://infosecwriteups.com/beginners-ctf-guide-finding-hidden-data-in-images-e3be9e34ae0d
    - https://0xrick.github.io/lists/stego/
    - https://d00mfist.gitbooks.io/ctf/content/forensics/data-extraction.html
    - https://futureboy.us/stegano/decinput.html
    - https://www.dcode.fr/png-chunks
    - https://github.com/R0B1NL1N/PayloadsAllTheThings
    - https://shankaraman.wordpress.com/tag/how-to-extract-ftp-files-from-wireshark-packet/#:~:text=Just%20open%20the%20packet%20in,the%20files%20in%20a%20Directory.&text=Firstly%2C%20the%20Client%20(10.10.,request%20to%20the%20Server%20(78.47.
    - ophcrack
    - https://www.yeahhub.com/the-12-best-must-have-tools-for-steganography-updated-tools/
