```
sudo launchctl disable system/com.apple.ODSAgent
sudo launchctl disable system/com.apple.screensharing
sudo launchctl load -w /System/Library/LaunchDaemons/com.apple.auditd.plist
sudo pmset -a womp 0
sudo defaults write /Library/Preferences/com.apple.mDNSResponder.plist NoMulticastAdvertisements -bool true
sudo launchctl unload -w /System/Library/LaunchDaemons/com.apple.nfsd.plist
sudo defaults write /Library/Preferences/.GlobalPreferences MultipleSessionEnabled -bool false
sudo defaults write /Library/Preferences/com.apple.security.libraryvalidation.plist DisableLibraryValidation DisableLibraryValidation -bool false
sudo AssetCacheManagerUtil deactivate
sudo /usr/libexec/ApplicationFirewall/socketfilterfw --setstealthmode on

```
