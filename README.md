# **These are best used in Kali Linux**

## **Reverse Engineering**
  ### To analyze ELF files:
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
    - https://futureboy.us/stegano/decinput.html  (jpeg, wav or au)
    - 0 width chars: https://330k.github.io/misc_tools/unicode_steganography.html
    - twitter spacing: https://holloway.nz/steg/
    
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
    - AudioStego (https://github.com/danielcardeenas/AudioStego)
    - Morse code wav files: https://morsecode.world/international/decoder/audio-decoder-expert.html

  ### File Signatures/Magic Numbers:
    - GIF : 47 49 46 38 39 61 18 01
    - PNG/IHDR : 89 50 4E 47 0D 0A 1a 0A
    
  ##  **Password cracking tools:
    - fcrackzip tool 
      fcrackzip -u -D -p ~/rockyou.txt ~/zipfilename.zip
    - john --wordlist=/usr/share/wordlists/rockyou.txt --format=raw-sha1 crack.txt
      for zip files:
        store the hash in a text file hash.txt
        first extract zip file hash : zip2john zipfile.zip > hash.txt
        then use john to crack: john --wordlist=rockyou.txt hash.txt 
    - stegcracker <file> [<wordlist>]   (used to crack passwords in files that contain hidden data)
    - sudo apt-get install pdfcrack
      pdfcrack -f <file_name> -w <location_of_wordlist_file>

  ## **For hashes**
    - https://hashtoolkit.com/
    - https://www.cmd5.org/
    - hashid - to identify the type of hash
    - www.crackstation.net
    - hashcat: 
      store the hash in a text file hash.txt
      hashcat -m <mode_number> -O hash.txt <wordlist>
      https://hashcat.net/wiki/doku.php?id=example_hashes
    
  ### Gcode simulator : https://nraynaud.github.io/webgcode/
  
  ## **Identify/Decode an unidentified encoding**
    - https://2cyr.com/decode/?lang=en
    - https://www.dcode.fr/cipher-identifier
    - https://gchq.github.io/CyberChef/
  
  
  ## **Barcode Reader/Detector**
  ### - https://products.aspose.app/barcode/recognize#/recognized
  
  ## **WEB forensics**
  ### Wayback machine
    - https://archive.org/web/

  ## **For Web Challenges:**
    - inspect element
    - view page source
    - robots.txt or other directory files (flag.txt)
    - check network (in inspect element) for any reloads/redirects
    - burpsuite
    - curl to send or receive data/payload
    - for sql injection try:
      abc' OR '1'='1'--
    - in URL, try ?cmd=ls -lrt
                  ?cmd=cd ..;ls -lrt
                  ?cmd=cat flag.txt 
    - try editing cookies (admin = True) [in login challenges]
    - to modify headers: use curl 
      ex. curl -H "Host: test.example" http://example.com/
    - try moving back directories using local file inclusion vulnerability
    - explore directories : append the url with /../
    - try checking for files like: /.git
    - to get all directories: wget -m <URL>
    
  ## **OSINT**
    - https://osintframework.com/
    - https://nixintel.info/osint/12-osint-resources-for-e-mail-addresses/
    - https://www.shodan.io/        (search engine for anything)
    - Google Dorking: https://infosecwriteups.com/finding-vulnerable-info-using-google-dorks-ethical-hacking-23f358117ceb
  
  
  ### Useful links and repos:
    - https://www.dcode.fr/cipher-identifier
    - https://gchq.github.io/CyberChef/
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
    - https://wiki.bi0s.in/
    - encoding conversion: https://www.rapidtables.com/
    - hashcat cheatsheet: https://hashcat.net/wiki/doku.php?id=hashcat
                          https://github.com/frizb/Hashcat-Cheatsheet
    - lfi cheat sheet https://book.hacktricks.xyz/pentesting-web/file-inclusion
                      https://highon.coffee/blog/lfi-cheat-sheet/
    - search for vulnerabilities and exploits: https://book.hacktricks.xyz/welcome/readme
