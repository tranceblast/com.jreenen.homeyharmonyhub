# Homey Harmony Hub Support

This project is in very early stage of development. At the moment this project supports:
- Pairing of devices connected to the harmony hub
- A mobile card supporting the power toggle functionality of the device
- An action card for sending a specific command to the harmony device using homey flows.

# Setup

Once the app is installed you can pair a device that is connected to the harmony hub:

![alt text](https://github.com/jreenen/com.jreenen.homeyharmonyhub/blob/master/assets/images/Device%20Pairing.gif "Device pairing")

After you have paired your device it will be available in the homey flow editor allowing you to send IR commands to this device:

![alt text](https://github.com/jreenen/com.jreenen.homeyharmonyhub/blob/master/assets/images/Device%20flow.gif "Using your device in homey flow manager")

# Future releases

At the moment there is no real roadmap but for the upcoming release you can expect the following:
- Support for Harmony Hub activities
- More flow cards (triggers, conditions, and actions)
- More device type icons (right now only GameConsoleWithDvd, television, stereo receiver, and PVR have a custom icon assigned) 

# Why developing another homey harmony hub driver when there already is one available?

I am aware there is already a [great project](https://github.com/netactivenl/com.logitech.harmony.hub) with a working harmony hub driver. Because I would like to have a different pairing strategy which would be a fundamental difference I decided to start a project of my own.

# What does this app track?

This app uses application insights to track the following topics:
- Application errors, which help to solve issues
- Unknown device types, so I can add more icons in future releases, making it easier to find the device you are looking for in the Homey flow editor.

# Donations
If you like the work on this project please consider a donation. Of course, this is optional and you should in no way feel obligated to send a donation. The donations will be spent on buying a second Harmony Hub to support me testing a multi-hub situation.

<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_s-xclick">
<input type="hidden" name="encrypted" value="-----BEGIN PKCS7-----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-----END PKCS7-----
">
<input type="image" src="https://www.paypalobjects.com/en_GB/i/btn/btn_donate_SM.gif" border="0" name="submit" alt="PayPal – The safer, easier way to pay online!">
<img alt="" border="0" src="https://www.paypalobjects.com/nl_NL/i/scr/pixel.gif" width="1" height="1">
</form>

# Used external library's

[swissmanu's harmonyhubjs-client](https://github.com/swissmanu/harmonyhubjs-client)

[swissmanu's harmonyhubjs-discover](https://github.com/swissmanu/harmonyhubjs-discover)



