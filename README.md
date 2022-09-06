[Yomichan](https://foosoft.net/projects/yomichan/) is a popular chrome extension for Japanese learners where you can hover over a Japanese word and see its meaning in English, like this
![enter image description here](https://miro.medium.com/max/1044/1*Ep4UPSzg0eqcHfTEEtCB7g.png)

Better yet, with some setup you can also hear a native speaker pronounce that word (click the mic icon) and even add that word into an Anki deck (green plus button) however you want! 

Since Yomichan takes a dictionary file as an input, it is not limited to only Japanese -- its pop-up UI can work with any language that has a compatible dictionary file, including Chinese. At the moment Yomichan only supports Japanese audio out of the box, however with some setup we can get Yomichan to talk to us in Native Mandarin instead!

This is the same addon as the [jamesnicolas' Yomichan Forvo Server](https://github.com/jamesnicolas/yomichan-forvo-server) but with Native Mandarin speakers from the audio by default rather than native Japanese speakers. You can directly clone this repo into your add-ons folder in Anki or install the add-on straight to Anki from [Ankiweb](https://ankiweb.net/shared/info/1118415626) (steps below). 

Before we begin we need to download a dictionary that we like. Thanks to  [Antti Pham](https://github.com/anttipham) we have a variety of different dictionaries we can use. Take a look at the different kinds of options below and download whichover one you like. **NOTE: DO NOT UNZIP THE FILES** we will be uploading the .zip itself to Yomichan in a later step. 

[Numbers instead of tone marks w/ bullet points](https://github.com/anttipham/cc-cedict-for-yomichan/releases/download/v1.1/CC-CEDICT.bullet.points.+.number.pinyin.zip)
![dict1](https://imgur.com/S5JxlMA.jpg)

[Tone marks w/ bullet points](https://github.com/anttipham/cc-cedict-for-yomichan/releases/download/v1.1/CC-CEDICT.bullet.points.zip)  (I use this personally)
![enter image description here](https://imgur.com/vixUCG3.jpg)

[Tone marks no bullet points](https://github.com/anttipham/cc-cedict-for-yomichan/releases/download/v1.1/CC-CEDICT.normal.zip)
![dict3](https://imgur.com/rFsxgrg.jpg)

[Numbers no bullet points](https://github.com/anttipham/cc-cedict-for-yomichan/releases/download/v1.1/CC-CEDICT.number.pinyin.zip)
![enter image description here](https://imgur.com/ZwlJC7Z.jpg)

Now that we have a dictionary *and we're not unzipping it* we need to have the following downloaded and installed

*   [Yomichan](https://foosoft.net/projects/yomichan/) if you haven't already 
*   [Anki](https://apps.ankiweb.net) - Even if you don't plan on using Anki flashcards Anki needs to installed and running whenver you want Chinese Audio
*   [Anki Connect](https://ankiweb.net/shared/info/2055492159)
* [This add-on for Native Mandarin](https://ankiweb.net/shared/info/1118415626)

In case you're unsure how to install Anki Add-ons like Anki Connect from above please refer to [this](https://scrubsjourney.com/how-to-add-anki-add-ons/) guide which is done on MACOS but the same steps will work on Windows just fine. Remember to use the code `2055492159` for Anki connect and `1118415626` for Mandarin audio when installing the add-on instead of the one used on the guide!

With everything installed we are ready to configure Yomichan for Mandarin!

**optional**
After you install Yomichan it will always open up the settings menu when you open your browser. In case you want to turn this feature off click 


![turn off browser open](https://i.imgur.com/JG1FW76.jpg)


1.  In case you aren't automatically in Yomichan go to the puzzle icon in your browser to open up your extensions: 

      ![find extension](https://imgur.com/iHZdif1.jpg)

2. Once you click that go to where Yomichan is and find the three dot icon:
	![click that and find ](https://imgur.com/6qMkV0e.jpg)
	
3. Click that and you'll see a menu like below. Once you're there you'll see a screen with options -- click that:
![click options](https://imgur.com/EXAjlYH.jpg)

4. Once you're in the settings page you will see a *Dictionaries* menu. Click on `Configure installed and enabled dictionaries...`
![click install dictionary](https://imgur.com/1oAs3KC.jpg)

5. Next you need to click import and select the dictionary you just downloaded. 
 ![import dictionary](https://imgur.com/vq78tfg.jpg)


6. Now we need to make sure that Anki and Yomichan are connected. Remember, *even if you don't plan on ever using Anki* we need it turned on when trying to get Mandarin audio. On the left side of Yomichan you'll find a box of options, click Anki button to go to the Anki settings:

   ![enter image description here](https://imgur.com/lfUDbd9.jpg)

7. Make sure `Enable Anki Integration` is on and says its connected like so. It may already be connected in which case no further steps are needed :) 

![enter image description here](https://imgur.com/DCw8UKU.jpg)

8. Now we need to setup the audio so it outputs in Chinese, go back to the sidebar and select Audio:
![enter image description here](https://imgur.com/yUm5q8h.jpg)

9. Once you're there make sure click on `Configure audio playback sources` 
![enter image description here](https://imgur.com/b5KEKmo.jpg) 

10. Under Audio Sources you will see the drop down menu is set to `JapanesePod101` by default

![enter image description here](https://imgur.com/2t0Kxhe.jpg)

click this and scroll to the bottom until you see `Custom URL (JSON)`

![enter image description here](https://imgur.com/smpfM6v.jpg)

once there you will be prompted to give a url. Please copy and paste `http://localhost:8770/?expression={term}&reading={reading}` into it. Don't forget to click the Add button on the bottom right! 


 <br/>

At this point you should have Yomichan working such that you can hover over a word, hold shift over it, and click the microphone to heard the audio icon :) 

However, if you would like to integrate Anki with yomichan such that you can instantly add a word to a deck by clicking the green plus button there are a few more steps. If you are not interested in Anki integration then you're done -- go have fun immersing in Chinese! 

In case you are curious how to enable adding Anki [here's a guide I made that might help](https://github.com/alexkiani/yomichan-forvo-server/blob/mandarin/anki%20setup.md). I separated the files out so that people won't get too intimated when they click this guide :p 


<br/>

Hope this helps and happy learning! In case there's any issues or you just want to talk feel free to drop a comment or reach out to me via email: alex kiani 97 at gmail (just close the spaces).

Have fun!