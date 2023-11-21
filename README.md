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
    - stegsnow -C -p '1234' newdos.txt
    
  ### For images:
    - strings filename | grep (stringtosearch)
    - steghide --extract -sf <filename>
    - zsteg -a <filename.png>
    - https://www.aperisolve.com/ (all in one steg tool)
    - https://lukeslytalker.pythonanywhere.com/deepscan
    - pngcheck
    - sudo apt install ruby
      sudo gem install zsteg
      zsteg <filename>
      (detect LSB steganography only in the case of PNG and BMP images.)

  ### For audio files:
    - audacity <file_name>
    - sonic-visualiser <file_name>
    
  ### Password cracking tools:
    - fcrackzip tool 
      fcrackzip -u -D -p ~/rockyou.txt ~/zipfilename.zip
    - john --wordlist=/usr/share/wordlists/rockyou.txt --format=raw-sha1 crack.txt
    - stegcracker <file> [<wordlist>]   (used to crack passwords in files which contains hidden data)
    - sudo apt-get install pdfcrack
      pdfcrack -f <file_name> -w <location_of_wordlist_file>
    

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
    - https://www.hackingarticles.in/online-message-decoder-spam-maker/
    - https://330k.github.io/misc_tools/unicode_steganography.html
    - https://www.shodan.io/        (search engine for anything)
