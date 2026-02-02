# Validate macOS policies with Microsoft Intune

This repository contains a template designed to validate macOS security and compliance policies using **Microsoft Intune**.


## Validated policies

The template validates the following macOS secure score settings:

- Account lockout threshold set to 5
- Minimum password length set to 15
- Maximum password age set to 90 days
- Enforce password history set to 24 passwords


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
