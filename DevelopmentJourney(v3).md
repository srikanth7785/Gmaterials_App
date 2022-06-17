> :construction: WIP: these are just scrap words, needs modifications :construction:

Ok, let me start with a little motivation for myself.
1. Current UI sucks.
2. If it works, it works - isn't called 'working'.
3. It's not me who's using the app, think like a user.
4. Why settle for less, when a lot more can be achieved.
5. Use the framework upto it's limits, if not beyond.
6. Nothing is a question of how?, it's just a question of 'what' "exactly" needs to be done.
7. No need to reinvent the wheel, everything's just a Google search away.
8. I ain't no developer, if I can't write maintanable code.
9. It's not gibberish, it's just English. Literally, writing code is just like writing an English essay, organise everything structurally and sequentially. Now, what is gibberish? Exactly!

Well..well..well! that's enough said. This is how it's going.
___
### Observations on how app currently is -
Went through each and every single, little, minute corner of app. Starts noticing how much better it could/should have been. 

Nothing is aligned properly. All these days, Am I blind or what🙄 - Now, that justifies 1st point of my motivation🌝.

Took a pen and paper, drew roughly how better could it have been.

// TO DO: insert hand drawn home screen UI image here

A proper format and font size should be followed throughout. Man, Oh man! literally there are different font sizes everywhere. Have I really been that dumb back then😶. Well, atleast not anymore I guess. Orrr am I still ?🥴.
Anyway, Coming back,..that's one thing that should be changed. For god's sake, I'm sticking with 3-5 different sizes, as needed.
___
Why did I use all those icons, they just make it look more congested. And they are unnecessary, atleast, not necessary.

// TO DO: insert current Branch details screen image here.

Point Noted. Just remove them, atleast, "not necessary" ones. Done. It's one step towards better now.
___
The core functionality of Gmaterials is to download materials. And, yeah, I should say, I did a good job here(emphasis on goooood. yeah, after all the <i>motivation</i> I started with, it's kinda needed😅). May be I'm not <i> that </i> dumb after all. But wait.. ** drums roll ** .. here comes a button which isn't functioning as expected. Really? Now!! Guess, that is why there are jobs specifically for testing.
> Inner me:
> What do you think all these days..that they just have lot of money to give away? You <i>dumb</i>!! (No emphasis here please 😬)
___
Ok, let me admit. These ads may be, may be..again, maayyy beee..litttlleee annoying. Can understand. But, guess what? I don't get those on my device. Well, I wrote the code after all. So, I can just comment few lines and make a custom one for self..right!😅. Also, on a serious note, One other Admob account of mine is blocked on the grounds of suspicious traffic as I used direct ad unit IDs instead of test ID which projected it as if I'm bringing the traffic intentionally when I'm just testing it during development. So, that is also a reason for me to make a custom app.

// TO DO: Insert `Test Ad` image here.

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
>motivation #2 kicks in..😏 <br>
>2. If it works, it works - isn't called 'working'.

So, how is it?...well, for starters, there are no models in place..didn't write any custom functions for widgets.. didn't break into individual components..no state management used.. literally, there are 5-6 screens in app and there are same number of files in `lib` folder😬 everything is written inline, just like an English paragraph😶. To give more context, once have a look at [Web_scrapping_with_flutter](https://github.com/srikanth7785/Web_Scrapping_with_Flutter) repo which demonstrates the `G-Events` feature. But, guess how it's implemented in current code.
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
<center> __ <br> <br></center>

>as motivation #8 says..<br>
>8. I ain't no developer, if I can't write maintanable code.
Hhmmmmm... so, that's a lot of work needed here. And a lot of brainstorming needs to be done. Ok, kinda fills the plate already, let's see what else is waiting in store.
___
Ok, that's enough observations on current one.  Let's start the new one 👀

So, bullet points, to-do:
* Current UI sucks - coming up with better UI👽
* Code Structuring - killing my brain already🧠
* Uniform font sizes - check✔️
* Remove "not necessary" icons - congestion free
* Nothing's aligned properly - Noted, take care of this!
___

> been off for a while, fell sick. getting back with double energy!!🥳

### Home Screen -

started working on the new design that I drew. looks good, for now atleast!

> So, how did I come up with this UI?

looking back to current version, what makes the current home screen 'not good' is that it is having nothing but the titles of differenct branches like `Computer Science and Engineering`, `Information Technology` and 3 other branches making a total of 5. but, It is just like filling up the space with big font and using large `Container`s. yeah, it sucks. 

so, ❗❗ NO LARGE CONTAINERS ❗❗ NO BIG FONTS ❗❗ DON'T JUST FILL THE SPACE, UTILISE IT ❗❗

<!-- ok, so, the new one is far better I feel. done. nice! -->

So, lets see what's needs to be there on an home screen?

In current version, there's no backend. but, as I'm planning to use Firebase as backend in the new version and with that also the Google SignIn. there's should be some user information shown on the home screen.

So, the top part of screen can have user info and can say 'hi' to user or some kind of welcoming message.

>Nice. that makes a lot of sense.

next - 'NO LARGE CONTAINERS'

but, how can I do that? remove those large containers and made them as small buttons with just `CSE`, `IT`. that's much better. No one really want to see all those abbrevations on the screen anyhow. - Cool.

It leaves much empty space below. should come up with something to fill the space which should also be contextual and should fit into the place. not to forget that as this being the home screen, that thing should be something that user is looking for on the home screen..soooo...what is such a thing!!???

well..let's think clearly!

* why a user opens this app? <br>

what else, for materials! either to download or to open the downloaded ones. <br>

nice. so, there's the answer!<br>

well, to download the required materials, user have to go the concerned screen and hit download. nothing can be done about it. so, what else's left? something can be done related to downloaded materials. like, user wouldn't want to go to the concerned screen every time and open the material even after downloading it right! so, there's should be a dedicated screen for the downloaded materials which already exists in the current version of the app. but, it could be further extended to make a mini version of it. like, say, there're only 2 or 3 downloaded materials in which case a dedicated screen isn't really necessary. right! also, like, when a user downloads a material it is most likely that the user is going to need/use it more than others in the near future.

> enough rambling! come to the point man!....yeah, so, here it is.

there can be a `Recent Downloads` section on the home section which has the 4 or 5 recently downloaded materials and user can access them from the home screen directly.
> that seems to be a good idea. contextual too !!

but, before getting the hopes high, can it be achieved? like, can I code it?

> motivation #6 #7 to the rescue! <br>
> 6. Nothing is a question of how?, it's just a question of 'what' "exactly" needs to be done. <br>
> 7. No need to reinvent the wheel, everything's just a Google search away.

<i> Wow!! 💥 I'm motivated 💥 I already feel like I know the the solution. let me put it into words</i>

 well, there's an `OfflineMaterials` db with all the necessary details,
 ```SQL
 CREATE TABLE _tableName(
    MODULE_ID TEXT PRIMARY KEY,
    MODULE_TITLE TEXT NOT NULL,
    SUBJECT_TITLE TEXT NOT NULL,
    FILE_SIZE TEXT NOT NULL,
    ...
    few more such columns
    ...
 )
 ```
 that needs to be maintained anyway, for the dedicated `Offline Materials` Screen. so, we would just need to tweek it a little bit and have one more column added to it which will maintain the order of downloads. so, what changes are needed? let's see.

 ```SQL
 CREATE TABLE _tableName(
    SEQ_NO INTEGER AUTOINCREMENT, -- New column to track the downloads order.
    MODULE_ID TEXT PRIMARY KEY,
    MODULE_TITLE TEXT NOT NULL,
    SUBJECT_TITLE TEXT NOT NULL,
    FILE_SIZE TEXT NOT NULL,
    ...
    few more such columns
    ...
 )
 ```
 
 So, adding a new `SEQ_NO` column, also making corresponding changes at all places needed, did the thing and it can now give the downloaded materials in the most recent ones first. like this,
```dart
foo([int top = 9999]){
    await db.query(
        _tableName,
        orderBy: '"${_cols.seqNo}" DESC',
        limit: top,
        );
    }
```
with this, when we can get the 4 or 5 most recently downloaded ones to show in the `Recent Downloads` section with `foo(4)` and can get all the downloads in the dedicated screen with just `foo()`. Nice!

> haven't implemented offline db at this point yet. so, as of now, it works theoritically!

So, now there's no complaint of empty space on the home screen. all the space is utilised. well, 'properly utilised'. so to speak!

No large containers. no empty space. not big font size used. looks just fine!

// TO DO: insert new home screen image.

-- done with home screen, UI part. --

### Subject Details Screen -


...... To be continued......

