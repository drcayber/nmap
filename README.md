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
