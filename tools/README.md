# Tools

## Scanner

Scanner of port, services, version of target server

- **nmap**

    - -sV, finding version of open port apps
    - -sC, default script attack
    - -p<target_ports>, scanning specific port. -p- for all port scan
    - -oN, write scan result to output file
    - -T<0-5>, fast scan?

- [**rustscan**](https://github.com/RustScan/RustScan)

## Scanner dir

Scanner of directory and hidden API of target webserver

- **dirbuster**

- **gobuster**

    options:

    - -o, output to file
    - -w, wordlist

## SQL Injection

- **sqlmap**
    
    options:
    - --file-read=<target_file>, download file of web server to local?
    - -tables, scanning tables
    - -T <table_name> --dump, dumping tables



## Cracker

- **John The Ripper**

    - john. brute force hash cracker using wordlists.
    - ssh2john. find passphrase of ssh key. 

- **zipcracker**

    zipcracker using wordlists.

## Proxy

- **Burp Suite**

    Browser Proxy to intercept and modify the request and etc. 

    - repeater: repeat http request using different value of given url param or payload.

- **OWAPS**
    - all in scanner?


- **metasploit**

    - all in one exploit 
    - run: /opt/metasploit-framework/bin/msfconsole
    - meterpreter, pwncat-like console
        - migrate?
    - exploit based on module, there are exploit, post, aux, encoder, etc module


- **netcat**

    - TCP / UDP connection & listener, see man page for simple reverse shell
    - `-l`, listening
    - `-n`, Do not do any DNS or service lookups on any specified addresses, hostnames or ports.
    - `-p`, specified port
    - `-v`, verbose output 



- **wireshark**

    - //TODO must learn today


## WEB

- **https://hookbin.com/**, web to test api 

- **https://gchq.github.io/CyberChef/**, The Cyber Swiss Army Knife - a web app for encryption, encoding, compression and data analysis

- **https://crackstation.net/**, online cracking hash tools

## CTF tools

- [pwncat](https://github.com/cytopia/pwncat)
- [pwntools](https://github.com/Gallopsled/pwntools)

## ?bruteforce tools

- **[hydra]()**
    - Example:  hydra -l user -P passlist.txt ftp://192.168.0.1


## Windows Pentest Tools

- **[enum4linux](https://github.com/CiscoCXSecurity/enum4linux)**, A Linux alternative to enum.exe for enumerating data from Windows and Samba hosts.
    - -a $IP | tee out.log 