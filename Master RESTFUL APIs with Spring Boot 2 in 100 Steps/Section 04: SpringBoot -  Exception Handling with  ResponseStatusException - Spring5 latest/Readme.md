### Step 31. Step-00: Introduction to Exception Handling using ResponseStatusException.md
Welcome back.

In this section, we are going to understand and implement exception, handling and response status

escorts for a regular restful APIs.

So we are going to look primarily into the response to Exception class, which is recently introduced

in spring fire.

So it is a fast rule for basic headed handling implementations in other restaurant space.

So it's also an alternative approach, response to sanitation.

And it is the best class for exceptions used for airplane status quo.

Hester WTOP response so we can create an instance of it providing an A.P. status and optionally Alesund

in the cars.

So if you see in detail, it's a runtime exception and response status exception.

Constructor arguments include social status, reason and cause.

So in status and as GTP status, it has to be a response for that respectless.

Philippe requests.

And the reason?

A message explaining the expection exception is that that particular response example, like if you

have said the photo for as a response user, not form, there are a specific product, not from letter

exactly in that manner, and also a triple call that the response to status description would cause.

So if you see the benefits we get using response status exception classes, we can implement it quite

fast.

And there is no specific need for creating custom exception classes unless we have a need, because

we can define hashtag response, status quo and better message at a time.

As well, creating exceptions programmatically would have more control over exception handling, so

at the same time, we have the benefit equal and we also have a little bit of downside.

So if you see the downside, so we need to deal with the application as we're defining them programmatically,

we find ourselves replicating multiple controllers.

So I think thing is a global exception, handling this approach will not look like a global approach,

like how we use in controller advice using controller advice, annotation.

It is difficult to enforce application rate conventions using a single class here.

And by combining both approaches, we can implement the control globally and also share those exceptions

locally as required.

And using that, we can achieve better results.

Only thing we need to ensure is that we are not mixing up of handling exceptions in both ways.

So we are trying we should ensure that we isolated everything properly when we are both in place.

So that's more important.

So now what about our implementation steps, how we are going to implement all these things?

OK, so we see the very high level implementation steps and when we are implementing step by step,

each step will have its own of details.

OK.

So as a first step, we are going to create a good Bransford exception handling.

So this good plant will be created both locally and then also in the remote repositories so that all

the exception handling this will implement in this respect to the plant.

So next thing is we are going to implement a response to this exception.

Forget usability service and the same way we are also going to implement response status exception for

update user bayati service.

So forget usability, whatever.

We implement firmware update usability and so it will be the same.

So or if required, we can even take it as an assignment so and instead that we are going to implement

response status exception for the user usability service Dirichlet service level so far and step one

and two, we will implement it at the controller layer and in step three we are going to implement that

service layer.

So when we are implementing that service layer, it is like directly we are using the response status

exception but in step one into when we are implementing it, it IT controller will use that as a status

exception and add the service layer within user customer exception and then move through that and then

we'll catch it in the.

Control earlier, so we'll see that how we're going to implement it, and in step four, we're going

to implement this status exception for clear user service.

And finally, once that is done, we are going to implement history status.

Good 01 created response for creating user service in the same way and location header with user password

cleared user service.

So these are the five steps which we are going to implement as part of this exception handling.

And this is the type of response status quo to section.



.

Thank you.


### Step 32. Step-00: Create git branch - local & remote.md
Welcome back.

In this lecture, we are going to create a good branch for our next section implementation, which is

nothing, but we are going to implement exception, handling and response to codes for our application,

which we have built.

So we are going to first go ahead and then check the gate status to verify whether we are in the M.B.A.

or not.

So from Master Branch, we are going to check out with Hyphen B option to create a new branch named

for the exception handling response to quotes.

And from that, we are going to also create a limited branch and then push the current base code to

the remote branch.

You get set up stream origin zero.

The exception, handling response status course.

And we can even go back to our GitHub repository and verify our branch got created or not.

So this is the big step before starting any the our.

Implementations for respective sections so far, this respectless action will first complete this these

steps.

OK, so let's go back to our comment line, which is nothing but a the next terminal and.

First, we need to check gett status, so we are on the branch master.

We can also see get sure branch.

OK, so which will show us the.

Branches, which we have currently, OK?

So if I see here the master branches with typical business services, development, computer and police

and Branch zero three is also a business service document completed which says that do not user management.

This is already a matter to master and master has the latest code with us.

OK, so now we'll go ahead and then create the new branch.

OK, so.

Get check out Fenby and then zero for.

Exception handling and also response status courts.

This is what we're going to implement now.

OK, so now if you see get.

Status.

Wearing brand 04 exception, handling this straight, as you can see it here on Brand.

So now what we need to do is we need to get push, right.

And then we will set up the upstream.

Right, set upstream.

And in the origin, so also provide the same brand name.

Korpi.

Best mode.

So it will take a while because it will be pushing the current code base to the remote plant.

Yeah, so if you see here we have the new brand created on the remote and from local branch to remote

brand.

We have the changes got sinked.

OK, let's go to our browser and then verify the same.

So we are in this stacks, Springwood building blocks, right, so we'll see the branch, you know,

we have the 04 exception handling, OK?

The latest could be a sucker for B to 036.

C, the business services development completer.

Right.

So this completes our step zero zero, which is nothing but creating a new branch of our new exception,

handling and response to the skorts implementation.

.

Thank you.


### Step 33. Step-01: Implement ResponseStatusException handling for getUserById.md
Welcome back.

In this lecture, we're going to implement Lesperance status except for get useability service.

So so we will see the series of steps we are going to follow as part of that.

So here are the series of steps we are going to follow to implement Response Trade Association for that

useability.

So first we are going to define customer exceptionally year, which is nothing but customer exceptions

package.

And then we are going to create a simple user, not fond exception class, which extends the exception.

And then we move on to the service layer and service layer.

We are going to update the usability matter with the exception, which is nothing but the smartphone

exception.

And we are going to check for user and if not existant to an exception.

And once this exception is the user is not in an exceptionally strong we need to cast that exception

in the control layer.

So we are going to change the user by the method in control.

Let me try catch block and catch Marchman implement.

That is one status exception and then will go to the postman and then we will test it.

And in addition to that, as we have been able to use in our project, so we also will also get the

place filled.

Also Priestley's attribute also in Nevada, decent response so that we are going to update our application.

That property is entrees track never.

So we will do that.

So once that is done and verify the response again, with the exception message and the host UDP status

code.

So this all these steps will implement in our response status exception for a little bit usability service.

OK, so let's move on.

I know.

So first, go to get perspective and cross-check our brand, which is zero for the exception, handling

and then response to it as quote, so which we have in the check out model, which means we can go ahead

and start over.

And so we'll go here and then create a new class.

And I will say you are not from the exception under the package exceptions.

Right.

So I'll see the exceptions and I will say.

You was not fun, right, and then I'll click on Finish.

So this is my usual not fun exception class.

So we are going to extend this class.

So I'll say extends.

Exception.

So we've also added differentiable much Nadira generated serial vaccinator here, and then we will define

our constructor here, so to define will go to certain date constructors for Superclass and I'll deselect

all and I'll just say exception string right and generated.

So we have created our default constructor here ok, which is nothing but our constructor using our

super classes.

So this is done and next is.

This completes our user, not fond exception, glass creations, so let me save this and come out.

And now next, more on Borella.

Service leader.

So we are in the service layer now, so let me make it bigger and let's go to get usable ideas service.

OK, so what we need to do here is so whenever an event occurs, which means like whenever a user tech

happens and then if that user doesn't exist, so it should be an exception.

So this method should throw an exception named user.

Not for the exception.

So.

Fund, so let me rename this I just.

Every time I forget this, so we next and then finish, OK, right now let's come back to use a service

and then use it not for my throat use and not for an exception and then import the.

Yes, an art form, exhibition class.

OK, so not so whenever we don't find the Heidi, it throws an exception, use an art form exception.

So what is the next step?

So we need to cross-check if the user is present and if the user is present, then return that respect

to the user.

And if user is not present, then through this exhibition.

Right.

So let's do that now.

So I've.

OK.

User is present.

Right, not of you is present.

Then through new user, not for exception.

Right, and what is the message so far, my views are not from the exception.

We have one input, which is nothing but that message, right.

So I'll see you are not found in use of repository.

Right.

And then I will say this.

OK, so.

That's good.

So we have completed our service changes, so Filiatrault, what we have done here so far, they've

got the user by I.D. service so far that we expect to get user by the method we have implemented, that

it was an exceptional user, not one exception.

Whenever the user is not present.

And we have to check that if user is not present through this news and not from exception, videos are

not found in user repository message.

So we also define this user not for an exception here.

OK, no exceptions package.

So this completes our service layer changes.

OK, then we'll move on to our controller changes now so we can see, you know, as soon as we have

implemented the exception handling for this user by method, we are seeing the mode in the control of

Syria, which means we are currently not handling that exception here.

OK, so let's go here and then handle that exception.

You can see it here.

OK, so currently unhandled exception type are not one exception.

You can see it here, right?

So now we are going to implement that.

We are going to handle that exception.

So we are going to introduce it like that block here.

And in that block we are going to.

Add this thing, OK, so control likes control.

Yeah, and in the catch block, I'm going to say user, not phone got user not for an exception.

Yikes.

Right.

And then if I find that exception, if I catch that exception, you first improve that.

OK, so I have inputted.

So now if I find that exception then.

Through a new exhibition named Lesperance Status Exhibition, so he starts our response to this exceptional

response status exhibition, right.

And then come and you've got to import it right.

So let me see this.

So let's define the constructor first.

TTP status.

Not.

Not phone.

And.

You can also say we can give our customers this year whatever we want.

OK, so are we can see exhibition DOT and get MRD so that whatever the message we have defined in our

service, the same message will be displayed.

OK?

So good.

So this completes our try catch block implementation in good usability.

So what happens here is whenever the user right.

Whenever you're not the exception is thrown at the service layer, it will be cached here.

And then we are going to say this one status exception through history to be not for nothing but for,

for and then also send a message.

Whatever we have defined in our service layer here, which is nothing but user not found in user repository.

Right.

And let's see if this.

Right.

So our ridi, this is currently not running, Stuart, so let me start our spring boot up.

This spring, boot up.

OK, so our application got started, so we'll go through a variety, you know.

OK, so our postman, so we are in the postman now.

So if you see get used by Eddie.

There should not be any idea with the one we should have by the 500 at one zero one zero one one zero

two and then one zero three.

Right.

So those will be available for us.

OK, but with one oh, we don't have any.

We currently are with 1000.

We don't have any idea in our database.

Right.

So, see, we have got the timestamp, which is the timestamp status error message clear.

And in part this is the spring paraded before the constructor, which is nothing but the photo model.

Okay.

So in this way will get the responses currently.

So if you want, we can customize the teratogenic exception handling the class.

OK, but for now we are getting the spring standard.

Ones will do the best for us.

Why?

Because most of the thing is already constructed here.

But if we have a need, we can even add a gentle exception, handling class and then our own what we

call our own attributes there.

OK, so here we can see a timestamp and the status load we said has to be not found.

It is for four.

We got it.

And also saying that it is not fun and it was also sending the message that are getting message.

We said he was not found in use repository, whatever we have defined in the service layer.

In addition, we can also see that we are getting the trace right.

So in this case, we need to be able now because we have enabled the tools we are getting that we will

disable it anyway.

So in the part of the user we are trying to access, we we we are getting it here.

So let's go back to our.

This one, right, and this is the parameter, right, Sara, that includes.

So this one, we will copy it and then pasted in our application dot properties to disable the.

Thing which is coming in our response.

OK, so I click on application that properties.

And I'll see.

And I'll say never.

OK, hold on, trust, but on whatever it is, OK, but currently by default, it will be set as always.

So which we are disabling.

Let me save it, OK?

So my job is getting reloader after the sale.

So let me go back to the postman and then one more request, OK?

Now it looks very good for us.

OK, so time stamp status error message in the bath and we are saying he was not found in use a repository.

Right.

So this is the thing.

So this completes our.

Response, status, exception, implementation for a look at user by.

So what we have done, just to reiterate, we have implemented custom exceptionally OK, which is nothing

but custom exceptions.

Package and the use are not the exception.

And we have implemented the service layer for the user by the method that throws exception and then

also implemented exception.

Check when you need to be thrown and whatever the exception thrown, we are going to catch that exception

in that control layer and then using try catch block.

And we implemented the exception there with the response status exception with both be status quo and

message and material.

So we are bringing it from our side, which will be defined.

And we went and then tested it using Posman and then seeing the proper responses.

Whatever we got, whatever we have defined.

We also know that we assign exceptions, OK, because of whatever is coming, we have removed it.

OK, so and we have verified again and we have got the proper exception message and then has to be status

code.

So this completes the implementation of this masturbators exception for that user by 80 or so in the

next lecture and focus on implementing the same further update usability.

.

Thank you.


### Step 34. Step-02: Implement ResponseStatusException for updateUserById RESTful Service.md
Welcome back.

In the previous lecture, we implemented the response to this exception for 11 years, thereby 80.

So in this lecture, we're going to implement the for our update useability.

So let's go ahead and then see the steps which we are going to perform.

So first, what we're going to do here is we are going to go to service and update the user usability

method with the exception, and also add the checks and balances, which is nothing but whether the

user exists in the respective repository.

Whenever the user, by the request comes late, we're going to check the rules that exist.

And then if that user exists cemetaries, the user doesn't take this to an exception so that we little

step we are going to implement.

And then the controller, we we're going to apply the title to block for the metal and the catch block.

We are going to implement the response status exception and then we're going to go to the postman and

then they start to use that for the error message.

So both the exception message and then here, should it be status quo.

So let's go back to our idea.

You know, so we had an update usability user in the user service.

We can see I produce about 80.

So here we don't have any checks.

Like as soon as I send the I.T. and the user body waterloo's and said that need context here and then

say to the repository so said right in the Palestinian context and then say, OK, but ideally what

we need to do.

So we need to check if the are from the local user, from user repository based on that idea and then

check if that exists or not.

And then if it exists, say it, if not exist with the exception.

OK, so I would tell the truth user, not one exception here.

So what I'll do is I'll copy these lines from our user by idea.

Right.

So I'll say control.

See.

And.

So I say this says optional use of.

Right, so now what we're doing here is we're going to check your deposit or not find a way to build

an I.D. sent, and then if the user is found right, if the user is not found, what we are going to

do is we are going to try a new user, not from exception here.

If user is not found, if he was found, then using the user user.

That said he said the position in context and then return the safety user.

So what I'm saying here is that not only the user repository and I'll add some additional message here

that provide the correct user data.

Right.

So this is these are sample services.

They might not be 100 percent like instead of sending a dynamically generated I.D., which we have usually

when we can send the user name, which will be unique to.

Right.

So multiple things can be done.

But here, the core concept, what we are trying to understand is how to implement the exception handling.

OK, so that's the story.

So here now we have implemented here update user by idea, like a check the user representative not.

And if your settings present, set the context and then save the user.

If user is not present, then throw the exception was not one exception with messages user not from

the user repository provide the correct user.

So that's what we have implemented for update user by.

So now if you go to the user controller.

Right, it's already throwing the message right.

And if you see here, it might be saying the same thing here.

Unhandled exception type user not font.

Right.

So which means we need to enable that like that block and then implement the exception handling for

this.

OK, so let me see.

Try.

Right.

And let me copy this, OK?

Right, and then we have the cash block here, which says.

What happened?

Yeah, users not for.

No exception, he right?

And then we are going to throw no response status exception, right?

It has to be status as 400 bad requests so I can throw the thing at 400 bad requests, and I also say

that I'll get the message from my service lawyer.

Maybe it's not a good message, but.

And then.

Let's close this, OK?

So now this completes our updated survey.

So what I've done here, so I have implemented a catch block and then that any 10 the I that update

you, that my idea and the news are if we get if they use that exist, if not, then use are not handled.

Was not one exception here with true new responsibilities.

Exception.

So let me save this.

It's already saved.

So let me save.

But right now, let's go to the post management district.

OK, so we are in the postman.

So our choices are producer 80.

Right.

So let's see if the user one doesn't exist.

Right.

So I say send.

So what happens?

It says time stamp status is for bad requests like yours are not from the repository and then provide

the correct user.

So whatever the message you have given in the service layer, we have got it in the state of response

also for granted, bad request.

So this completes our implementation of the response to this exception for our update user Bayati method.

Right.

So we have implemented the changes in service layer controller layer and also tested using Posman.

So in the next letter, we'll focus on implementing the same for delete user by 80.

But what we will do there is like a little bit different.

We'll do everything from side with layer instead of coming at the controller layer, which means in

the service layer itself will implement the response status exception.



.

Thank you.


### Step 35. Step-03: Implement ResponseStatusException for deleteUserById RESTful Service.md
Welcome back.

In this lecture, we we're going to implement a response to the school exception for the disability

service directly at the service layer.

So let's see how we are going to do.

What are the steps involved here?

OK, so let me go to the steps.

OK, so if we are going to go to this man, check for two years and if not exist, then throw the response

status exception directly.

OK, so there is no customer message and then handle the sadness.

Look at the controller.

So in control made no changes.

OK, directly we are going to implement this at the service layer and then test it.

OK, so let's go back to what I really know.

And we are in the user service.

Not so it here.

OK, so you are saying.

That if you saw the predator, that fine bird is present, then you're not delayed, but so we can remove

all those things like, ah, let me bring this out here, OK?

And then let me remove this and then copy the same thing, which we have done it for our average user,

by the way, because we're going to check the user.

And then if the user is not present, then through the exception and if the user is present, then deleted,

that is the thing.

Right.

So it's the same concept here.

So just copied here, that's all.

So now if you see what we are doing is if the user will find the user, what they've done, whatever

input parameter will find the user and if the user is not present, then throw a new exception.

No exception is going to be here in response to this exception.

So let me see.

Response status.

Exception, and I'm going to say it is to be Dr..

SJP status, not a bad request, right?

And the messages seem so, and we need to import this that so import response, status exception.

That's all.

And then we are good.

So let's see what we have done here, OK?

So.

The user sent as input parameter ID, so we'll go and maintain that user in the user repository, and

if the user is not present, then for response to the exception, that status quo type status, that

bad request for 400 and the message was not found was was repository provider correctives already.

So that's about the thing.

OK, so that's what we're going to do.

So this completes our delete user by implementation.

So let's save this and then go ahead and test it now.

So we have saved it.

Let's go back to our Posman.

Right.

And here is the thing, OK?

So one should not be in our database.

So let's hear one.

Right.

And if you see, we got that right.

So your status is Freudenberg by request and method is used not only the repository but the correct

user.

So that's about the thing.

OK, so this completes the implementation of delete user bidi, that response to the exception.

So in the next election, we'll see the create user thing.

.

Thank you.


### Step 36. Step-04: Implement ResponseStatusException for createUser RESTful Service.md
Welcome back.

In this step, we are going to implement this status exception for create user service.

So let's see what our steps involve for doing it.

OK, so let me go back to my steps, OK?

So here are the steps, so implement response, status exception for our great user, so to do so,

what we're going to do first is like we are going to create an exception, which means exception plus.

So, again, we are planning to implement this like a standard implementation like production model

where we can say that we will have the service layer where we can through the exception and we'll catch

it on the controller layer and prove that response or description from controller layer.

So for that purpose, we are going to again create one more custom exception clause, which is nothing

but use that exists exception.

So the service, we're going to update the creators and matter with the exception, and we're going

to verify if user exists based on user name.

This is the important thing here, right?

Because for the user level, as the idea is going to be auto generated.

Right.

So we will not have any information.

So we need to verify it based on user name as user name is a unique constraint.

We should be good with that.

OK, so we can say user target user name and then if the user is not equal to now, throw the exception

that whatever the response came.

So if it is not like whatever the response came from, this check is null, which means that user is

not fun, then see that user.

So that's we are going to implement OK.

So if not null then true the exception.

That's what we are going to implement.

OK, so if our primary is instead of our pegylated idea, if it is user name, then the implementation

is going to be a little different again.

So it's a case to case basis, right.

So here we have implemented in this model.

OK, so it's not a standard R, right?

It is only the beginning to implement it, not the case.

OK, everyone will have their own style of logic and like to implement in this way now then going to

control and will update the creators of method with the try catch block and in a catch block we will

catch the exception that this exception when this is thrown and then implement the response to exception

and then test the same using other Posman.

So this is what we're going to implement using our response status exception for the user.

So let's go back to it, you know.

Right.

So.

What is the thing, so we make it so let me go to my exceptions package and then say no class, right

and no exceptions package.

So I'll see you.

There exists exception, I can say, that already exists.

Exception, whatever the name we feel is relevant here.

Right.

So and in this.

So what we will do is.

Bill extends to.

Exception, it's the same as the last one, OK, so I'll send it generators, you will watching.

You are OK and then I'll created constructor for this, right?

So from source construction using superclass and the deselect all and then selectively string one by

because currently we're handling only with the string.

So this is created so.

Let me say it right?

Yeah, but so the exception to that respect to class user service.

And let me make it bigger, right?

Yeah.

So what it was that our clearly other method is very simple here, which means whenever they use a body

cell, then I'll just say that use are currently extended with another three to four lines of additional

logic.

So one is we are going to check if user exists, right, using username which is sent in the user body.

OK, and.

If not exists, this through exception named.

Use this exception.

Right.

User.

This exception, so to do so.

First, I need to extend my this one, OK, so it's estrus user exists.

Exception and then improved that class here, OK?

And first thing is, if you that exists using username, right?

So first one we need to do is we need to check that user is present, but not using user.

Existing user.

As a to.

User repository.

Not fine, but you said you have a method named find the username, right, and for this, we don't

have any input parameterize user name, but we have something called we have the complete user objects.

And so what I will say is you said that that username, so that I can get the exact username sent from

the request and then using that, we will implement this.

OK, so now what we will do is.

Right.

So if.

Existing use of.

Not equal to.

Right.

So which means some that is present inside.

So then I'm going to throw the exception to the new user existing exception with their message, suggesting

that whatever we define, we never use that exact exception constructor.

So I'll see.

User.

Already exists in the repository, so I'll say this, OK, that's all.

Right.

Let me.

So what's happening now?

So we have implemented three things here.

One is we have other method procedures like this exception when OK, when we don't leave, when we find

that user in the repository saying that already exists in the repository.

So find out whether that user exists in the repository or not because of the user repository, that

findable username.

And as we don't have any input parameters here.

Right.

So using the user context.

Right.

You are not getting the name.

We have provided it so that if the user exists based on that, we have implemented this logic.

OK, so now this completes the service layer implementation.

So we'll go to the controller layer controller had already started complaining for us.

OK, so let's go to the quote users area here and then we will implement the toilet block here.

OK, so what I'll do is.

Hmm.

So I see control here, control shift format, OK?

Right, and no, implement that catch block and catch block.

I need to catch the exception yuzu exists.

Exception, each lt was like this exception and.

Let's throw the response to exception description from here, right, so I'll see through new.

Response status.

Exception.

And I'll say ETP.

Stuart, I start by the quest and you start get a message from the service layer.

So let me go up.

Yeah, here is the thing, right?

Yeah.

So let me say it.

OK, so what we're doing here is if you use that exists, then the exceptional catch and throw the exception

with this one status exception, if you did not exist, you just have to start create yourself, OK?

So let's go to our postman and student.

OK, so here is the you, sir.

OK, so this time user might not be there.

They're OK.

So let me create it.

OK, let me send it and then.

It got created.

All right, so get used by the if I say one will find that user wrote.

See, we find we are finding that users are now, again, one more time for the same user.

I'll try to send it.

OK, so and then you should try an exception for us, OK?

I have sent it.

OK, so you can see it here.

Timestamp and status 400 by request user already exists in a repository.

So we have handled successfully this user already exists exception.

So that's about the create user exception handling using response status exception.

OK, user already exist exception.

So let me go back to the steps and let me reiterate what we have done here.

OK, so first you have to use this exception clause in the exception package and then in the service

layer for the community as a method.

We have extended it to say through the exception and in that we have verified of user existence.

If user exists, then through the exception, namely user this exception and in the country that we

implemented try catch block there.

If the catch block, whenever this user like this exception is thrown, it will catch that and then

throw that response status exception with this to the status quo.

And then the speckling message.

So we went to pressmen and then posted the same and we got the expected exception, response and then

GTP status code.

So this completes the step about implementing response to this call for it cleared user.


### Step 37. Step-05: Implement HTTP Status code & Location Header for createUser Service.md
Welcome back.

In this lecture, we're going to implement his typical response called Astudillo One created for the

user creation service and also the location that we are going to be using.

You are a component builder so that the location will be the part of the user which it has created.

OK, so let's see how we are going to do that so we will see the steps first.

So we are going to implement this completely in the control.

More so in the controller here.

We are going to implement two things.

One is that the one created and the other is the location header.

So location that we are going to use there, you are a component builder to build it.

So another important thing here is when we are building it, right.

So it's a location header, so which is nothing but a header.

So we are going to set the headers here for location and it's like a desktop set.

Location of location had been using very competent builder.

So that's where we can to implement.

So let's go back to already idea and do that now.

And once that is done, we're going to create a user and then test it.

Right.

So I am here now.

So first, what I'm going to do is I'm going to set.

To find that you are a company builder.

So you are a component builder, and then I'll say Dallas builder, right.

And no, the next thing is up.

So let the user get created.

We don't have any problem with that.

OK, so once the user is created.

Yeah, here, OK, once the user is created, so let me say why I'm not returning anything here currently.

Yeah, so.

Once the user is created, what should happen?

That's the important thing, right?

So.

They will.

Petfinder has treated beheaders, no.

It does.

This is a call to.

You just heard us.

Right, and then I will say at the start said location, location, header.

Right.

So this is the one that said location inside this, I'm going to say that that part I'm going to set

the part right.

So in part, first thing in my what will be my partner here?

So slash, you know, just slash how you divide.

So that is the path and thought how I'm going to get by using dart board and then expand and I'm going

to be using you.

Dart, dot, dot.

Right.

And then see who you are.

So that now I have my location on the desert with the smashing of or whatever that I created.

So now what we need to do is we also need to return the responsibility.

Right, which is nothing.

But one is Hadass and then one is has to be a status created.

So let me do that now.

So you.

Response entity and I watch these wild ride.

And.

The parameters are Hadass, and that is how it to be so so far we have we to this location here that

we should be good and another one which we need to achieve nothing but has to be status quo.

OK, so.

Let me put response entity so that we are good, so now you're also going to defend Leveton Typewrite,

such an attitude and take responsibility, right?

So that's good.

So now if you see here, what we have been able to do is create a user user got created and we are going

to set the Hadass.

And it's like a had this in history to be here that we are going to set the location header with the

user slash.

I like user part and then we're going to return it back, OK.

So what we're going to return to sender has to be status created.

OK, so let me save this right.

And let's go back to our Posman.

Right.

And then this is the create user.

So I'll say this is a fun one.

OK, so let me play this.

OK, so I said, so what happened?

You can see it here.

Two zero one was a God created in the same game.

And the group of the headers here, see the location had that right.

So location, its original slash one.

So let me create one more user for our convenience.

Right.

So let me get this up.

So I'll say the user to and then as soon as the constraints, we need to change both of them.

Right.

So I'll say one more time.

See, now, location header is true.

And should it be status quo, that was the one created.

So this completes several created as a method implementing both the location header and also the history

to be status quo to zero.


### Step 38. Step-06: GIT Commit, Push, Merge to Master and Push.md
We'll come back, one final step is to checking the code, what we have done so far and then push it

to our respective repositories.

So I will go to the staging and then I will make it bigger.

Right.

So we have captured these files, whatever, and then created two new friends and notable exceptions.

So I say.

Response status.

Exception must come it right and then I click on it and then push so that this will be pushed to the

remote repository to.

Good.

So this complete so another thing will go over get.

Perspective, and then we will check out the master, right?

Yes, I want to check out the master.

Before that, I'll go to my gym here and then stop the gym.

OK, so I'll go back to get perspective and I'll check out the master.

Do you really want to check out my stuff?

Yes.

OK, so I take that master.

So I would imagine my exception handling branch into the master.

So I would say much OK, with my 04 exception, handling my master will be master with exception handling

it good.

OK is computer response.

Should have exception for good.

So now I have a master here.

I'll push the same branch to the remote.

Right.

If you.

And then push it.

OK, so push completer, so if you see exception handling and let me do your final refresh so that we

get the latest things.

Here it is, it filed for refresher.

You can see here both have the same comical fine and B nine six two four zero four a.m. the same also

M. and 04 had the same chemicals.

So which means our respective branch where we have committed to the changes and we implemented and committed

to achieving this.

And our master plan in both local and remote are in sync.

So this confirms that we are good with this and in the next section, whatever we are going to discuss,

but again, will create the new branch and test it.

So now you have the advantage of checking out whatever branch we want.

Okay, so this is nothing, but this is ground zero branch.

Okay.

Which is we don't have any other code, so this is only a world.

And after that we have implemented a user management service in the same way.

This is exception handling so like this.

So every incremental mode we are doing it.

So this will help you in checking out and then testing in an incremental manner.



.

Thank you.


