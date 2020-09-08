# Protocols


## Summary
| Name      | Syntax      | Description |
| :-----------: | :-----------: | :-----------:   |
| ssh      | ssh://      | secure shell       |
| http/s      | http/s://   | web request?        |
| ftp      | ftp://   | file transfer        |
| sftp      | sftp://   | SSH file transfer        |
| smb      | smb://   | windows file transfer        |

## Details & Usefuls Flag

- **ssh**

    Secure shell with default port 22. remote command line, etc.
    
    options:
    - -i <id_rsa>, using specified id_rsa file to connect the server. default id_rsa is .ssh/id_rsa.pub 
    - -p, specify the port
- **http/s**

    Communication protocol over computer network
    
    notable HTTP request to inspect:
    - GET
    - POST
    - HEAD

- **ftp**

    File transfer protocol using port 21 as default


- **sftp**

    File transfer protocol using SSH

- **smb**

    Server Message Block. Windows file transfer protocol