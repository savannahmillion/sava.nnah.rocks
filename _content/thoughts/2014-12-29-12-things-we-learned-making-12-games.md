---
title: 12 Things We Learned Making 12 Games
_template: thoughts-lp
blog-img: {{ homepage}}assets/img/projects/12games/santa-face.png
emoji-animation: about-face
---

<p class="small center">* due to the intangible nature of learning, bulleted content may not numerically add up to the actual number "12", but we thought the title was catchy and can assure you we definitely learned a lot.</p>

<p class="center"><br>by Savannah and David</p>

##<br>GitHub Collaboration

Savannah: This was my #1 favorite thing to have picked up through Twelve Games. Before this project, I had yet to have a real need for a version control tool, but I knew it was a valuable skill for developers to have and wanted to learn it. I'm now really comfortable using git in the command line and I'm consistently using it for my personal site, too. Going to that chart of github activity on my profile and seeing the little gray squares get progressively more and more green is both satisfying and addicting.

##HTML, CSS and the Web Development Pipeline
David: I can't tell you how many times I'd go to W3schools and try to build something in HTML and CSS. It would always end with me having a few scattered paragraph elements and getting frustrated with CSS and stopping. I had never learned about having a normalize CSS file or anything like that, so when Savannah told me about it I was pretty pissed. WHY IS THIS NOT THE DEFAULT IF EVERYONE USES IT? UGGGGHHHHHHH. Regardless, the minor amount of web development exposure I had (uploading files to a webhost, tweaking some HTML or php files here and there, etc.) prior to this project didn't really give me a solid understanding of the pipeline/workflow for how it all comes together. Even though Savannah built the whole site, I feel much more comfortable with front end web development now!

##PHP Includes & .htaccess
Savannah: I've used CMSs before that utilize php and was familiar with what php does, but I'd never had a reason to write it before now. I've been working on projects through MAMP for a while, so I was happily surprised that writing a php include was literally as simple as it sounds. Same with .htaccess files &mdash; although I've edited existing ones, never had to create one from scratch. (I ended up copy + pasting one from somewhere else, so that's not exactly creating one from scratch is it?) In this case I only used it to make the urls pretty, but I learned .htaccess files can actually do a lot more than that. You can see my super simple, barebones, copy + paste .htaccess on the [github repo.](https://github.com/savannahmillion/Twelve-Games/blob/master/.htaccess)

##Learning Javascript (syntax, integration, and browser support)
David: I had never worked in a purely javascript environment before. I mainly work in C# and C++ so there were many things about javascript that threw me off. I had used similar languages before (such as Unity's UnityScript) but not extensively and definitely not on web.

I'm a stickler for type declaration in languages, and while some argue that using 'var' for everything helps developers form good variable naming habits I don't think that outweighs the benefits of allowing explicit type declaration. This annoyed me for a bit (I would frequently get syntax errors for declaring for-loops with 'int i = 0' instead of just 'i = 0') but I eventually got over it. I still prefer explicit type declaration ;)

One of the harder lessons I learned was to write code that would work in most-if-not-all browsers. For some of the games, I wanted to avoid creating unnecessary global variables and write functions that could yield/maintain data within a local scope. I stumbled upon generators, which emulated that of coroutines (Unity makes heavy use of these). It was exactly what I needed, but apparently generators aren't officially part of javascript yet. It wasn't until I had already finished game 2 and started working on game 3 that I realized my use of generators was the reason that the games didn't work on mobile browsers. I ended up having to rebuild the entire game with much nastier code. If you go through the source for game 2, I'm sorry.

It also took me a while to stop brute forcing my logic and learn to create classes within javascript. While the ultimate goal was to make the games work, I wanted people to be able to use these games as a learning resource. If you go through the source in order (game 1 - 12), you'll see the code is much less scattered and, in my opinion, a bit more organized. I tried to consolidate as much global functionality in a common.js file, though there are still a few things that ended up being reimplemented every time (such as the Naughty/Nice dropdowns...I could have consolidated that code too :P).

Overall, I feel pretty comfortable with javascript now and look forward to building future projects with it!

##Sticky Footers
Savannah: This was an enormous headache. I wanted an illustrative footer for Twelve Games, to balance the heavily illustrated top navigation. I've always found coding sticky footers to be a big pain (especially when they have a solid/contrasty background and it's super obvious when they are a pixel off) but figured this was a good time to get acclimated with them. I referred to this [CSS tricks article](http://css-tricks.com/snippets/css/sticky-footer/), which is extraordinarily simple, and got the footer to act the way I wanted it to on every page except the home page for the longest time. Turned out I was having margin/padding issues. It was a huge relief when I finally diagnosed that problem. My sticky footer game is now stronger than it was. I feel good about this.

##Designing for Mobile and Desktop
David: Initially Savannah and I decided we would focus on the games working on desktop only, but still have the site be responsive. I ended up having a bit of extra time, so I did my best to make the games feel good to play on mobile as well. This usually didn't take too much extra effort, and ended up being a really good idea considering analytics showed most of our visitors and players were on mobile. A few of the game designs ended up changing slightly in order to accomodate a mobile control scheme, but none of our original ideas were necessarily compromised by supporting touch input.

##Debugging for Web and Mobile
David: I worked in Firefox and Chrome when testing on desktop, and I used Safari on my iPhone when testing the games on mobile. The error reporting for javascript can be a little vague, but by the end of the project I learned to properly interpret some of the quirks and recognize what was really causing errors.

As for debugging on mobile devices, Safari has a nice feature where you can enable mobile debugging and get the console log from your mobile safari browser to show up on your desktop. It helped me identify a lot of the issues particularly related to touch input and mobile browser support! I'm sure other browsers have similar tools, I just happened to find this one first and it required no effort to set up.

##Making Really Tiny Games isn't as Easy as I Suspected

Savannah: One of the trickier parts of this project was coming up with so many seriously tiny games. Pretty early on I started referring to them as "interactive art" because I wasn't even sure they could fit the definition of the word "game." (Whatever, they're games.) Since we only worked on the entire thing for ~1 month, we could only sink a few hours into each game, which usually meant that after brainstorming ideas and before rendering assets we had to seriously lower our scope. So much of the project became stripping away game ideas to their most simple, feasible core. Much respect to all of the game devs that participate in game jams &mdash; having time as a limited resource is quite the challenge.

 &#9813;