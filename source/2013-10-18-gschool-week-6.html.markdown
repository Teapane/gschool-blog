---
title: gschool -week 6
date: 2013-10-18 14:53 UTC
tags:
---

 This week marked the beginning of building web applications.  We moved on from building command line applications to actually utilizing the Ruby we have learned to build a web application, via a tutorial titled IdeaBox.

 The basic premise of IdeaBox is to build a web application that can store ideas in a database, and then these ideas can be searched for, grouped by attribute, etc.  In order to accomplish this goal we are learning how to utilize Sinatra.  From what I have learned so far, Sinatra is like Rails little brother.  Since Sinatra is built on Ruby, a lot of the syntax is familiar, but the concepts are rather different.  By this I mean we were sort of thrown into the web and multiple languages: Ruby, HTML, CSS, Javascript, etc.  

 Going through the tutorial was rather monotonous and dry.  The material was interesting but I felt like I wasn't really grasping all the things I was doing; it was more of a read and copy the code into my editor. I got through the tutorial rather quickly, but when it was over I wasn't entirely sure of what I had done.  It worked, I could view the webpage when I ran a local server, but I didn't know why. 

 This is not a comfortable feeling. This was not a good place to be in I thought.  So what to do you ask?  Well start over of course.  I went back through the tutorial, this time utilizing testing, and really tried to understand what I was doing.  The second time around I felt a little more comfortable with what I was doing, and was really starting to look at the code to understand what it was doing.  However, I was still a little bit lost; luckily, on Thursday night I had the opportunity to pair with my mentor Austen Ito.  This mentoring session could not have come at a better time. 

 I sat down with Austen (via screenshare, he does live in NYC) and started to look over the code.  Through our three hour session I really started to get an understanding of what the code was doing and it was a really great feeling.  By refactoring some of the pre-existing code I really started to understand why the code was there.  It was really satisfying to do this.   

 So now we are on the web.  We are building things that aren't command line dependent and it's really cool.  The biggest difference, for me at least, is setting up the testing environments in Sinatra.  When we were building command line apps, the testing was static; now, the testing needs to account for the constant change of state of the web application.  This concept to me was really confusing and difficult to set up.  I couldn't understand why my tests were expecting 1 as a result but kept returning two, then three, then six, and so on and so forth.  Each time I was loading the server, more and more data was going into the database and I couldn't understand why my tests kept failing over and over.  This lead me to figure out the whole idea of environment.  

 Setting up environments in test suites is crucial because it allows you test the functionality of the web without actually creating new data in the database.  This lead me to utilize such ideas as teardown(I had been using setup so frequently in tests so this inverse operation of teardown made sense) and setting up ENV['RACK_ENV']= "test".  I am still a little shaky on how this all works, so it is certainly something I will need to keep teaching myself about in order to really understand; but, my tests are working and that's pretty sweet.  

 I have felt really good about how this week has gone so far.  Focus week was really helpful in letting me step back and try to understand everything that was going on.  I feel like I gained a lot last week by going over topics again and trying to understand them.  It was a refreshing week and I felt like it prepared me well for this week and the new project, especially because we are doing this project solo.  

 On Monday when the project was assigned, we were told to work independently but we were also assigned small groups that we could utilize for help.  I got an awesome group :Rolen, Will, and Meeka. These three are all total rockstars; it has been really nice to have them for help and they are always more than willing to lend a helping hand.  It is however a little intimidating to start a project alone.  I thought I knew more than I actually do and I am starting to really realize this.  

 So here I am, trying to do a project on my own and it is really putting into perspective my level of understanding of the material.  I feel like I know enough to make things work, but I really want to understand more and be able to do more on my own. Also, considering there is an assessment on Monday, I need to really sit down and evaluate my understanding and try to pick apart what I am shaky on and were I need to improve.  

 I am nervous for the assessment; I mean, why wouldn't I be?  But I also feel like I shouldn't let it stress me out. I can only do so much, but I think it will be nice to put into perspective what I do know and what I don't.  I don't really think there is a good way to prepare for it other than just doing what I am already doing.  I have a solid understanding of setting up directories, creating test suites, and writing some code that works, but may or may not be pretty


