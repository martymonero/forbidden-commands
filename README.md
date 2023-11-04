# forbidden-commands
A curated list of useful commands that I needed for a specific task. No lecturing here. If you are here you know why you need them. Eval is not evil.


# WINDOWS
## Disable Windows Defender

Run Powershell As Administrator

### Disable Real Time Monitoring Only (For reversing Malware, etc..)
```
Set-MpPreference -DisableRealtimeMonitoring $true
```

### Disable more features
```
Set-MpPreference -DisableIntrusionPreventionSystem $true -DisableIOAVProtection $true -DisableRealtimeMonitoring $true -DisableScriptScanning $true -EnableControlledFolderAccess Disabled -EnableNetworkProtection AuditMode -Force -MAPSReporting Disabled -SubmitSamplesConsent NeverSend
```

# MACOS

## Show All Hidden Files
```
defaults write com.apple.Finder AppleShowAllFiles true
killall Finder 
```
