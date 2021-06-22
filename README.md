# tools-set-up
      
      everything about the tools i use , from where to get them to ow to start using them.
# TOOLS

      1. VM - oracle vm && OS - inside VM - kali  
      2. VPN - proton vpn
      3. STORAGE - github
      4. BURP suite - on kali
      5. chrome extensions
      
# 1. VM - oracle vm  &&&&  OS - inside VM - kali
     
      
      Source - https://www.youtube.com/watch?v=wX75Z-4MEoM
# 2. VPN - proton vpn
      
      Source - official website
      
      https://protonvpn.com/download
 
      unable to install on KALI - so instead installed on WINDOWS (my host machine)
# 3. STORAGE - github

     No description needed - documenting everything - my whole learning journey
     
# 4. BURP suite - on kali
    
     Source - https://www.youtube.com/watch?v=4Egz-LkVlnI
     
     ** FREE PRO VERSION.
     
     IF video not found - try to find this - 
       https://medium.com/@sherlock297/install-burp-suite-pro-on-kali-linux-6abccc3860a8
       
       
    else 
       Steps to install Burp Suite Pro cracked on Kali Linux:
       Steps to install Burp Suite Pro cracked on Kali Linux:
       Note : We have used zshrc for setup, if you received any error related to zshrc then you can try using bashrc. For this you have          to replace zshrc with bashrc
       Download : https://drive.google.com/drive/folders/1HOQJTsjLL2hqGB-VMBxL5vvdInKesT8y
       Download Java 8 : https://adoptopenjdk.net/releases.html?variant=openjdk8&jvmVariant=hotspot
       Open Downloads folder
       Open terminal in Downloads folder
       Run : sudo su
       Extract Java Archive file : tar -C /usr/lib/jvm -xzf OpenJDK8U-jdk_x64_linux_hotspot_8u292b10.tar.gz
       Close Terminal
       Extract Burp Archive file on Desktop
       Open terminal in the same folder that is in Desktop
      Run : sudo su
      Run : java -jar burp-loader-keygen.jar
      Open new terminal in the same folder that is in Desktop
      Run : /usr/lib/jvm/jdk8u292-b10/bin/java -Xbootclasspath/p:burp-loader-keygen.jar -jar burpsuite_pro_v1.7.37.jar
      Wait till burp loads and show the Enter License Key Screen
      Now copy License from file burp-loader-keygen
      Paste it in Burp Suite.
      Click on Next
      Click on Manual Activation
      Copy : Activation Request from Burp Suite that is copy request
      Past it into burp-loader-keygen file
      You’ll receive Activation Response
      Copy Activation Response from burp-loader-keygen file and paste it in Burp Suite.
      Click on Next and then Finish.
      Now go to terminal
      Run : nano ~/.zshrc
      Scroll to the bottom of the file
      Add : alias burpro=”/usr/lib/jvm/jdk8u292-b10/bin/java -Xbootclasspath/p:/home/kali/Desktop/Burp\ Suite\ Pro/burp-loader-keygen.jar-jar /home/kali/Desktop/Burp\ Suite\ Pro/burpsuite_pro_v1.7.37.jar”
      Note : Above path may be different for you. Please check and change it accordingly.
      Save file : CTRL+O and Press Enter
      Exit File : CTRL+X
      Run : source ~/.zshrc
      Close All terminals and Open new Terminal
      Run : burpro
      Thank You..!!!
      More Info : https://portswigger.net/burp/pro
      
# 5. chrome extensions
     
     
     
     
     
     
# 6. PROXY SETUP

     A)  OPEN - BURPSUITE & FIREFOX
     B)   ON BURP - GO TO PROXY TAB 
                             THEN OPTIONS TAB 
                                       LOOK IN PROXY LISTNERS TAB - by default burp listens to  127.0.0.1 : 8080
                                                                  - 127.0.0.1 => IP && 8080 => PORT
     C)   by default - FIRE FOX USES PORTS - 80 & 443 (standard)
                     - TO CHANGE THIS AND USE THE BURP SUITE ip AND port
                              - GO TO FIRE FOX - CLICK ON THE THREE LINES ON RIGHT 
                                               - GO TO PREFERENCES
                                               - GENERAL SETTINGS - GO TO BOTTOM - LOOK FOR NETWORK SETTINGS 
                                                                                 - CLICK ON SETTINGS 
                                                                                 - THEN MANUAL PROXY CONFIG - THE USE THE BURP SUITE IP AND PORT
                                                                                 - USE THIS FOR ALL PROTOCOLS (CLICK IT)
                                                                                 - SAVE AND CLOSE
                                                                                 - REFRESH TYHE PAGE TO TEST
                                                                                 - BUT IT THROWS AN ERROR
    D)  NOW OPEN BURP SUITE - PROXY - INTERCEPT - IN INTERCEPT TAB NOTICE THAT intercept is on by default
                                                - TURN IT OF TO DIRECTLY SEND THE PACKETS TO FIREFOX 
    
