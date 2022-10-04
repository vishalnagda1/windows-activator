## Getting started
What you first need to do is open CMD (Command Prompt) as Administrator using this keyboard key:

<kbd><img src="http://i.stack.imgur.com/B8Zit.png" width="11"></kbd> + <kbd>R</kbd>

And now type in ``cmd.exe`` in the box

It should now look as something like this:

![image](https://user-images.githubusercontent.com/66115754/134801377-b9769c34-8a9d-4d4f-ba8e-6c073f1ce4a2.png)

Now press this keys on your keyboard:

<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd>

Now you have something like this:

![UAC Permissions](https://user-images.githubusercontent.com/66115754/134801445-9b90e121-350b-42ea-afec-b499f1fbfae9.png)

Now, click on ``Yes``

Now you have something like this:

![Windows Command Prompt](https://user-images.githubusercontent.com/66115754/134807479-53ccdaf9-feb0-49a3-9843-5bb4db016128.png)

### The commands
Now, type the following command:
``slmgr.vbs /upk``

**Note**: this will remove your current activation key!
Now it will give an message, click on ``OK``

And now this command:
``slmgr.vbs /cpky``
It will give an message once again, and click on ``OK`` again

And now type this command:
``slmgr.vbs /ckms``
Once again click on ``OK`` when you get an message
### Edition upgradable check command
Now we are gonna check of your edition is supported to upgrade to Pro, run the following command to check this:
``DISM /online /Get-TargetEditions``
If you see ``Professional`` in the list, then you can upgrade your Windows edition to Pro for free!
### Running Windows Pro installer
Now, copy and paste this complete command:

``sc config LicenseManager start= auto & net start LicenseManager``

``sc config wuauserv start= auto & net start wuauserv``

``changepk.exe /productkey VK7JG-NPHTM-C97JM-9MPGT-3V66T``

``exit``

It will run an installer and you will see an message: ``% complete``

Now wait until it's 100% and then you get an error (This is normal, this needs to happen.)

When you get the error, just click Exit and then reboot your pc.

You will now see an message that he is running updates and is installing features, just wait until its done and check ``info`` in settings, You will see that Windows 10/11 Pro is installed! (**May show Windows Enterprise, but will be Windows Pro!!**)

But we are not done, You will see that it isn't activated and that you can't change some settings, now we are gonna fix that!

## Method 1 For Activating Windows Pro
There's another method with a batch file. You can download it by [clicking here](https://vishalnagda1.github.io/windows-activator/activator.bat).
It will start to download. Click ``Save (As)`` to save it. Now we need to open Windows Explorer. First, click these keyboard keys together:

<kbd><img src="https://svgshare.com/i/dg_.svg" width="11"></kbd> + <kbd>R</kbd>

Type ``explorer.exe`` in the box and click ``Enter`` on your keyboard or click ``OK``.
Now it will open Windows Explorer. You're here now:
![Windows Explorer On Start With Windows 11](https://user-images.githubusercontent.com/66115754/163762296-3bfe5cb5-0c2d-4464-9398-7eaa48c95c53.png)
Click on ``Downloads``, or go to the directory where you saved the downloaded batch file. Now you are here (or on a different place):
![Downloads Folder With Batch File On Windows 11](https://user-images.githubusercontent.com/66115754/163762758-67484b44-e0fe-402d-aad1-37b2a07373ee.png)
Click on the batch file 1 time, then right click and click ``Run As Administrator``. It will ask for UAC permissions. Click ``Yes`` now. Now a console windows will open. Wait until it says ``<product activation succesfull>``. Now you activated Windows Pro for free! It also asks if you wanna see someone's blog. Press ``Y`` if you want to and ``N`` if you don't want to see.

## Method 2 For Activating Windows Pro
Now we are gonna run some other commands to activate Windows 10/11 Pro.

Press these keyboard keys once again:

<kbd><img src="https://svgshare.com/i/dg_.svg" width="11"></kbd> + <kbd>R</kbd>

It looks like this again:

![Run Dialog With cmd.exe Text In It](https://user-images.githubusercontent.com/66115754/134801377-b9769c34-8a9d-4d4f-ba8e-6c073f1ce4a2.png)

Press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd>

You will get an message, just click on ``Yes``

Now you will get an Command Prompt.

Type the following commands one for one to activate:

``slmgr /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX``

``slmgr /skms kms8.msguides.com``

``slmgr /ato``
 
**Note**: This does not always work. When running ``slmgr /ato`` it does not always work, but keep trying.
Now you have Windows 10/11 Pro and it activated! You can check settings to see it.


#### Contributing

1. Fork it ( https://github.com/vishalnagda1/windows-activator/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new pull request.
