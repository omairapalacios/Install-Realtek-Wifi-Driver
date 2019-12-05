# Guide to Install RLT_WifiDRiver in Linux Distributions
#### Based in : https://github.com/lwfinger/rtlwifi_new

- Before of begin with installation may you need to run this command to update to download the package lists from the repositories and "updates" them to get information on the newest versions.

  `sudo apt-get update`

- The next command is used for install numerous packages and tools for compiling/building software.

  `sudo apt-get install build-essential`

- Install git to get the drivers repository

  `sudo apt install git`

- Clone the repository where is the drivers

  `git clone https://github.com/lwfinger/rtlwifi_new.git -b extended`

- Enter to the cloned folder

  `cd rtlwifi_new`

- Access to the branch extended

  `git checkout extended`

- Now, install make, make is typically used to build executable programs and libraries from source code

  `sudo make install`

- Add the modules:
    -sudo modprobe -r "Your Wireless driver code" for example:
  
    `sudo modprobe -r rtl8723de`

    -sudo modprobe "Your Wireless driver code" for example:

    `sudo modprobe rtl8723de`

### This is all!
