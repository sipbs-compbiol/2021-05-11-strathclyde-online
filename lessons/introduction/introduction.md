# introduction.md - 2021-05-04-strathclyde-online

**START THE SLIDES**

-----

## WELCOME: Who Are Your Instructors?

- Well, there's me - Leighton Pritchard. I'll be teaching the `R` lesson on data management and visualisation.
- I'm a computational biologist
  - My research is entirely computational. I spend my days programming, analysing data, and working out how to make mathematics and computers represent biology more accurately
  - I've been programming for about 40 years, since the ZX81 came out and one of my schoolfriends' elder brothers got one.
    - I got a ZX81 in 1981, taught myself how to program in BASIC, and have been learning about computers ever since.
    - There are always new languages, techniques, and tools coming out.
    - I've never reached the end of any topic in computing - I'm always still learning how to code.
  - I've been a Carpentries instructor for about six years
    - I've taught across the UK, to groups of mathematicians, musicians, librarians, biologists, physicists, social scientists, and anyone else who is interested
    - I really like teaching the `R` lessons, because learners can get from never having programmed before to reading, cleaning, and generating complex visualisations of data in under a day.
    - I especially like how learners can go away with a new intuition and understanding of how to get computers to take the hard work out of data management and analysis. It's a really empowering skill, and it's great when I see their work later, and it's got cool data analysis in it.

- Your other instructor is Steve Ford
  - Steve, would you like to introduce yourself please?

- And we could not teach this course at all without the helpers, who are giving up their time to assist you on the course today.
  - Please would you all like to introduce yourselves:
    - Emma, Angelika, David, John, Alemao, Darren
  - The helpers will be your first point of contact throughout the day
  - If you have questions or issues, one of these kind people will be on hand to answer your questions, and keep you going through the course

-----

## WELCOME: Prerequisites

- So what are we expecting of you, when you start this course?
  - We **do not** expect you to have *any* previous programming knowledge
  - We will be taking you through as though you are new to the subject
  - We **do** expect you to have installed the required software before you arrived
    - If you have not done this, please raise your hand in Zoom and a helper will assist you
  - The software you need for today is:
    - `git bash` (if you're on Windows - if you're *not* on Windows you can use a terminal window)
    - `RStudio` and `R`
    - a text editor (**NOT WORD!** - you need an editor that saves plain text, like `notepad++`; you *can* use `RStudio` for this)
  - For tomorrow's session, you will need to install `OpenRefine` on your machine

-----

## WELCOME: EtherPad

- I've mentioned the EtherPad a few times already, but what is it? and where do you find it?
- The EtherPad is like a Google Doc
  - It's a shareable, online document in the cloud
  - We can all edit it, live and simultaneously
  - There is a link to it from the course webpage

**DEMO COURSE WEBPAGE AND LINK**

- We ask you to use this for a few reasons
  - It's a way to all interact together, even while physically separated over Zoom
  - You can take communal notes
    - It's fine to take personal notes, but *your insight* might be the missing link for someone else to get what's going on. So we encourage you to share your note-taking in the EtherPad
  - You can pose questions
    - This is particularly good for questions where the answer might help a lot of other people
    - Anyone can answer, not just instructors and helpers
  - The link persists after the course. You can return to your notes at any time.

**INVITE STUDENTS TO INTRODUCE THEMSELVES ON ETHERPAD**

- Please add your name to the EtherPad, and next to it put
  - one word to describe your research
  - one thing you made that you're proud of

-----

## 2. SCHEDULE

-----

## SCHEDULE: Timetable

- The overall schedule is on the course website 
- **OPEN SITE**
  - [https://sipbs-compbiol.github.io/2021-05-04-strathclyde-online/](https://sipbs-compbiol.github.io/2021-05-04-strathclyde-online/)
  - This has the timings, and also links to slides and notes that we'll be using.
  - Please do follow along with the material on your own machine, if you want to - or download them for reference later

- The overall timetable is this:
  - This morning Steven will be teaching the Unix Shell
    - This is meant to empower you to use the computer to automate repetitive tasks, and demystify some of the "hacker" stuff you might have seen in things like *Mr Robot*, or *Sneakers*
  - In the afternoon, I'll be teaching the first part of the `R` course
    - We'll be covering how to work with and represent data in `R` so that computational analysis is made much easier and more reproducible
  - Tomorrow morning, Steven will teach data cleaning with OpenRefine
    - This uses a different tool for exploring, summarising, and cleaning tabular data reproducibly
  - And finally, tomorrow afternoon I will present the second part of the `R` course
    - This will move into publication-quality data visualisation and - if we have time - analysis using R notebooks

-----

## SCHEDULE: Lesson Structure

- Each of the four lessons lasts around three hours
  - Because Zoom is really tiring - for all of us - in long stretches, we're going to try to break things up into three 45 minute sections, with a 15 minute gap between them

- You'll also get an hour for lunch

- You can get in touch and ask questions at the breaks
  - If you have long, involved questions, it might be best to ask these in the breaks

-----

## SCHEDULE: Workshop Roles

- We're each of us here with a particualr purpose, today
- You guys, the learners, are all here to get as much out of the day as you can
  - We expect you to code along with the lessons, try the exercises, and **ask questions**
  - You're here to be empowered by learning a new skill; we're all here to help you, so please don't be shy to ask
  - We also want you to share your own knowledge and perspective on what we do today.
  - So please do talk in the chat, and on EtherPad. If you've got a cool solution or find an interesting link - share it with everyone

- Me and Steve, as instructors, have prepared the teaching material for today and will be leading you through it
  - We'll be doing this mostly by **"live coding"**
    - You'll see our screens, and we'll work through the material, explaining as we go.
    - We'll make mistakes, but that's all part of it.
  - This works best when you guys all code along with us.
  - If we're going too fast or too slow, let us know

- Our helpers today and tomorrow will be your personal guides, to some extent.
  - The helpers will be monitoring the Zoom chat and EtherPad, ready to help answer your questions and sort out your problems.
  - They're the most critical part of Carpentries teaching - without the helpers it's just like watching a video. The helpers are the magic secret sauce.

-----

## 3. HOUSEKEEPING

-----

## HOUSEKEEPING: Code of Conduct

- We're all here to provide a comfortable, friendly, safe, respectful, and effective learning environment for everyone
- To help with this, there is a Code of Conduct for Carpentries courses, which you can find on the Carpentries site
  - it is linked from the Etherpad, and the course page

- As you might expect, it more or boils down to "don't be a dick."
  - If you have any doubts about what that means, then the Code of Conduct is quite detailed about it.

- There is an incident respose procedure and, if you have any issues or concerns that might be Code of Conduct violations, you can contact me, Steve, or one of the helpers, and we'll take it forward

- If we're the problem (and I hope we're not), then there are two direct emails to the Carpentries organisation you can use
  - The `coc` email is seen by all the Code of Conduct committee
  - The `confidential` email is for confidential reporting

-----

## HOUSEKEEPING: Help

- Learning online is quite different from the face-to-face Carpentries sessions
  - In-person, the helpers would be in the room, and you - the learners - would indicate you needed some advice by using post-it notes
  - That won't work here

- If you need immediate 1:1 assistance, please **raise your hand in Zoom**
  - A helper will be monitoring Zoom for this, and try to direct a helper to you as soon as possible
- If you don't need immediate 1:1 assistance, but you have a question *for now*, **please put it in the Zoom chat**.
  - A helper will be monitoring, and should get you an answer quickly
  - Or another learner may answer it for you - that's also great!
- If you've got a more general question, or a longer question, **please put it in the EtherPad**
  - A helper (or maybe a learner) will give an answer
  - These questions/answers can then be used to help other learners who might have the same issues

-----

## HOUSEKEEPING: Feedback

- We have a favour to ask you, as learners
- We really need your feedback
  - This is how we improve, both as teachers in general, and in delivering this specific material
  - You are the best judges of how we're doing; you're getting the material as it is now, from us as we are now
  - You can tell us what is working well, and what isn't
  - That may help tomorrow, but it will certainly help future learners

- We want two kinds of feedback from you
  - First, we have a Qualtrics survey after each lesson.
    - We're asking each of you to please tell us one thing about the lesson that went well, and one thing that could be improved (and how, if you've got an idea of how...)
    - We'll put the links on EtherPad at the end of each lesson
  - Secondly, there's a Carpentries online survey that tells the main organisation how we did.
    - There's a link to this on the course website

-----

## 4. LET'S GET STARTED