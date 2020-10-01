---
title: "How to install Burp Suite Professional for free on Windows"
date: 2020-09-06T21:19:22+05:30
draft: false
---

Burp Suite is an integrated platform for performing security testing of web applications. It is designed to be used by hands-on testers to support the testing process. Here we will see how you can install it for free on your Windows 7/8/10 64-bit machine.

Things that you will need:

1. Java JDK (13.0.2) - [Download](https://rb.gy/makqnd)
2. Burp Suite Pro zip file (2020.9) - [Download](https://t.me/burpsuite/135)

---

After you have downloaded both the files, follow these steps:

- Run the downloaded file `jdk-13.0.2_windows-x64_bin.exe` and let it install.

- Search `environment` in the Windows search bar. You will see a match for `Edit the system environment variables`. Open it and then click `Environment Variables` button in the bottom.

  You will see a window containing a part like this:

  ![Environment Variables](https://www.linkpicture.com/q/variables.png)

Under the System variables tab, click `New` and add the following variables:

`Variable name: CLASSPATH`

`Variable value: C:\Program Files\Java\jdk-13.0.2\lib\*.jar`

---

Click OK. Then click `New` again and add another variable:

`Variable name: JAVA_HOME`

`Variable value: C:\Program Files\Java\jdk-13.0.2`

---

Finally, double click the `Path` variable and click `New`. Add the following path:

`C:\Program Files\Java\jdk-13.0.2\bin`

Click OK and close Variables Window. You are half way there.

---

Now extract the downlaoded `BurpSuite_Pro_2020.9.zip`. Use the password: 311138 if prompted. You will see three `.jar` files and one `.txt` file. Open the folder.

- Press and hold Shift key and right click on the screen. Click open `Command Prompt` or `Windows Powershell` window here.
- Paste and run the following command:

  `java -javaagent:BurpSuiteLoader_v2020.9.jar -noverify -jar burpsuite_pro_v2020.9.jar`

- Follow the instructions to install Burp Suite.
- When you reach the License activation page, open a new Command Prompt window again in the same folder and run the following command:

  `java -jar burploader-old.jar`

- You will see the following window:

![Burp Suite License Activation Window](https://www.linkpicture.com/q/activation.png)

- Copy the text in License box and paste it in your installation window and hit Next.
- Select Manual Activation, copy the Activation Request key and paste it in the above shown window to get the Activation Response key.
- Paste the Response key in the installation window and you are done!

#### How to open the installed Burp Suite Pro?

- Open Notepad and paste the following command in it:

  `java -javaagent:BurpSuiteLoader_v2020.9.jar -noverify -jar burpsuite_pro_v2020.9.jar`

- Now save the file as Burp.bat
- Open that file whenever you want to open Burp.

---

Congrats, you have successfully installed Burp Suite Pro. If you have any queries or doubts, feel free to ping me on [Telegram](https://t.me/vvekm) messenger. I will be happy to help you!
