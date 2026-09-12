# SubLim3 Remote Support for Android

This is the source for the SubLim3 Innovations view-only Android support client, based on RustDesk 1.4.9.

## Security profile

- Uses `support.sublim3innovations.com` and the matching public encryption key.
- Remote keyboard/touch input is disabled.
- Clipboard, file transfer, audio capture, camera, and remote permission changes are disabled.
- The Android Accessibility input service is excluded from the application manifest.
- Android still requires the device owner to approve screen capture when starting support.

## Licensing

This modified client remains licensed under GNU AGPL v3, consistent with the upstream RustDesk client. The complete corresponding source is provided in this repository. RustDesk is an upstream project; SubLim3 Innovations is responsible for this modified build.

## Updating

Keep the Android signing keystore and its credentials permanently. Every future APK for this package must use the same signing key. Rebase S3 changes onto a reviewed upstream release, run the Android build workflow, test on a non-production device, and then publish the resulting APK.
