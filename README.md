# nmap
+ ultimate version!


# Learn for use:

```
import nmap3
nmap = nmap3.Nmap()
results = nmap.scan_top_ports("target.com")
```
+ show results with json!

```
[
    {
        "address": "host.com",
        "hostname": "193.189.40.23"
    },
    {
        "address": "domain.com",
        "hostname": "127.0.0.1"
    }
]

```
# Show data with data type list and dict

* run script for system information in nmap3 lib

```
import nmap3
nmap = nmap3.Nmap()
os_results = nmap.nmap_os_detection("127.0.0.1")
```

+ data response:
+      show with json

```
[
    {
        "cpe": [
            {
                "cpe": "cpe:/o:linux:linux_kernel"
            }
        ],
        "port": "80",
        "protocol": "tcp",
        "service": {
            "conf": "10",
            "extrainfo": "Ubuntu",
            "method": "probed",
            "name": "http",
            "ostype": "Linux",
            "product": "nginx",
            "version": "1.14.0"
        }
    },
    {
        "cpe": [
            {
                "cpe": "cpe:/o:linux:linux_kernel"
            }
        ],
        "port": "443",
        "protocol": "tcp",
        "service": {
            "conf": "10",
            "extrainfo": "Ubuntu",
            "method": "probed",
            "name": "http",
            "ostype": "Linux",
            "product": "nginx",
            "tunnel": "ssl",
            "version": "1.14.0"
        }
    },
    {
        "cpe": [
            {
                "cpe": "cpe:/o:linux:linux_kernel"
            }
        ],
        "port": "2000",
        "protocol": "tcp",
        "service": {
            "conf": "10",
            "extrainfo": "Ubuntu Linux; protocol 2.0",
            "method": "probed",
            "name": "ssh",
            "ostype": "Linux",
            "product": "OpenSSH",
            "version": "7.6p1 Ubuntu 4ubuntu0.3"
        }
    }
]
```
# Real command nmap for use!

```
nmap -p http -sS -O 127.0.0.1 ;
```
# other script list in directory:

```
ls /usr/share/nmap/scripts
```

<img href="https://github.com/drcayber/nmap/blob/main/fonts/git.png">


- How to use script NSE?
+   ```
    nmap --script=SCRIPTNAME -p 80 127.0.0.1
    ```
    
