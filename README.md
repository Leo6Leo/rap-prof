## Inspiration
“OMG so many lecture recordings, I am so stressed!” “I have 2 assignments due this Friday and 1 quiz tomorrow. I have to watch all recordings tonight”

Are you worried about being unable to finish the 10 hours left behind lectures before the exam tomorrow? Are you annoyed when professors speak too slow and pauses too often during a lecture? Don’t worry! We’ve got the solution for you! We are caring for your mental health! No more stress!

Inspired by the problems described above, our team decided to create something that **automatically** removes the “redundant” part of every lectures -- the silence intervals in which the professor might be looking at chatbox / thinking / writing -- and then returns the edited version *online*. 

How much time does it save? Roughly estimated: 30%. Meaning a 120-minute- lecture is actually one and a half hour. In addition if the user plays the video at double speed, 72 minutes of our youth in total is saved!

## What it does

The webpage provides a form where the user could input an URL to a video, click on ‘Next’, then the video will automatically be downloaded to the server, in which the program will trim the video and remove the silent parts of the video. Then, the edited version will be returned and displayed to the user through an embedded video player on a separate webpage. Inside the video player, users could also use common functions like adjusting the playback speed, fullscreen and etc.


## How we built it

Framework: we used Django to set up the overall framework of our webpage and its server. For visual designs such as the motion background, we mainly used aspects of CSS such as @keyframes. 

Video-editing-program: we used ffmpeg first to get the silent part in the video and generate a txt file containing the timestamp of the silent part, and then sent the result to the  moviepy to cut the video. 


## Challenges we ran into

In the initial stages of building the silence remove program, we tried to implement and utilize existing open source libraries such as jump cutter and silence remover, but unfortunately both of them did not work on our ends(The cut video and the audio file were not synchronized). Therefore we had to manually program the video editing functionality. 

Another challenge was that after completing the program, we realized that the processing efficiency of this program was not meeting our expectations -- it takes quite a while to generate the edited video.

## Accomplishments that we're proud of

Being able to create a project in such a short amount of time was an experience never thought of before for some of our members (two out of three of us are first-time ‘hackers’). We’re certainly very proud of the webpage we made, the program we created.

However, in addition to that, being able to create something that is actually useful to the community and resolves real life issues are things we’re even more proud of, we hope in the near future we can continue to improve on this project, optimize the program better, and promote it to more people in need like us.

## What we learned

As our team mostly consists of members with few to little experience in web development (and even programming), this hackathon has provided an incredible gain to our knowledge of programming in the area of web development. It is hard to emphasize how much we worked and learned during these two days and the tremendous effort everyone put in to make this project possible.

A few of the things we learnt: 
How to use ffmpeg to detect sound time period and output the all data in txt file and then we use python to format and extract the silence_end time and silence_duration.

Thanks to the online tutorial made by Donald Feury, we really learnt a lot from him.

How to use the python library moviepy to edit videos (trim, combine, speed up and etc.)


How to use CSS to create an animated background and animated objects.
How to use bootstrap to create a navigation bar.

## What's next for Rapper-Prof
We are considering the reason causing the processing efficiency too low was the hardware of our own computer. We will focus on deploying our program on the cloud server, and continuously seeking any other methods to improve the efficiency. We will definitely continue updating and maintaining this program. Hope the hacker also interested in this program to join us!



Thanks to:

Ckplayer
https://gitee.com/niandeng/ckplayer

Donald Feury
https://dev.to/dak425/automatically-trim-silence-from-video-with-ffmpeg-and-python-2kol

Divinector (for animated background)
https://www.youtube.com/watch?v=5RoXCs54CN8&t=222s&ab_channel=Divinector

ffmpeg
https://ffmpeg.org/

Moviepy
https://pypi.org/project/moviepy/
