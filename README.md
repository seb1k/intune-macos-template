# Intune macOS Password Policy Template

A ready-to-use Apple configuration profile (`.mobileconfig`) to deploy a password policy on macOS devices managed by Microsoft Intune.

This profile is intended to help administrators meet common security recommendations such as Microsoft Secure Score, CIS benchmarks, and internal security policies.


## Validated policies

The template validates the following macOS secure score settings:

- Set account lockout threshold to 5 or lower in macOS
- Set minimum password length to 15 or more characters in macOS
- Set 'Maximum password age' to '90 or fewer days, but not 0' in macOS
- Set 'Enforce password history' to '24 or more password(s)' in macOS


## Requirements

- Microsoft Intune
- macOS devices enrolled in Intune
- Administrator permissions to create Configuration Profiles

## Add template : go to Intune > Devices > macOS | Configuration
Link : [macOS | Configuration](https://intune.microsoft.com/?ref=AdminCenter#view/Microsoft_Intune_DeviceSettings/DevicesMacOsMenu/~/configuration)


- Create new Policy
<img width="212" height="140" alt="image" src="https://github.com/user-attachments/assets/9c36bc69-13e6-4acf-a3ec-e48e6c256804" />

- Custom Template 
<img width="265" height="358" alt="image" src="https://github.com/user-attachments/assets/f900a98c-1078-4578-86d1-570a358856bf" />

#### Basics
- Name : Recommanded security rules (password policy template)

#### Configuration Settings
- Custom configuration profile name : **com.apple.mobiledevice.passwordpolicy.mobileconfig**
- Configuration profile file : Upload the `com.apple.mobiledevice.passwordpolicy` file from this repository.

#### Assignments
- **All devices**

#### Review + create
<img width="81" height="28" alt="image" src="https://github.com/user-attachments/assets/0fe79f6a-7e95-40d3-a11b-0f71e39a6841" />

## Testing

It is recommended to:

- Test on a small pilot group first.
- Verify deployment in Intune.
- Confirm the password policy is applied on macOS.
- Ensure users are informed if a password change is required.

## Notes

This template is based on Apple’s macOS passcode configuration profile documentation:
https://developer.apple.com/documentation/devicemanagement/passcode


## Testing

It is recommended to:

- Test on a small pilot group first.
- Verify deployment in Intune.
- Confirm the password policy is applied on macOS.
- Ensure users are informed if a password change is required.

## Microsoft Documentation

- https://learn.microsoft.com/intune/device-configuration/custom-settings-configure
- https://learn.microsoft.com/intune/fundamentals/deployment-guide-enrollment-macos

## License

MIT License

## Disclaimer

This project is provided as-is without warranty.

Always validate configuration profiles in a test environment before deploying them to production devices.
