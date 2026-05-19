 > Keep in note that if it worked for me it doesn't mean it will work for you. As of writing this, my laptop's BIOS version is `PQCN27WW`. I own a Lenovo LOQ 15ARP9 gaming laptop. It happened to me recently, about 3 to 4 days ago.
 > What I am getting from my solution and other solutions from the internet is that the `.bin` files have to match your BIOS' version. That means that mine is `PQCN27WW`, and the solution should be (and was) `pqcn.bin`.
 > If this guide works, what I can suggest is take a photo and remember your laptop's BIOS version, it might save you 3 days of senselessly copying a `.ROM` to a pendrive, renaming it to 100 different variations, then plugging it into the broken laptop only to realize it didn't work.

 # The guide

 ## What you need:

 - FAT32 USB drive
 - The correct BIOS package

 ## Setup:
 If you have a USB drive but it's not on FAT32 filesystem, then you have to format it to be correct. Here is how to do it if you don't know how:
 1. Plug in the USB drive *(I will be calling it pendrive later on)*
 2. Open file explorer and navigate to 'This PC'
 3. If you see your pendrive, right click it, then click **format**.
 4. What you are after is the **file system** dropdown menu, click it, then select FAT32.
 5. You don't have to bother with the menu below it, select default or 16 kilobytes.
 6. Click **start**
 Once it is finished, it will tell you so. **DO NOT UNPLUG YOUR PENDRIVE WHILE IT'S FORMATTING!** After it says it's done, you can go ahead and close the formatting window.

 ### Setup pt. II.
 Now you have your pendrive configured correctly! What you now need is the BIOS package. You can download it from Lenovo's website:
 https://pcsupport.lenovo.com/us/en .
 When it loads, you want to click **Browse Product**. Then click **Laptops**. Now, once you clicked it, all other device icons will gray out, and 2 dropdown menus will appear. Click **Select Series**, then type in "**G**", then you should see **Gaming Series Laptops** below G Series Laptops. Click **Gaming Series Laptops**. Then in the subseries,
 type in your laptop's subseries. For me, it's **LOQ 15ARP9**. After a new page loads, click **Drivers & Software**, it's the first one, click **Select Drivers** in the **Manual Update** card. Now you will see many buttons, click **BIOS/UEFI**. Now, you should see a __BIOS Update__, click the **Download** button that is at the end.
 Now, once you downloaded the bios update file. You are going to need another tool to extract the contents. I'd reccommend `innoextract`. However it doesn't work on desktop for some reason, atleast not for me. You need another laptop. Which if you don't have another laptop in your home, you might be cooked.
 There will be a copy of what I extracted from the installer by my other laptop. **If the BIOS version doesn't match with yours or you have a completely different laptop subseries, don't use it.**
 Now, you have to find a `.ROM` file. Mine is named `JLG52027.ROM`, this is what you need.
 1. Copy the `.ROM` file to your pendrive.
 2. Rename it to your bios version's first 4 letters, and replace `.ROM` with `.bin`. If you do not see the extensions in the file names, you have to enable in in file explorer, go to View and turn it on, it's on the far right, the middle one.
 > Now your file should be named `pqcn.bin` or something like that.
 3. Disconnect your pendrive safely after the operations are complete by going to your system tray, right clicking on the USB drive icon, and ejecting your pendrive there, if it responds with a notification saying it's safe to disconnect, you may disconnect it. If it doesn't say that and gives you a warning istead, wait for a few seconds and try again.
 
 ## Flashing the laptop
 You now have a pendrive configured properly with the correct file. **Turn off your laptop if you haven't already by keeping the power button held down until it's light turns off**. Then
 1. Disconnect power source
 2. Wait a few seconds (5 minimum)
 3. Plug in your pendrive into the USB port **closest to the charging port**. (All others should work but let's not put it to the test)
 4. Plug in the charger
 5. Hold down `Fn` and `R` keys
 6. While holding those keys, **press the power button once**, **then let go of the power button**.
 7. Keep holding those 2 keys for 10-15 seconds, __then let go__.

 Please wait for a few minutes, __it's not instantanious__. **Do not unplug the charger, nor the pendrive.** You might make things worse, tho I highly doubt it can get any worse than this.

 If your laptop starts beeping in a __heartbeat-like pattern__. **You did it!** If not, consider making a claim with __Lenovo's customer support__, and kindly tell them your situation in the **best of detail**. Depending on warranty *(mine is Premium Care on-the-spot)*, they should __send out a specialist__ to come solve it, or they will come to __collect your laptop__.