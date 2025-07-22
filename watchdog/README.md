# Compile
```
gcc wdt.c -o wdt
```

# Disable the system watchdog

## Step1. Open watchdog.conf file
`sudo vi /etc/systemd/system.conf.d/watchdog.conf`

## Step2. Modify
```
[Manager]
# RuntimeWatchdogSec=120
RuntimeWatchdogSec=0
```
## Step3. Reboot
`sudo reboot`

# Test
```
# System will reboot automatically after timeout
sudo ./wdt <timeout in seconds>
```
- default: 60 seconds, if there is no timeout value as input parameter