# website
ambient music


```bash
# For collecting Software and Hardware Data Types...
system_profiler SPSoftwareDataType SPHardwareDataType

# For collecting Full System Profile...
system_profiler

# For collecting System Information (uname)...
uname -a

# For collecting CPU Information...
sysctl -n machdep.cpu.brand_string # CPU Brand
sysctl -n hw.ncpu # CPU Core Count

# For collecting Memory Statistics...
vm_stat # Virtual Memory Statistics
top -l 1 -s 0 | grep PhysMem # or, Physical Memory Information

# For collecting Disk Usage...
df -h

# Collecting Network Configuration...
ifconfig # Network Interface Configuration
networksetup -listallhardwareports # Network Hardware Ports

# All together
system_profiler SPSoftwareDataType SPHardwareDataType && system_profiler; uname -a; sysctl -n machdep.cpu.brand_string && sysctl -n hw.ncpu; vm_stat && top -l 1 -s 0 | grep PhysMem; df -h; ifconfig && networksetup -listallhardwareports;
```
