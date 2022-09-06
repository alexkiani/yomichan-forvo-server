
Hey! This is a guide to show you how to integrate Anki card adding with Yomichan, particularly for Chinese cards. 

For anyone that's an absolute Anki beginner check out [this quick read](https://docs.ankiweb.net/getting-started.html#key-concepts) on the key concepts of Anki. 

This guide assumes you're a first time Anki user and starts from the ground up, but don't worry if you're an Anki pro -- I'll let you know exactly when and where to skip around ;)


1. First we need an Anki deck to put your Yomichan cards in. If you already made a deck or have a deck where you wanna store them feel free to skip this step!

     
     ![enter image description here](https://imgur.com/Us42sNE.jpg)

Name the deck whatever you'd like. For simplicity's sake I'm calling mine yomichan

![enter image description here](https://imgur.com/K4oO39b.jpg)


2. Now we need to create a note type that's specialized for yomichan. Go to Tools -> Manage Note Types
	![enter image description here](https://imgur.com/OW7uVOm.jpg)


<br/>
Now Click Add -- don't worry if your Note Types is empty or looks nothing like mine. 

![enter image description here](https://imgur.com/zOocOfk.jpg)

Now with `Add: Basic` highlighted click Ok

![enter image description here](https://imgur.com/QLoY7iv.jpg)

Again, name this note type whatever you want. I'm calling mine yomichan once more.

   ![enter image description here](https://imgur.com/xOmd50B.jpg)

3. Now that we created a note type for yomichan, we need to edit it so that it's Yomichan ready. Once Again go to Tools->Manage Note Types. This time click on the note type you created, it should have [0 notes] and click `Fields`

![enter image description here](https://imgur.com/YsImSVV.jpg)

Once you're there, you'll notice that there's only two fields: Front and Back. Click `Add` and add in the fields of Audio, Sentence, and Pinyin shown below. Don't forget to hit `Save`!

![enter image description here](https://imgur.com/luYqn98.jpg)

4. Now with the fields added we need to edit the cart format themselves so that they show up in a nice way. Once more, back to Tools->Manage Note Types click your card type and hit `Cards` this time

![enter image description here](https://imgur.com/a5nksT5.jpg)

Once you're there you'll see a box in the left hand side where you can paste html code. Don't worry if your box looks nothing like mine, I'll give the code you need to copy in. There are three templates we need to paste in: Front, Back, and Style. Please copy in the following for each one -- once again don't forget to save when you're done!

Front:

`<div style='font-family: BIZ UDGothic; font-size: 48px;'>{{edit:Front}}</div>`
<br/>
Back:

    <div style='font-family: BIZ UDGothic; font-size: 48px;'>{{Pinyin}}</div>
    
      
    
    <br>
    
    <div style='font-family: BIZ UDGothic; font-size: 24px;'>{{edit:Sentence}}</div>
    
      
    
    <hr id=answer>
    
    <div id="autoplay" style='font-size: 36px;'>{{Audio}}</div>
    
    {{edit:Back}}
    
    <br>

<br/>

    Styling:
    
    .card {
    
    font-family: arial;
    
    font-size: 20px;
    
    text-align: center;
    
    color: black;
    
    background-color: white;
    
    }

4. Onto the last step! Go back to the Yomichan settings page, to the Anki settings

![enter image description here](https://imgur.com/lfUDbd9.jpg)

Once there hit `Configure Anki card format`

![enter image description here](https://imgur.com/VlhhyXY.jpg)

Now here we can have a little customization with how we want our cards to look. First of all, make sure that your `Deck` matches the name of the deck you want your yomichan cards to go into and your `Model` is the card type you made. 

Regarding the fields, at a minimum fill out the `Front` , `Back` , and `Pinyin`fields like I have below. Don't freak out that `Pinyin` is labeled `{furigana}`, that's just yomichan's way of adding in the text that goes above hanzi/kanji.

If you don't want an audio pronounciation of the word in your deck, leave `Audio` blank. Same with `Sentence` if you don't want the scentence where you read your word to go into the card you're making. 


<br/>
And you're done! Thanks so much for reading this guide and I hope you have a ton of fun immersing yourself in Chinese or any language you like :D 

If you have any questions feel free to drop a comment or reach me at:

alex kiani 97 at gmail  (just close the spaces)

Happy learning!