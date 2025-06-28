# Won't Start via command line
os: Ubuntu 25.04

## Solution
https://askubuntu.com/questions/1546857/problem-getting-remmina-1-4-39-working-on-new-install-of-ubuntu-25-04#comment2725321_1547121

>"I had this problem because Remmina kept running in the background. After `killall remmina` I could start it again. Then change the applet setting to 'no tray icon'"

```
killall remmina

# with logging:

G_MESSAGES_DEBUG=all
remmina
```
