## Step 0
As stated on the previous install page, you MUST install Nodejs from [nodejs.org](https://nodejs.org). If you do not install this IT WILL NOT WORK.

If you are running Windows 10, please either Disable the service ``World Wide Web publishing Service`` or run ``net stop`` from CMD.

If you would prefer to watch a video that goes along with this, please click [here.](https://www.youtube.com/watch?v=x_A58Ttvjd0)
## Section 1: Preparing the Application

Step 1. Clone the Repository. For ease of updating I suggest that you clone the repository, if you do not know how to do that then please follow this [guide.](https://github.com/OstlerDev/PopcornTV/wiki/How-to-Clone-the-Project)  
Step 2. Open the Command prompt and enter the commands below.
```sh
$ cd Desktop
$ cd PopcornTV
$ npm install
$ node atv.js
```
Step 3. If you see something like below then you are ready to move on. (Only stop if there are errors. If there is an error please follow what the error is saying)
```
Starting PopcornTV
DnsProxy binding on 10.0.1.2:53
Web: listening on 10.0.1.2:80
SSL Web: listening on 10.0.1.2:443
Starting Commit: (numbers and chars)
```

## Section 2: Preparing your Apple TV

Step 1. Go to your Apple TV and select the settings Application.  
Step 2. Select General > Network > "Your Network" > "Your network" again. You should end on a page that says "Wifi Configuration" at the top. (It might also say "Ethernet Configuration", this is normal and OK)  
Step 3. Go down to "Configure DNS" and set it to Manual, then enter in the **local IP address of your Computer** that is running PopcornTV (it should show this in CMD). In my case it was "10.0.1.2". (You will see that the DNS setting has 3 spaces for each section, for me since my IP is "10.0.1.2", I would put "010.000.001.002" in the spaces, just add zeros where needed.)  
Step 4. Once the DNS is set, menu out back to the "General" page.  
Step 5. Scroll down to where it says "Send Data to Apple" and select it then set it to "No"  
Step 6. Once your setting says "No", while hovering over "Send Data to Apple" (like shown in the image below) press the "Play/Pause" button on your Apple TV remote. It will open up a screen that we will use in the next window.  
![](http://i.imgur.com/ZUwdFkq.jpg)
Step 7. Select "Add Profile" then click "Ok"  
Step 8. On the "Add Profile" page it should pull up a text box. Type in "http://trailers.apple.com/trailers.cer" then click "Submit". This adds a custom profile to your Apple TV that allows SSL connections between your Apple TV and the PopcornTV Application.  

## Section 3: Wrapping Up

You are now done with the installation! Just make sure PopcornTV is running whenever you wish to use it!

PopcornTV runs inside the Trailers application on your Apple TV. Just open the trailers application to begin.