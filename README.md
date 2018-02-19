These are some scripts I've written over time to help with some tasks, below is a list of what each script does:  
* die-webp - The default image-viewer on Xubuntu (ristretto) doesnt work with webp images. 
Make Thunar (file manager) open webp images using this script, and it'll convert the webp image to png using `dwebp` command from `webp` package, delete the webp image, and
open the resulting png image using default image viewer
* getip - just prints the ip address
* ptclstatus - my ISP (PTCL) is a bit annoying, and sometimes, it keeps disconnecting frequently. The connection status can be seen from `192.168.10.1:80`, 
but that requires me entering the username & password, but after some tinkering, I found that the data I need is provided at `192.168.10.1:80/port_link_status` in JSON 
format. This script runs in background, reads that JSON status every 30 seconds, and shows notifications if it disconnects/connects
* trackpad-toggle - enables/disables the trackpad, had to write it because Fn+F8 didnt work out-of-the box for my ThinkPad with Xubuntu
* netmon - this script is to be run in background. It scans the network (LAN) after every specfied number of seconds (60 default), and gives notifications when a device leaves 
or joins the network. It requires the `fping` package to be installed, `sudo apt install fping` for ubuntu installs it.

---

## License
All these scripts are licensed under MIT license, contained in `LICENSE.md`