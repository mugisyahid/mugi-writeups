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

    ???
    run: /opt/metasploit-framework/bin/msfconsole


- **netcat**

    - //TODO must learn today


- **wireshark**

    - //TODO must learn today
