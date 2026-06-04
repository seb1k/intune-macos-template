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

## Add template : go to Intune > Devices > macOS | Configuration
Link : [macOS | Configuration](https://intune.microsoft.com/?ref=AdminCenter#view/Microsoft_Intune_DeviceSettings/DevicesMacOsMenu/~/configuration)


- Create new Policy
<img width="212" height="140" alt="image" src="https://github.com/user-attachments/assets/9c36bc69-13e6-4acf-a3ec-e48e6c256804" />

- Custom Template 
<img width="265" height="358" alt="image" src="https://github.com/user-attachments/assets/f900a98c-1078-4578-86d1-570a358856bf" />

#### Basics
- Name : Recommanded security rules (password policy template)


#### Configuration Settings
- Custom configuration profile name : **com.apple.mobiledevice.passwordpolicy**
-  Configuration profile file : put the `com.apple.mobiledevice.passwordpolicy` file from the repo

#### Assignments
- **All devices**

#### Review + create
<img width="81" height="28" alt="image" src="https://github.com/user-attachments/assets/0fe79f6a-7e95-40d3-a11b-0f71e39a6841" />



## Notes

This template is based on Apple’s macOS passcode configuration profile documentation:
https://developer.apple.com/documentation/devicemanagement/passcode
