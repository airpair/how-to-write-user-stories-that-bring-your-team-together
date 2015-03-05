Software Development can be a messy, complex beast. Feature creep is always 
lurking around the corner, getting even a small team on the same page can feel daunting and communication can easily become muddied.  After working on teams for over 45 products I’ve become a strong believer in the value of using user stories to guide the development process. If you are an entrepreneur, developer or designer working on a new product or updating an existing application, user stories can give you and your whole team a great framework for keeping your project organized, cohesive and focused.

##What are user stories?

I like to describe user stories as a detailed list of actions and objects associated with the features of an application. That’s a little dense so we’ll unravel it a bit.

The difference between user stories and features can be a bit subtle so let’s use something simple, a kitchen, to think through their relationship. Features describe the high level actions. The features of a kitchen could be:

- You can can wash dishes in a dishwasher
- You can store things in cabinets
- You can store perishables in a refrigerator
- You have counter space for prep work

User stories will take each of those features and break it down to detailed, lower level specifications. Let’s look at the feature ‘you can wash dishes in a dishwasher’. The user stories associated with this feature might be: 

- A user can open the dishwasher
- A user can close the dishwasher
- A user can add soap
- A user can set the timer

We would also include details about the dishwasher, which is an object associated with one of our main features. For example we might say ‘a dishwasher has and on off switch’, ‘a dishwasher has two shelves’, ‘a dishwasher has a tray for soap’, etc. The idea here is to be break features down into the necessary actions and objects until all of them have been thoroughly described. It may feel a little silly, like you are stating the obvious, but it’s this kind of granularity that will keep a software development project moving forward with intent and focus.

##Prework

Before you are ready to write user stories, you should have done a fair deal of Business Analysis work. Here’s a short checklist of questions that you should have answered already:

- Why are you making this?
- What are the business goals?
- What defines success for this project?
- What is your target market?
- What pain points are your solving for them or value are you adding to their lives?
- What are the technical & lifestyle trends among your target market?
- What platform(s) are you developing on?
- What is your budget?
- What is your timeline?
- Who are your competitors and how are you differentiated from them?

##Shut the door, have a seat

Before we begin with the steps to writing user stories I’d like to emphasize that this is a process that you have to spend some time with. You will not get a perfect or complete list the first time around so set aside time to revisit this document 2 or 3 times with your team. 

I  very strongly believe that user story creation is best done with not only the primary stakeholders for the project, but also, at least one UX designer and one developer. If you don’t have designers or developers lined up for the project yet, find some that you respect and pay them to sit down with you and help you think through your user stories. Having the right people in the room during user story creation could literally be the difference between the success or failure of your product. Don’t skimp.

Okay, so let's get started. I like to use a Google Drive spreadsheet for my user story doc as it’s easy to share and update. For the purpose of this article, I will be showing you the process using a simple meditation timer app that I built 2 years ago. 

##The 5 Step Process
###1. Write the Features###

So first we want to write out the main features of the product. You can be ambitious here. In an ideal world, what would it do? We’ll come back later with a reality check as to how many of these features we can actually build.
So for my mediation timer I’m going to say:

- You can meditate with a nice timer display
- You can save various meditation settings for future use
- You can track your total meditation hours
- You can share your meditations to social media

That feels pretty complete to me so let’s move on.

###2. Identify User Types###

This is an extremely important and often overlooked part of the process. The user types we are talking about here are not ‘a 90-year-old woman’, ‘a monk’, or ‘a 20-something hipster’. Those are personas. User types are classes that the app assigns to a user that determine which views and functionality the user will have access to (which permissions they will have). For example, we might have ‘visitor’, ‘basic user’, ‘admin’, ‘super-admin’ etc.
 
For the sake of my meditation timer I’m going to assume that I will be creating a native iPhone app. Therefore my user types will be:

- Meditator (anyone who has downloaded the app)
- Social user (someone who has connected a social account to the app)

It’s important to strive to find accurate and descriptive names for your user types. Don’t waste too much time trying to be clever, though. The most important thing is that everyone is clear on what the user types are and uses the same language to describe them. I also note when I have a hierarchy of permissions. For example stating that a ‘social user’ in my app has all the same permissions as a ‘meditator’ and can take all the actions a meditator can take.

###3. Identify Terms & Metaphors###

I’m alarmed how often I find myself on teams where the business team, dev team and design team are using completely different vernacular to describe the same thing. This quickly creates a tower of babel that can derail forward momentum and cause anywhere from minor to major miscommunications. To help clear this up we create a list of terms and metaphors associated with the product. Again, it’s important to find accurate and descriptive terms but don’t get into a time suck with trying to be overly clever.

So for my meditation timer I have:
- Session (an instance of a meditation)
- Clock (the clock displaying my time remaining)
- Quick-use (my saved settings for a session [I'll note here that this word seems awkward, I’ll come back later and try to make it better but for now I move on])
- History (history of my sessions)
- Session summary (a summary of an individual session)
- Stats page (a summary of all my sessions)
- Share (posting a completed session to facebook or twitter)

When you first create this list, it will not be complete. I usually jot down 5 or 6 words and move on. Then, as I’m writing my user stories, I’ll bold terms that appear in each user story and add them to my list of terms & metaphors.

###4. Write the Stories###

Okay so now we dive in to actually writing the stories. I like to take it one feature at a time and one user type at a time, starting with the most basic, in my case, a meditator. I’ll put my features in the far left column of my document and then write stories in the second column. I expect to have several stories associated with each feature. Let’s start with ‘you can meditate with a nice timer display’. I don’t need social login to use this feature so all of our stories will be for a meditator. To create the stories, I think through what actions I would have to take to engage with this feature.

*You can meditate with a nice timer display*
- A meditator can choose a length of time for a **session**
- A meditator can choose an image to display during a **session**
- A meditator can choose to show or hide the **clock** during a **session**
- A meditator can choose a **bell type** for a session \*\(note that I don’t have ‘bell type’ in my list of terms. I will now go back and add it)

This is starting to look pretty good. I won’t go through all my features here but let’s look at the feature ‘you can share your meditations to social media’ so we can see how to switch user types.

*You can share your meditations to social media*

- A meditator can link their account to twitter and facebook *(you might note here that this is the action that turns a ‘meditator’ into a ‘social user’)
- A social user can share the **session summary** of any completed **session** to facebook and/or twitter
- A **session summary** includes date, time of day,  length of **session**, and **session** image *(note that this story doesn’t talk about an action like the others but talks about the attributes of an object that is related to this feature)

We would continue with this process until we felt we had all the user stories for each of our features. User story documents I encounter for a 3-12 month project generally ranges from 30-60 stories depending on the complexity of the product and the granularity of your document.

###5. Prioritize###

So now that we have a good list of user stories, it’s time to prioritize. Sadly we often don’t have time or money to do all the things we want right away so we have to choose what’s most important. First, I’ll organize my features in order of importance. For me ‘You can meditate with a nice timer display’ is much more important than ‘you can share your meditations to social media’. Then I’ll go in and order the user stories within a feature. In the case of my timer, ‘A meditator can choose a length of time for a session’ is crucial, where as, ‘A meditator can choose to show or hide the clock during a session’ is just nice to have. I’ll move that story to the bottom of the list.

Lastly, go through and make decisions of what user stories will be implemented in this cycle of development and note that in a column next to the stories. Note that just because a feature is in this version of the product, that doesn’t mean that all the user stories for the that feature will be in this version. My final document will look something like this:

*You can meditate with a nice timer display* (v1.0)
- A meditator can choose a length of time for a session (v1.0)
- A meditator can choose a bell type for a session (v1.0)
- A meditator can choose an image to display during a session (v1.0)
- A meditator can choose to show or hide the clock during a session (v2.0)

*You can share your meditations to social media* (v2.0)
- A meditator can link their account to twitter and facebook (v2.0)
- A social user can share the session summary of any completed session to facebook and/or twitter (v2.0)
- A session summary includes date, time of day,  length of session and session image (v2.0)

##User Stories in Software Redesigns or Iterations##

A user story document is not only valuable for developing new software but also for iterating on existing software. Often times if I’m iterating on a product, I’ll start by creating a user story document for the existing product. It’s an amazing way to deeply understand the product and (often) start to see some of the problems as well. Then I’ll make a second document for the iteration project highlighting features and stories that will be changed, added or removed.

##A note to those who think this is just fussy, old school, waterfall-style organizational overhead##
"But I work at a startup," you say. "I iterate every week. This is too formal for us and is a waste of time." To you I say, you are right. And you are wrong. All people developing software go through these steps. The only difference is how you document it. If you are the single developer of a product and you sit next to the CEO (because there are only two of you in the company), this information might only be documented in your brains and your conversations. It might be changing constantly. The important thing to remember though is that you *are* creating user stories. You are defining terms and metaphors. You are creating user types. You are prioritizing features. You are bundling certain stories into certain phases of development.

Being aware these decisions are happening every moment of development will help you be in control of the process and keep you organized and on track. In the lean startup world I often listen to developers talking about a feature and coming up with various names for things associated with it, various user stories and various priorities. Often, as the designer, I have already or am currently thinking through the exact same things and may have come to different results. I recognize a point of either diversion or cohesion so I usually interject to try and bring us all on the same page. To decisions that combine all our knowledge and insight into finding the best solutions.

For small teams, recognize that the processes I've described in this article are happening to you whether you document it or not and take control of those processes in whatever way best suits your style. For larger or more distributed teams or if you are hiring an agency to to work for you, it is crucial to have very clear documentation that can be shared around to create a clean, mutual vision.

##Worth the time##
Writing user stories like this can feel time consuming but is immensely valuable in reducing costs, confusion and misdirection. The business team can use the feature list and terms to create detailed copy for marketing materials, the design team can use the stories to create information architecture and wireframes for the app, and the dev team can use them to design and build the code structure. When you all sync up to share and combine work there will be far fewer surprises, holes and frustrations and everything will flow together much more smoothly. As changes inevitably arise, you can update this document to reflect the latest goals and priorities.
