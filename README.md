# Validate macOS policies with Microsoft Intune

This repository contains a template designed to validate macOS security and compliance policies using **Microsoft Intune**.


## Validated policies

The template validates the following macOS secure score settings:

- Set account lockout threshold to 5 or lower in macOS
- Set minimum password length to 15 or more characters in macOS
- Set 'Maximum password age' to '90 or fewer days, but not 0' in macOS
- Set 'Enforce password history' to '24 or more password(s)' in macOS

## Prerequisites

- Microsoft Intune
- macOS devices enrolled in Intune

https://developer.apple.com/documentation/devicemanagement/passcode

## Add template

Add this template in Microsoft Intune in the same way as other macOS passcode configuration profiles :

https://learn.microsoft.com/en-us/defender-endpoint/mac-install-with-intune#step-2-network-filter
 
## Notes

This template is based on Apple’s macOS passcode configuration profile documentation:
https://developer.apple.com/documentation/devicemanagement/passcode
