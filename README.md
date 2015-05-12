**How To Install ?

- Copy the folder psmouse-elantech-x551c in your /usr/src directory

**Now run the following commands

- `sudo dkms add -m psmouse -v elantech-x551c`

- `sudo dkms build -m psmouse -v elantech-x551c`

- `sudo dkms install -m psmouse -v elantech-x551c`

- `sudo rmmod psmouse`

- `sudo modprobe psmouse`

**Add following lines to /etc/rc.local file before exit 0

- `sudo rmmod psmouse`
- `sudo modprobe psmouse`
