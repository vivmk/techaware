---
title: "Everything you need to know about the Tor Browser - Part 2"
date: 2020-10-09T19:18:14+05:30
draft: false
author: "Khaleeq"
description: "Tor can be used on almost all the popular devices today - be it running Linux, Windows, Mac, Android or iOS. It is also supported by IOT devices. You can directly fire up the Tor Browser on these systems but its not the most effect way to utilize Tor."
tags: ["Intermediate", "Tor", "Guide"]
---

## Part 2: How to use Tor?

Tor can run on antyhing that has an eletric plus be it Windows, Mac, Linux, Android ,iOS or IOT devices. Today we are going to explore how to use TOR on the following platforms

- Tor on Windows, Mac and Linux
- Tor on Android and iOS
- Tor on IOT devices

---

### Tor on Windows, Mac and Linux

You can directly fire up the Tor Browser on these systems but its not the most effective way to utilize Tor. As we all know how _privacy oriented_ Windows and Mac are  :joy:, it is not advised to run the Tor Browser on these systems. The same goes with the Tor on Virtualbox or Vmware.

Let us not forget Tor is privacy tool not an anonymity tool. So I would insist you use an OS built for Tor like **Tails**. You can download the Tails and burn it to your USB and your good to go. I will also show you how to make a persistent volume on the Tails USB.

#### Setting up Tails USB

##### Requirements

- 15 Minutes of your precious time
- A USB stick with minimum 4 GB storage

Let us get started!

Download the Tails OS form the [Tails](https://tails.boum.org/install/index.en.html). Always be up to date on the Tails OS because new bugs and vulnerabilities get discovered everyday. After downloading, [verify](https://tails.boum.org/install/win/usb-download/index.en.html#install-inc-steps-download.inline.basic-openpgp) the checksum.

> _Pro tip: Always verify the downloaded checksum regardless of just this OS!_

Burn the Tails OS to your USB using [_Rufus_](https://rufus.ie/). Now boot from your USB.

When you boot up the USB you'll be presented with this screen, by default your MAC address will be spoofed and only Tor Browser will be allowed to run, other Browsers will be disabled.

You can setup the Admin password if you want to access any internal system drives (this is not advised) or execute any root user commands (again this is not advised unless you have something legit to do). Nothing wrong with setting up the Admin password unless you know what you are doing.

![Initial boot](https://www.linkpicture.com/q/VirtualBox_Tails-4.11_09_10_2020_13_32_11.png)

![Additional Settings](https://www.linkpicture.com/q/VirtualBox_Tails-4.11_09_10_2020_13_32_31.png)

This is live system, meaning you can not save anything, and all the customizations made to Tails USB will be lost when you reboot. Not only this, but Tails also wipes the RAM to protect you from cold boot attacks.

And if you remove the USB while the system is running the system wipes the RAM and shuts down.

Tails changes your timezone, runs all your network traffic through Tor chain and reduces your fingerprints on the internet.

![Tor Browser](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-53-01.png)

Do not run Tor Browser in full-screen because this can give up your screen resolution which adds to your web fingerprint.

![Tor Browser](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-53-12.png)

As you can see the IP address, we are connected to Tor network.

You can also change the security level...

![Security](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-53-54.png)

![enter image description here](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-09-54-16.png)

#### Configuring the persistent volume

So if you want to save anything you would need a persistent volume. The persistent volume is encrypted so you need not worry if someone gets their hands on your Tails USB.

This is very useful is you are using _cryptocurrency_ or basically anything and you are tired of configuring every time.

Open the Applications > Tails and Configure persistent volume. You'll be presented with a persistent setup wizard and pretty much follow the instruction on the screen.

![Configuring the persistent volume](https://www.linkpicture.com/q/VirtualBox_Tails-4.11_09_10_2020_13_36_49.png)

![Persistence wizard](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-15-05-37.png)

Select the applications or utilities for which you would want to enable persistence and select save:

![Setup](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-15-06-51.png)

![Reboot](https://www.linkpicture.com/q/Screenshot-from-2020-10-09-15-14-21.png)

You have to reboot in order for the persistence to work:

![setup complete](https://www.linkpicture.com/q/IMG_20201009_143844.jpg)

To delete persistent volume select delete persistent volume in Applications > Tails.

---

### Tor on Android and iOS

#### Android

Tor Browser for Android is the only official mobile Browser supported by the Tor Project. [Install](https://play.google.com/sTore/apps/details?id=org.Torproject.TorBrowser) it from the Google Play Store and you are good to go!

Also check out [Orbot](https://play.google.com/sTore/apps/details?id=org.Torproject.android), a free proxy app that empowers other apps to use the internet more securely. Orbot uses Tor to encrypt your Internet traffic and then hides it by bouncing through a series of computers around the world. All your trafic for the selected app will be routed through Tor cahin.

#### iOS

Install the Tor Browser from Apple App Store and you are good to go. [Onion Browser](https://apps.apple.com/us/app/onion-Browser/id519296448) is the original free and open-source Tor powered web Browser for iOS.

---

### Tor on IOT devices

Why don't you go and figure that out by yourself? :wink: