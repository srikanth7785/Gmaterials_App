> :construction: WIP: these are just scrap words, needs modifications :construction:

Ok, let me start with a little motivation for myself.
* Current UI sucks.
* If it works, it works - isn't called 'working'.
* It's not me who's using the app, think like a user.
* Why settle for less, when a lot more can be achieved.
* Use the framework upto it's limits, if not beyond.
* Nothing is a question of how?, it's just a question of 'what' "exactly" needs to be done.
* No need to reinvent the wheel, everything's just a Google search away.
* I ain't no developer, if I can't write maintanable code.
* It's not gibberish, it's just English. Literally, just like writing an English essay, organise everything structurally and sequentially. Now, what is gibberish? Exactly!

Well..well..well! that's enough said. This is how it's going.
___
### Observations on how app currently is -
Went through each and every single, little, minute corner of app. Starts noticing how much better it could/should have been. 

Nothing is aligned properly. All these days, Am I blind or what🙄
Now, that justifies 1st point of my motivation🌝.

Took a pen and paper, drew roughly how better could it have been.
% alt_text: image_here %

A proper format and font size should be followed throughout. Man, Oh man! literally there are different font sizes everywhere. Have I really been that dumb back then😶. Well, atleast not anymore I guess. Orrr am I still ?🥴.
Anyway, Coming back,..that's one thing that should be changed. For god's sake, I'm sticking with 3-5 different sizes, as needed.
___
Why did I use all those icons, they just make it look more congested. And they are unnecessary, atleast, not necessary.

Point Noted. Just remove them, atleast, "not necessary" ones. Done. It's one step towards better now.
___
The core functionality of Gmaterials is to download materials. And, yeah, I should say, I did a good job here(emphasis on goooood. yeah, after all the <i>motivation</i> I started with, it's kinda needed😅). May be I'm not <i> that </i> dumb after all. But wait.. ** drums roll ** .. here comes a button which isn't functioning as expected. Really? Now!! Guess, that is why there are jobs specifically for testing.
> Inner me:
> What do you think all these days..that they just have lot of money to give away? You <i>dumb</i>!! (No emphasis here please 😬)
___
Ok, let me admit. These ads may be, may be..again, maayyy beee..litttlleee annoying. Can understand. But, guess what? I don't get those on my device. Well, I wrote the code after all. So, I can just comment few lines and make a custom one for self..right!😅. Also, on a serious note, One Admob account is blocked on the grounds of suspicious traffic as I used direct ad unit IDs instead of test ID which projected it as if I'm doing it intentionally when I'm just testing it during development. So, that is also a reason for me to make a custom app.

Anyway, basically..it's working good. And those aren't frequent or nothing like, just pop-ups on screen. It's purely contextual and occasional. Nice!

So, no changes needed related to Ads.
___
Let's talk about how the app is structured code-wise.

** <i>Spoiler alert!! This part adds to the motivation at beginning😐</i> **

It sucks!! That's it..just two words!! <i>It's horrible</i>..two more words..<i>it's pathetic..</i>
Ummm..no, it's not enough..just twoooo more words..
<i>💥 it's dumb!! 💥</i>. Yeaaahhh, I kinda had to say that.

Ohhh mmmyyy goodnessss!!!! I'm really thankful to god that it's working fine at production level and people rated it at `4.7/5.0`. Had those people seen this code, I wouldn't wonder if they don't even want to consider giving 0.3. Yesss, it's that bad. 

But..well, it's working..right!
>Remembering motivation #2 😏
> >If it works, it works - isn't called 'working'.

So, how is it?...well, for starters, there are no models in place..didn't write any custom functions for widgets.. didn't break into individual components..no state management used.. literally, there are 5-6 screens in app and there are same number of files in `lib` folder😬 everything is written inline, just like an English paragraph😶. To give more context, once have a look at [Web_scrapping_with_flutter](https://github.com/srikanth7785/Web_Scrapping_with_Flutter) repo which demonstrates the `G-Events` feature. But, guess how it's implemented in app?
```dart
.
.
InkWell(
    child: child, //UI stuff, again inline😐
    onTap: (){
        // Whole code from [Web_scrapping_with_flutter](https://github.com/srikanth7785/Web_Scrapping_with_Flutter) 🙄
    },
),
.
.
```
     
> Objection from past me! 
> * No models used? Not really required. Well, it would have been good had they were used..but, kinda not necessary.
> * No state management? Absolutely, not necessary. We shouldn't have something just for the sake of having it. right! So, yeah.
> * Everything inline? Well, It was written in 2019. So, kinda rookie thing. Like, okay! But, heyy..not anymore. Change it now!!! Ok, noted.
> * No components? About `lib` folder? *** Out of sight!! ***    Didn't hear about `G-Events`🤫

Hhmmmmm... so, that's a lot of work needed here. And a lot of brainstorming needs to be done. Ok, kinda fills the plate already, let's see what else is waiting in store.
___
Ok, that's enough observations on current one.  Let's start the new one.

So, bullet points, to-do:
* Current UI sucks - coming up with better UI👽
* Code-wise - killing my brain already🧠
* Uniform font sizes - check✔️
* Remove "not necessary" icons - congestion free
* Nothing's aligned properly - Noted, take care of this!

...... To be continued......

