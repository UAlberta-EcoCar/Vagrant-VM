#OS
##Ubuntu
The standard vagrant VM should be under Ubuntu 16.04. This should be upgraded regularly until the next LTS release (post 14.04) is released. We should then be hpping from LTS release to LTS release.

##Debian
Debian Sid should me made available in case anyone finds Ubuntu too bloatwarey. If anyone runs into issues with Ubuntu, or if anyone wants a change of pace or to learn a bit more about how linux works under the hood, the Debian VM should be used. This should be updated with every major Debian release.

#Software
##Platform IO
VMs should come with platform IO preinstalled. This includes various platform IO related tricks that allow platform IO to work under linux "out of the box"

###udev rules
VMs should come with the default VM rules installed that allow platform IO to query /dev/ files without root access. These can be found at https://raw.githubusercontent.com/platformio/platformio/develop/scripts/99-platformio-udev.rules

###clang
The clang package should be installed for linting/code completion. These can be found through standard repos for both Debian and Ubuntu
