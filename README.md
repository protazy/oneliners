# oneliners

## MacOS
### Turn off system daemons
```
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.mDNSResponder.plist
```
Replace the .plist file with the relevant service descriptor. Relevant service descriptor locations:
* Service descriptor locations:
* /System/Library/LaunchDaemons/ - System-wide daemons provided by Mac OS X
* /System/Library/LaunchAgents/ - Per-user agents provided by Mac OS X.
* ~/Library/LaunchAgents/ - Per-user agents provided by the user.
* /Library/LaunchAgents/ - Per-user agents provided by the administrator.
* /Library/LaunchDaemons/ - System-wide daemons provided by the administrator.
