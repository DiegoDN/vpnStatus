A simple utility that displays an indicator in the system tray regarding your VPN connection status.

You can find more details on [original repo](https://github.com/rvaccarim/vpnStatus) and on [original blog post](https://robertovaccari.com/blog/2021_02_24_vpn_status).

My take on this customize two things:

* The icons (the original icons are very good, but I'm colorblind and have a hard time to differentiate between the used icons to show connected and disconnected states). You will see that the icon for connected was chaged to a Big Red Cross to remind me to disconnect from VPN after use (my actual VPN is very slow).

  |Original Icon|Modified Icon  |
  |--|--|
  |![original icon](https://raw.githubusercontent.com/DiegoDN/vpnStatus/e0a40e667e7e93e12d52f397b6e8377d7778dbe8/vpnStatus/Resources/Active_original.ico =100x) | ![new icon](https://raw.githubusercontent.com/DiegoDN/vpnStatus/e0a40e667e7e93e12d52f397b6e8377d7778dbe8/vpnStatus/Resources/Active.ico =100x) |

* The arguments: For some unknown reason the original args dont always identify my VPN. I've changed the arguments to:

  `"/C ipconfig | find /i \"VPN\""`
  

To build this I've used Visual Studio 2019.
