![banner](banner.png)

#Disable WebRTC Indicator Overlay Firefox Add-On
Removes the floating overlay with the firefox and camera icons that is displayed when the webcam or microphone are accessed over webrtc. This add-on is only meant for use in special environments like embedded applications or kiosk systems.

## Installation
You can get the add-on [here](https://addons.mozilla.org/en-US/firefox/addon/disable-webrtc-overlay/)

## Removing the Permissions Popup
In case you also wish to remove the popup that asks for permission to use camera/microphone, you can set `media.navigator.permission.disabled = true` in `about:conifg`. However, this should also only be done in controlled environments.

## Security and Privacy Implications
Please take into account that there is a reason that the developers introduced this overlay. Especially the combination of the two options can have serious security implications, because any website could listen to your microphone and camera without you even noticing. Only use both options in controlled environments and just the addon only when its really necessary for your application.

## Building and bundling

- Install the Mozilla Add On SDK as described here: https://developer.mozilla.org/en-US/Add-ons/SDK/Tools/jpm#Installation

- Ensure the `jpm` tool is in your path.

- Build the extension with `jpm xpi`

- Log in to https://addons.mozilla.org/en-GB/developers/addons and sign it.

- Download the signed extension.

