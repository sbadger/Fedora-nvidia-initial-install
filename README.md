# Fedora-nvidia-initial-install
When you install hangs with a Nvidia video card


When presented with the list of boot options highlight "StartFedora-Workstation-Live 30"
then press 'e'
then go to the line that starts with "linuxefi"
add the following to the end of the line
xdriver=vesa modprobe.blacklist=nouveau

My line looks like this
linuxefi /images/pxeboot/vmlinuz root=live:CDLABEL=Fedora-WS-Live-3020190326-n-0 rd.live.image xdriver=vesa modprobe.blakclist=nouveau
then press ctrl-x to boot
