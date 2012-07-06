Sharicloud
==========

Sharicloud - Portable Owncloud with zero configuration

Project idea - Portable Owncloud Sharicloud:
Goals: 
1. Portable- hardware independent solution for shared storage server
2.Easy to deploy - zero configuration
3.Ease of use - clientless  web interface+various connection options (WebDAV,SSH, cifs?, nfs?)
Architecture:
1. Underlying OS: Bootable USB with custom Ubuntu (Ubuntu-builder) 
running vbox(qemu?) with owncloud_TC (sharicloud)
2.Storage space in vdi container + option to mount over network ssh,cifs,nfs
3.Interface: web+WebDAV (owncloud), SSH+CIFS?+NFS?(TC)
Add-ons(?):
Dyndns client
elFiler web interface- drag&drop files, compress/decompress  rar,
Local VMXRay for mounting VDI - recovery solution
VDI Fuse in Ubuntu for mounting VDI- recovery/share from vdi 
Clustering configuration with VBox teleport
Encryption of VDI Data Container
Tasks:
Check which VM container (vmdk,vdi,qcow2,iso etc.) is easily resizable
How to mount virtual container to any OS (over web browser to rw)
Decide what to put visible on USB partition when not booting from USB:
Both VDI (TC_owncloud and data container)
Portable VDI mounting tool ?
Portable chrome?
Portable Qemu/VBox?
?- because of .exe/viruses + platforms to support