---
title: "Everything you need to know about hidden part of the Internet"
date: 2020-09-10T18:30:29+05:30
draft: false
author: "Khaleeq"
description: "How to use TOR"
tags: ["Intermediate", "Cyber-security", "Guide"]
description: "TOR can be used on pretty much anything with an electric pulse, it can run on Linux, Windows, Mac, Android, iOS and any IOT device."
---

# Part 2: How to use TOR?

TOR can be used on pretty much anything with an electric pulse, it can run on Linux, Windows, Mac, Android, iOS and any IOT device.

- TOR on Windows, Mac and Linux
- TOR on Android and iOS
- TOR on IOT devices

# TOR on Windows, Mac and Linux

You can directly fire up the TOR browser on these systems but its not the most effect way to utilize TOR. As we all know how privacy oriented Windows and Mac are, it is not advised to run the TOR browser in these systems. The same goes with the TOR in Virtualbox or Vmware.

Lets not forget TOR is privacy tool not an anonymity tool. So I would insist you use an OS built for TOR like **Tails**.

You can download the Tails and burn it to your USB and your good to go. I will also show you how to make a persistent volume on the Tails USB.

## Setting up Tails USB

### Requirements

- 15 Minutes of your precious time .
- A USB of stick (Minimum 4 GB).

Lets get started.....

Download the Tails OS form the [_Tails website_](https://tails.boum.org/install/index.en.html). Always be up to date on the Tails OS because new bugs and vulnerabilities get discovered everyday.

And after downloading the Tails OS **[verify the checksum](link%20coming%20soon)**.

> _Always verify the downloaded checksum regardless of just this OS._

Burn the Tails Os to the USB using [_Rufus_](https://rufus.ie/).

Now boot from your USB.

When you boot up the USB you'll be presented with this screen, by default your MAC address will be spoofed and only TOR browser will be allowed to run, other browsers will be disabled.

You can setup the Admin password if you want to access any internal system drives (this is not advised) or execute any root user commands (again this is not advised unless you have something legit to do). Nothing wrong with setting up the admin password unless you know what your doing.

![Initial boot](https://www.linkpicture.com/q/VirtualBox_Tails-4.11_09_10_2020_13_32_11.png)

![Additional Settings](https://www.linkpicture.com/q/VirtualBox_Tails-4.11_09_10_2020_13_32_31.png)

This is live system, meaning you cant save anything and all the customization made to Tails USB will be lost when you reboot. Not only this but Tails also wipes the RAM to protect you from cold boot attacks.

Tails changes your timezone, runs all your network traffic through TOR chain and reduces your fingerprints on the internet.

![tor browser](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-53-01.png)

Do not run TOR browser in fullscreen because this can give up your screen resolution and add to your web fingerprint.

![enter image description here](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-53-12.png)

As you can see the IP address, we are connected to TOR network.

You can also change the security level....

![enter image description here](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-53-54.png)

![enter image description here](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-54-16.png)

And if you remove the USB while the system is running the system wipes the RAM and shuts down.

### Configuring the persistent volume

So if you want to save anything you would need a persistent volume. The persistent volume is encrypted so you need not worry if someone gets their hands on your Tails USB.

This is very useful is you are using _cryptocurrency_ or basically anything and you are tired of configuring every time.

Open the Applications, Tails and Configure persistent volume. You'll be presented a persistent setup wizard and pretty much follow the instruction the screen.

![Configuring the persistent volume](https://www.linkpicture.com/q/VirtualBox_Tails-4.11_09_10_2020_13_36_49.png)

![Persistence wizard](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-15-05-37.png)

Select the applications or utilities for which you would want to enable persistence and select save...

![Setup](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-15-06-51.png)

![Reboot](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-15-14-21.png)

You have to reboot in order for the persistence to work

![setup complete](https://www.linkpicture.com/q/IMG_20201009_143844.jpg)

To delete persistent volume select delete persistent volume in Applications, Tails.

# TOR on Android and iOS

### Android

Install the TOR browser from Play Store and you are good to go...

![tor](https://www.linkpicture.com/q/Screenshot_20201009-174616.jpg)

[TOR Browser](https://play.google.com/store/apps/details?id=org.torproject.torbrowser) for Android is the only official mobile browser supported by the TOR Project.

![orbot](https://www.linkpicture.com/q/Screenshot_20201009-174641.jpg)

[Orbot](https://play.google.com/store/apps/details?id=org.torproject.android) is TOR free proxy app.

### iOS

Install the TOR browser from App Store and you are good to go...

![enter image description here](https://is1-ssl.mzstatic.com/image/thumb/Purple113/v4/da/b9/ac/dab9acf3-7946-dc77-7170-70662e920655/pr_source.png/600x0w.png)

[Onion Browser](https://apps.apple.com/us/app/onion-browser/id519296448)Onion Browser is the original free and open-source Tor-powered web browser for iOS

# TOR on IOT devices

yeah you go figure this out by yourself...
