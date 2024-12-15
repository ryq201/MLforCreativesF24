# Final Project
## “Synesthesia” Music Box

“A music/jukebox that is played through a submitted drawing”

My final project changed a decent amount from original idea to final product. Originally, I was inspired by my harmony project from Code of Music where I used a user’s drawing to trigger different chord progressions, and following some class feedback, felt that the idea of interpreting the drawings in more depth could be used on a much greater scale for making music. I began to think of all the different aspects of a drawing that could be analyzed, such as color, line weight, angle, etc. and how it could be used to remix or generate a track. During that same week, we were experimenting with Transformers.js, and one example I took a particular liking to was Doodlenet, a classifier that could ID simple doodles. With these two ideas in mind, I decided to try and combine them, hoping to make a musical instrument that would observe and classify a drawing, and make an appropriate composition based off of that info. 

My initial research pointed in the direction of more functions related to Transformers.js, involving sentiment analysis as well as musicgen. These tools would streamline the process of analyzing a drawing. On the musical side of things, I began looking into the various ways a generated mp3 could be remixed in Tone.js. 

Originally, I thought the project could be for people who may not understand or know how to make music, so by letting a user draw something, they could generate their own. However, I think my project is for anyone who wants to draw or have fun. There are no underlying themes, just a simple pad that allows someone to draw something digitally, and music to make the experience more enjoyable after. 

However, this is where things started to kind of fall apart for this project. While Doodlenet and the drawing functions worked alright, Transformers.js was constantly either buggy, slow, or completely broken. After repeated trial and error as well as discussing it with Alan, I decided to give up and went the low tech route, which was simply hard coding the sentiment response and possible tracks. This was actually relatively simple to do, as Doodlenet provides a list of all possible terms, and with the help of Chat GPT, I could quickly generate a dictionary of all the terms and a correlating sentiment. 

On the music side of things, now with hard coded tracks, the app became more of a music box rather than a generator. However, I still implemented features to remix the track, such as line and hold length to control track speed, and using the erase tool causing the track to reverse. I had originally hoped to code something to convert the tracks into something easier for Tone to work with, thus allowing more remix-ability, but was strapped for time and had to leave it as is. 

Although I did not get a chance to user test my project outside of class, the demo session the class before was helpful in understanding the weak points from a user perspective of my project. I noticed that people repeatedly struggled to find the clear canvas button, as the palette, generate response, and eraser buttons were all grouped together at the bottom of the page, but the clear button was at the top. Another challenge I noted was that people got no feedback from the app when toggling on the eraser, meaning that they couldn’t tell if they were using a brush or eraser. I solved these issues by repositioning the clear canvas button, as well as making it more obvious that the eraser was a toggle by having the button get highlighted when selected. The cursor was also replaced with a brush or eraser depending on the mode to make it more clear which tool the user was actively using. 

The reference I was most dependent on was the original Doodlenet github page and p5 sketch. My project actually uses the original Doodlenet sketch as a base, and I built features onto that original sketch to fit my purpose. Other sources I used were the p5 documentation pages, as well as Stack Overflow and Chat GPT for miscellaneous code questions. The dictionary that uses all 345 possible responses from Doodlenet and ties them to a emotional category is the most notable contribution I got from Chat GPT. 

If I were to continue working on this project, I would definitely want to expand more on the music front. Better remixing and more variables of tracks, and more possible tracks period. AI generated tracks would be interesting, but I did experiment with those for a bit and thought they sounded atrocious. Nevertheless, it could be a path worth exploring further



Assets:
![eraser](https://github.com/user-attachments/assets/8b928021-4ea5-4a0f-ac5d-c2819a594025) ![brush](https://github.com/user-attachments/assets/ff6833c9-0025-49b5-9cf7-af127785a738)
