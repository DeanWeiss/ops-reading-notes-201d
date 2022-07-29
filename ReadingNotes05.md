# Windows Command Line Tools

#### Dean Weiss
#### 26 July 2022

## SMP Protocol

SMP works through a client-server approach, where a client makes specific requests and the server respondes accordingly. This protocol facilitates file shares between networked computers

This allows a user of an application to open, read, move, create and update files on the remote server.

NetBIOS identify eachother over TCP port 139

Microsoft merged SMB protocl with their LAN manager product.

Microsoft renamed SMB to Common Internet File System (CIFS) and added more features, including support for symbolic links, hard links, larger file sizes, and an initial attempt to support direct connections over TCP port 445 without requiring NetBIOS as a transport (a largely experimental effort that required further refinement).

Microsoft changed SMB to operate over port 445. SMB still uses port 445.

Microsoft continues to invest in improving SMB performance and security. SMB 3.0 which was introduced with Windows 8 and Windows Server 2012 brought several significant changes that added functionality and improved SMB2 performance, notably in virtualized data centers.

Additionally, it introduced several security enhancements such as end-to-end encryption and a new AES-based signing algorithm.

Port 139 - Used by SMB dialects that communicate over NetBIOS. It's a transport layer protocol designed to use in Windows operating systems over a network.
Port 445 - Used by newer versions of SMB (after Windows 2000) on top of a TCP stack, allowing SMB to communicate over the Internet. This also means you can use IP addresses in order to use SMB like file sharing.



###### Cited from: https://www.upguard.com/blog/smb-port
