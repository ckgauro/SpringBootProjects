### Step 84. Step-00: Versioning Introduction.md
Welcome back.

In this section, we are going to understand and implement a pill rationing using Springboard.

So if you see here, it is primarily categorized into four of us.

We can implement Springboard.

So once is the solution and the other is the request parameter rationing and the other is custom header

rationing.

The last one is we type are mine type are acceptable rationing.

So to start with and start with and understand what you are rationing.

So if you see here you run over something is nothing.

But we are going to provide you what is the version of the EPA if we are implementing multiple versions

of our EPA.

So we are just going to provide its rationing now where you are.

So if you see here we have the one that we're watching rationale for the EPA and B 2.0 version of our

AP implementation.

We are going to add additional address field in our entity and then we are going to retrieve that using

V 2.0, which means in our in response, we are going to see addressing those extra.

And we did meet with the Russian and in Russian, it is going to be, as is so far, whatever we have

to build it.

So we're going to do that again.

It is going to be absolutely real time.

It's not.

We just.

Beans and then static beans and then creating some variables.

It's not like that, okay, so we're going to use standard GPA and implement it.

So as we have already created the entity.

So now we need to ensure that to support both views.

One is B 1.0 and and B 2.0.

In very previous lectures, we have already discussed about three major things.

OK, so one is the model mapper for the details.

The other is map script and also Jason.

So we have already implemented those things in our previous sections.

So what we will do is by using that knowledge, we will try to implement and then showcase our V 1.0

and then V 2.0, the different fields.

And so not using the model number so that we like a single entity, having multiple fields like newly

implemented fields will be available in 2.0 using model mapper and whatever we have created for V 2.0.

So movement from university, that is the request parameter versioning indicus parameter rationing.

If you see we're going to pass the parameters of the model so that parameter.

So if you see here, Russian is equal to one, so they can also say the parameters.

So the other one is watching is called as usual, the same user data as what we have created is auditable

what we want and then veto accordingly.

We are going to leverage for implementing the request parameter worsening too.

So the next one, Mouzon is like custom header versioning.

So so far we have seen UI and also the WIKUS parameter.

So the next is to implement the API versioning using custom header.

So we are going to implement it in such a way that whenever we send a header name as a Russian with

value as one, then the JSON response will be whatever is related to Russian one.

And if you send, then whatever is related to will be displayed.

So that's about the version we we're going to implement.

So the next is media type.

We also call it as mime type or even the acceptable versioning.

So in this we are going to send accept header.

So and when they accept that, we are going to define in our respective method.

So if you see here, this is the accepted that, OK, so this is the standard format to define it.

OK, and if you go to Disney dot org, we have the letter standards to define it and then follow a lot

of standards for implementing Meatpaper mind type headers.

OK, but for now we can take this as a reference and then we can implement it.

So this is the V1, but our python difference is that we need to fetch the V1 API details.

So the same be happy for me to fetch as the beta version of the details.

So moving on to the implementation steps.

So what we are going to do is as usual, we are going to create a new branch for our Entropia learning

module and we will create the prerequisite things required for us.

So we already have a user management application with all the related services.

So what we will do is will create the equivalent data was required for us.

So one of the user, DETI will be one and the user data V2 and then move on with implementing the you

are a versioning using those data was will implement the required methods.

What you are watching using model m'appelle and the next is to implement the cost parameter.

Roshini so that one also we will implement using the methods we define their next is implement custom

header versioning and then also implementing the media type portioning.

So once we implement all these things and then test it so it will go ahead and then commit and push

code where idy so this complex, our entire API versioning, so on high level we can even see the steps

required for doing so.

These are the detailed steps outlined in our best quality, Terfel implementing it.

So in every step what we are going to do, we have listed out here.

So what we'll do is like whenever we are implementing that respect to step as the starting introduction

will discussable each step and then implemented it.

OK, so we have built seven steps to implement each new order.

So we will do that in our upcoming lectures.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 85. Step-01: Create DTO's required for Versioning Implementation.md
Welcome back.

In this lecture, we are going to create a new big brand for our versioning module and then we are going

to create the divisions and they are just filled in our user entity.

These we are going to do to move on with our internal implementation for versioning with all the four

types which we have discussed in our introductory section.

So let's go back to the code and then review the steps which we are going to perform.

So if you see here, we are going to create new good brand.

So I'm going to come up with this and then put this ready.

And the next is we are going to go to the user entity and then add a new field address.

So once we added whatever we have defined in our data that Ezekial, which is nothing but our pre populated

data, it is going to tretter.

So we'll also add some data for address column in the data that Ezekial.

So that completes our entity layer changes.

So then we'll move on to our data layer and will create details.

So one is user data will be one and the other is user V2.

In the user it will be one.

We will ensure that whatever is currently present before adding address feel.

So we will try to define all those things except address and user data.

We will also add the address field.

If you see here, we are going to do this with our GPA implementation and also the -- to database.

So it says that it looks like 100 percent real type of implementation where then we want to handle these

things from versioning perspective, how we want to handle our controller layer or our service layer

with our videos and then all these things we are going to look into now.

So let's go back to the idea, you know.

Right.

So if you see let me go to the get perspective.

And if you see here.

The previous comment, which we have done is with the maps, that means like the previous section which

we completed is 10 to springboard detours, maps, and it is also merged with our remote muster and

our local master, which means from our local master, we can create a new branch.

OK, and then I'll give the names 11 01 Springboard Learning.

So the reason I have two 11 zero one one zero two, we are going to look into springboard content negotiation.

So we are going to have two modules in the lemon section.

One is watching and the other is content negotiation.

So far, zero one we are giving versioning.

So let me click on finish.

So we have checked out now with our 11 zero one springboard LESSONING.

So let's go back to our idea.

So our first challenge is to go to the user entity and then implement the new address, fill in that.

So I'm going to include this section here, OK?

And then I'll open my user entity.

Right.

So let me make it bigger.

So I'll go down.

And here I'm going to add a new field named Public String Address.

So I'm just giving it as a string for now.

But if we want, we can even create a model for that and then define like city and then street and then

country, everything we can define.

OK, but for now, to make our implementation easy and also to ensure that we, our core focuses on

versioning.

So in short, I'm just giving the string here, OK, and I can see column.

Right.

And the name is equal to I'll address OK and will go down and will regenerate our fields.

Constructor with that.

OK, we can even write it but it's good that if we generate.

Constructed using fields, and we have the address listed.

Now let me generate it, OK, so it had generated here, so let me copy that card and then pasted here.

So now we have generated fields constructor.

Let's also generate the getters and setters.

OK, so I will generate the getters setters.

So generate getters and setters for our address will select all it selected let me generated light.

So we also generated a two string earlier.

OK, so the two string mainly is for our if we enable any logging in our controller, our service layer

and if we want to log something related to this user object or user being so we can this to string is

there, then the things will be logged effectively.

So that's the reason we are generating this two string.

So let me read into it with our new data.

OK, generate two string generator.

So ideally we didn't enable logging so far, but on some time later when we are working on the logging

module, effectively, we are going to look into it.

So now if you see if I start the.

Tomcat, it is going to fail.

OK, why?

Because we don't have the address feel right, so address the data we don't have so obviously it is

going to fail.

Column count does not match Eskil statement.

We can see it very clearly.

So let's go to our DataDot skill in our sauce main resources.

So here, let me say open with Backstreet's.

Right.

So address will come as the second field based on the.

Order.

Right, alphabetical order.

So ideally, we need to define our queries with the user and then hear everything, the detail, column

names come up and then in that order, we need to fill the data here, for example, like a user I.D.

and then address in the same order.

We need to fill the data here, but that it looks bigger.

So we just took the shortest path, OK?

So but only one thing we need to ensure is we if that field comes here, are not we need to cross-check

in our history database.

OK, so like that.

So we'll have some minor issues with this.

But fine.

OK.

So here it is.

It's only a in-memory database.

Right.

So here I am going to say I'm just going to use that restring, OK.

So in the same way.

So I'll also give you here New Jersey.

Right, and here I will say.

California.

OK, so we added.

Three fields here, OK, means like for the three records, we are there, the address.

So let me save this.

OK, now it is safe, let me start this back, OK, Ranna'sSpringboot dletop.

OK, this started, so let me go back to our house to console.

And then let me connect to that and then click on users, so let's start from user one selector so you

can see user right here and then we got the address and then address that also populated here.

So as I said earlier, after the user area address got populated, accordingly, we have used to date,

but ideally we can write our own insert statement when you are writing.

You can write, as I said earlier.

OK, so it is nothing but insert user insert in the user and then we can define all of our column names

here.

And then in the same order, whatever.

We have defined the column names here, we can enter the data here.

OK, so let me save this back.

OK, so no changes.

So this looks good.

So this completes our both entity changes and other data security changes.

So our next step in this system in this respect to model is in this respect letter is to focus on creating

our two.

Dee Dee was OK, so data transfer objects, nothing but user data will we want and then use the data

we do.

So if we go to over data or section, we have user MDT and then user MSJ do so in a previous section.

When we are working on model mapper and then map struct, we ensure that we have created these things,

which is nothing but a means nothing but model mapper and A is nothing but map struct.

So for our versioning section will create user data V1 and then use a veto.

Right.

So I'll see user little Vivaan.

Right.

And then let me finish.

So here we need to define all other variables.

OK, so all the fields we can see.

Right.

So let me go to user.

OK, and then let me capital orders, OK, so except address, we are going to have everything in this,

right?

So let me go to you.

That will be one.

And let me remove all these things, whatever we have extra.

Right.

So let me come here.

OK.

So just a second.

It is over almost, OK?

So we have all our.

Friends defined here use a lady username, first name, last name, email and then assistant and then

order.

OK, so let me source and then generate our.

Getters and setters for all these things.

OK, so generate and will also generate for the GOP, so no argument constructor is needed to make GOP

happy.

So I'll see constructor.

OK, then let me remove this and false constructor will generate it and then put it, and if required,

when we are doing logging or anything, it will be useful for us.

Right.

So I'll see.

OK, so gender that feels constructed also, so we have now everything ready here.

So this completes our user, DTL, V1, right.

So let me save this and minimize and I'll go here and create our user data.

We do.

Right.

So next class is.

You said that you veto and let me click on finish.

So now we are going to create you that it will veto.

So what we have so far, we have the following vote.

So let me copy and paste best.

We have all the variables in the date of a veto.

We are going to have one thing extra here.

It is nothing but our address feel right.

So let me get this and copy it in our user.

Veto.

Right.

So now let's generate all our getters and setters and everything, OK, so gendered constructor from

Superclass.

OK, so that's done.

So let me bring it down.

Yeah.

Let me generate our constructor using feels generate.

And finally.

Generate our data, set us selectable and generate.

So we completed creating our user data veto, so this completes our section, right, so we need to

add new full name address, addressing our user entity, update the data school.

And in the data, literally, we need to create user data even and then user data we do.

So we have completed these things in the next lecture will move on with implementing Urara versioning.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 86. Step-02: Implement URI Versioning.md
Welcome back.

In this lecture, we are going to implement the Urata versioning, so let's go back to our detailed

steps and see them.

So if you see here in the control earlier, as I said earlier, we are going to focus on using the model

map or further converting our entry object to the digital right.

So for that purpose, we are going to use user model Mappa Control.

We are going to copy and then create.

It tells you that you are a worsening controller and then we are going to use Model Mappa to transform

into great detail and then we are going to implement things like using this.

We are going to transform and then we are going to implement two methods, one for one and then one

for V2 and for other versions.

You can see for V1 we are going to see V 1.0 slash 80 or we wondered once we can get multiple versions

here if we want.

And then for V 2.0 we are going to see it like this, which means we 1.0 and then 1.0, not at the same

level.

So in the same way, we 2.0 will have a different level, which means user data will be two will be

displayed for this, which means it is going to have the original address field.

So when we are testing the postman, we are going to use this.

You are right.

OK, so see versioning slash, you are slash users.

So we have given very thorough names so that we are doing the stuff in the right order.

OK, so there will not be any confusion when we are learning also.

So all the code will be useful for us as a template and if it is required.

So let me go here and let's go to the controllers.

We have the model mapper controller here, so let me copy that controller.

And then base state controller, right?

And I'll give the names, whatever I define here, user Urata versioning controller.

Right, click on.

Let me open this now word.

So if I see here you have the model, mapper, slash user, so let me change it to the euro, whatever

we have defined here, right.

So which is nothing but.

Rationing, slashing water, so whatever we are testing, all other services will be under rationing

slash, you are slash users, so this control at how it is unattracted with the rest controller.

So this is going to be a test controller and it requires mapping.

Is rationing slash?

You are slash users, which means you Tewari and we have user service word and also model map are operating

there and then we have existing method here stating that it's written by per user model per user.

MDT will and will take the idea from the part variable and then what we'll do is we'll retrieve the

user OK, thoroughly that user object and then pass it to our model map of that map, that user and

pulling the model apart, that whenever I send the user for you, you convert it into user data.

So if you convert it to our V1 version, so Hollywood is going to be you will see.

So if you see here, our get mapping is going to be this way.

Even we can write it down.

Right.

So I can say we are going to use two things here.

Right.

So I will say and OK, so.

We wondered zero and another version we are going to use here is slash the one that one slash Heidi.

Right.

So this is the thing.

So this one we are going to use for.

Version one, right?

I can see you want to be a sir.

Versioning and hyphen and then we one that looks good, right?

So.

The return so far as it is going to be for the vivants version, it is going to be we can change it

at the end.

Okay, so now we have if you see here.

Are going to get the user in the user optional, and from that we are going to retrieve the user.

So now and then what we want to transform is we want to transform it into user data V1.

Right.

So instead of using the memory to silence the user, data will be one in command.

You've got to improve that.

And you're the name also user data V1 and from model number perspective, model map of that map and

whatever that user.

Right.

Whatever the user decided we have retrieved.

So that need to be transferred, transformed into user data.

We won the deal.

We won that class.

So what are we going to return the same thing.

Right.

User data.

Even so now we also need to change our method written by peer to user data on V1.

So let's change that one.

OK, so that's all.

So what we have done here is we have used our existing model mapper controllers method.

OK, what we have defined there in that what it is there is we send the ideavirus service and then we'll

be using that as we get the user in the user optional exact user object will get it here by using user

optional dockett and then that respective user object will pass it to the model.

Or that map as the first parameter means nothing but the source parameter.

My source is the user object and my destination is going to be user table V1.

So and then I'm going to return the same user data V1.

So this is about the first one, right?

So if you define the second one, it is going to be just me.

Two changes, right.

So let's also define the second one, too.

Right.

So let me get it down here.

Copy.

And then it is going to be me too.

Right.

So when we do, we said that we 2.0 will suffice for us.

OK, so I will say V 2.0.

OK, and we don't need to put like this for that.

Right.

OK.

And my method is getting somebody to write and it is going to return me to write instead of me when

we are going to return V2.

And Rita.

And Rita and even the return type is going to be to come on shift.

All right.

So now our user data will be told will be written using this.

OK, so let me save this.

So we have also implemented the V 1.0 method and the 2.0 method.

So in V 2.0 method, it is going to transform the user into user data.

What we do, which is nothing, but which also contains the address field.

So and then it will return.

So this completes our you are versioning implementation.

So we will move on to our.

Postman and then all right, so let me copy this.

OK, so let me go to the postman here.

That is it.

Yeah.

So we have already disappeared.

This is all the letter.

Posman projects are Posman requests.

Clearly separated so that at any time we contested thoroughly those things, so in the same way for

the divorce, also we have these things in the same vein that will create a new folder for our in England,

worsening and worsening.

So let me minimize these things.

OK, so in running, our first thing is our first request is going to be at request.

I'll say I'll say get yuzu by Heidi and then I'll say you want to be one, right?

So worsening.

So let me.

So this is one bad thing in Postman.

OK, so and what I'll do is like I'll copy our what can you use us whatever we have defined in our controller,

right?

So now what we are going to do is here we 1.0 and then let me say it here and let's call that, OK?

So we got the response.

OK, if you see here, the user name, first name, last name, e-mail, SSN orders, and then we don't

see any of the address Filkin for 1.0 in the same level test one more for one bad one and one that one

also didn't get any address field.

So let's do it for 2.0 in the 2.0.

If you see here we have a map of the user will be to where we have the address field.

So let me change it to zero.

Right.

So 2.0 and then save and then send it so we can see here address fill popped up.

So for using that you said about chinning when we are using V 2.0 we got the address fill that's all.

OK, so we can even say Wittels.

Serious we to so that we have the equivalent product for that one.

I will say we 1.0 and and Invicta, I will say May 2.0.

So this completes our implementation of your BASAD rationing, OK?

We have done everything with our GPA and then has to database with our existing product itself in detail.

And we have used the model Mappa for transforming our user object to user data.

So in the next lecture we will focus on implementing the.

But chinning using request parameters, so I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 87. Step-03: Implement Request Parameter Versioning.md
Welcome back.

In this lecture, we are going to implement a request parameter versioning, so let's go ahead and then

see the detailed steps we need to implement.

OK, so in request parameter versioning, as usual, we are going to copy our existing user.

You are watching controller and then add additional parameters with parameter version one and version

two.

So methods are going to be and the data objects are going to be same.

But only one thing changes is the parent's values and another thing is the complete you in the controller.

So this one is for our organization perspective, which means like how we are organizing our APIs,

what we are building as part of this project, we are going to say versioning and under what we are

saying, it is paramount.

OK, so let's go ahead and then implement that now.

So as usual, we'll copy this and go back to our idea.

Right.

So I need to come back.

I think so.

User, you are a worsening controller.

Let me copy it and let me paste it and let me get the name right.

I'll say this says user request parameter versioning controller.

Right.

So we are creating multiple controllers here because we are trying to put our code very much separate

so that it will be easy to reference as part of this section what we have done.

OK, so we are clearly organizing to ensure that our during the learning process, we don't have any

issue or any confusions.

All right.

So now we have changed our request, mapping to versioning slash Perram slash users.

Right.

So now instead of you are rationing, this is going to be the.

Request barometer, basad whatshername.

It's the same for this one, Ulcerate.

Listening.

So what we're going to send instead of you, what we are going to send.

Request Adams.

OK, so let me remove this and let me remove this right and I will say value is a call to slash Irey

after users, right.

So and value is equal to Idy.

And now we need to define our bottoms.

OK, so I'll Adams is equal to.

Version one, right?

So this is going to be version one, so this method is version one in the same way I can define the

same for our second method.

Right.

Let me keep it here for our second method.

And it is going to be the version.

If we want, we can put version one in there and then see what happens.

Right.

So it throws the error.

So let me change it to two and then save it.

OK, so now it popped up correctly.

If you want, we can see what happened.

OK.

See.

And we can see it here, we have the weather popping up again, ambiguous map and cannot map so-and-so

or so-and-so, right?

So that's the thing here.

Was a request from Washington controller.

So let me change it to Russian two and then save it.

So if you see here in the mapping section, right.

So things should be unique, which means it cannot be either either here, it should be unique or in

the parameters.

Right.

So if we have one more parameter here, again, no issue as input parameter.

So it's the error is related to that.

Nothing related to what?

Chinning what we are doing here, OK.

So now we have defined both methods with the Russian one and then Russian in the gate mapping with Purdum's.

Right.

So now we can move on to go ahead and then start testing.

So as usual, shall we need to copy our context.

But right.

So that's the more important one.

So we are seeing worsening slash parum slash user.

So earlier one is watching Slash.

You are right.

So now it is Bagram's, so it saved.

So we'll go to over Bowsman and then save the existing one.

Let me close one and I'll save us and I'll say this says request I can say directly parametrized Purdum's

v1.

OK, and let me give the context here.

OK, let me minimize these things.

OK, so Param Sweatman and versioning parents, users.

Slash one zero one, right?

What question mark Watson is equal to one, we can see it here, right?

So let me click on Save and then send it right.

We've got the response and the response.

We can clearly see here.

We don't have anything else here related to address.

So let me change it to two years and then save it and then send.

OK, so you can see where we got the address in Iraq, which means it was my proposal to use a veto

so that the other day to a veto we are getting new Iraq, which is nothing but our address.

So let me change it back to one so you can see here and here also you can see the slide here.

Also, we can define it or we can directly light it here with a question mark.

So let me say it.

One is good.

So let me also say this with so that we have both ready for us.

OK, so let me minimize these things.

OK, so we have that.

And then let me also say it with two.

So now we have both projects, both which was created in Posman also.

And we have successfully tested our request parameter BASAD versioning, OK.

So as usual, we already discussed it very in detail about what is present in this matter.

Nothing.

But we are going we are going to retrieve the user using it and install it in user and in the user.

We are going to pass that as the source for the model mapper and the destination is going to be whatever

the data object we want to convert.

So for each one, which means like for each of the.

Russians, we have this upgraded objects available here for Russian when we have used data were even

and further Russian to use the data will be to accordingly it is transforming and then providing us

the decent results back.

So this completes our request parameter rationing.

So in the next lecture, we will focus on custom header versioning.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 88. Step-04: Implement Custom Header Versioning.md
Welcome back.

In this lecture, we are going to implement custom header rationing, so if you go back to your detailed

steps, as usual, what we have done in our Parum section instead of Pelham's, we are going to have

headers.

So we are going to copy our request parameter Russian controller and then make it as user custom header

version controller.

Right.

And then for the get mappings, they are going to change it to headers and then head that.

I'm going to say the operation is equal to one for the first one and the AP version is going to do for

the second one.

So when I'm testing their Posman, I'm going to ensure that I'll send the header.

Depression is equal to one and then April two to tougher when I'm testing both moved on and then be

two versions.

In addition, we also ensure that our context is versioning slash header slash users for disrespect

to rest controller and then implementation.

So let's go back to our idea and then start working on the same thing.

So let me copy the user request parameter version controller and then paste here.

And the name I'm going to say user custom header Russian controller.

Right.

And then click.

OK, so now I have the.

User, custom header, worsening controller.

So what we need to do, we need to get the part right, versioning headers users.

So this is the one, so I'll copy this vote.

So now we have that things ready.

So instead of bottoms, we are going to set headers, right.

So I can copy the header and then paste it directly.

Right.

So.

Hadass.

Heavenly music, our custom had a municipal version and is a code one for the matter one.

Right.

And for the second one, it is going to be to.

So let me give you some spaces here and then define it does right, and it is nothing, but it is custom

had that sort of versioning.

So I'll say custom header BASAD versioning.

Right.

So I'll see custom Basad worsening.

So now we are going to send the headers instead of firearms from our previous section.

Right.

So in the methods are going to be C and everything is going to be same only in the gate mapping we or

just the headers.

Right.

So can command a command shift f OK just to format the court to look nicer.

So let me see if this.

Right.

So let's go back to our boss man, let me copy the version that uses this context, which is required

for us in the postman.

OK, so let me save my existing postman request, as had last slide.

So I'll say headers and then I will say one.

Right.

And then see.

So now it will be saved in the versioning with headers.

Right.

OK, even so, here, let me remove this and also remove all these things context.

OK, let me say versioning slash header slash user slash and my user is one zero one.

Let me say it here and now let me go to the headers here, because the header section, so what I'm

looking at is a hyphen russianness, my header name.

Right.

Ippei hyphen version and I'll give the values one.

Let me save it and send it.

So we got the response and we can see here we don't have anything here.

Right from address perspective.

Stanfield's we have got it.

So now let me say this veto and then say to versioning and I'll change the header values and then again

save it and then send it.

So now if you see the GSM response, we can see here in the address we can see the you are OK.

So I can also send the user as one zero two from earlier.

We're testing only with one zero one.

Right.

So one zero two.

So we can see NewJersey are we have one more user named.

One zero three and we can see California, he has only one or that, right, so it looks good.

So now if I say the heteros one for this user, so it should not show any hydrosphere that way about

it.

OK, so let me put to save send.

OK, we should be good now.

So this completes our custom header implementation for versioning.

OK, so in the next lecture we will focus on implementing the media type.

OK, so let's reiterate what we have done.

So we have changed the request mapping here and in get mapping we just added the headers with AP Watson

one for the first one and second one with headers with the AP version two.

And then we went back to our postman and then tested it.

So we just replace it with headers here and the header name we have given the customer that name yapper

hyphen version.

That's all we have done.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 89. Step-05: Implement Media Type Versioning.md
Welcome back.

In this lecture, we are going to implement the media type rationing, so let's see the detailed steps.

OK, so immediately portioning, as usual, we are going to create the new media type version in control

or by copying any of the custom header control over the parameter controller.

And then we'll go ahead and then update the mapping.

OK, with this part, OK, which is nothing but produces is equal to applications.

We ended up stac simplified, not even plus Gissen and for the second one it is going to be veto.

Right.

And then we'll go into a lot Posman and then put the header values accept.

Right and tested.

But this value.

So instead of.

Custom header, you're doing it with our acceptation now, so if you see here, whatever the client

who is consuming the service, he is supposed to send disrespect to her like disrespectful value for

the acceptable.

So let's go back to our idea and then start implementing this.

So let me.

Go here.

No idea.

And copy this, had us control, all right, copy and paste it right, and the name is going to be user

media type controller.

Click OK, so now we have our media type watch any controller, so we should have our context also here.

So let me say this as media type, right?

So.

The same year also, it is going to be media time.

So this is our media type context.

OK, so here it is, good.

So instead of headers, we are going to change it to produce and then update our path accordingly.

So let me copy this and then pasted.

So in the same way, Fred, our next method, we are going to also put it.

And just going to change it to veto, right, and this is going to be a media type versioning, so let

me also change that comment.

Right.

So I will say mediatheque worsening, so in this, if you see here, so whenever the user sends the

header, I accept header with this content, then disrespectful version of services sold, which means

user data will move and will be sent in the same way whenever a user sends this meta header in the accept

header.

So user data veto will be sold.

So let's go ahead and then implement our.

Postmen requests and then tested the same thing.

OK, so let's come here and let me see if this is media typewrite, media type V1.

And my this is going to be user slash one zero one save here and let me change this to accept Heather

and my value.

Right.

Well, you will copy from our code here, OK?

So application slash, we ended out stacks.

Simplify that app so you can put whatever you want here, OK?

So if you see that there's an app that are so that as per the latest and just even this value also is

getting changed.

OK, so but for now we can use it.

OK, so this one you can put company or our organization or anything.

OK, so I just killed Stack simplify.

OK, so let me copy this complete stuff.

Right.

And then go here for the accept.

Let me put this.

OK, see you.

And then send.

So I got the one zero one.

So let me take this for one zero three.

OK, so I got the one zero three and I don't have any address field here, right.

So let me see if this a veto.

Right.

Media type written version of my API.

And I also think the acceptable way to apply for me to write and let me send it right now, I got the

address field.

So this confirms that to you.

Whatever we are sending the accept header, OK, if it matches here, then it is going to give us the

exact data for that respective version.

So this completes our even the media type of questioning.

So let us to reiterate what we have done.

Fromentin, if you see here.

So let me go here.

Right.

So these are the complete steps, OK.

So far, we have created a new branch and then we have created two DETI was here, one for user data

will be one and the other one is user data V2.

And then.

We have also created the address, fill that entity and ensure that in that user data or even other

than address, everything will be there and that it will be too, including the address will have the

fields.

So and we went back to implementing that.

You are rationing.

So we have pasteboard with we wondered, you know, we and then we 2.0.

So by updating them in the respect to get map in the area and next we move on to parameter rationing

and ensure that in the get mapping we have added perambulation is equal to one and then Watson is equal

to two.

And for our users, query parameter Russian is equal to one.

And then Watson is called the two.

We have tested and ensure that only for the second service we got the address field.

Then we move on to the custom header versioning in custom header versioning.

Also, we have provided the headers in the kidnapping saying that a Russian is equal to one.

So this area version is called to do so.

This and then in the context also if you see we have sent the header from the postman, Russian is called

one and then AP, Russian is called to two and then Piston.

And then we got the results as expected for one, we didn't get the address feel.

And for two, we got the address filled with ventrilo media type Russian.

By implementing it, we have provided producers' is equal to this applications that we ended up so into

our pipeline we won and then our pipeline between both methods and ensure that when we tested it, the

first one we thought address will and the second one with address will then be sent to the accept header

as this value.

So which means clients are supposed to send the accept header with those respective values to ensure

that the access that respect to API.

So that's about the implementation of versioning and doing so.

Now, when all these are completed, our final step is to commit and push code where I rewrite.

So let me go back here and let me minimize this and let's go together.

So we have saved everything right here in the good staging.

We can we have also made the changes to our data, Eskild, right so far our I just feel so let me push

all these things here and I will say whatshername first comit, OK, and then I'll commit and then push.

So 11 01 Springwood Washington will also be created in our remote origin.

So click next.

And click finish.

OK.

Good, so let's go back to our guest and then also see that worsening first commute.

Good, right?

So here we can see it.

So next in the next lecture, anyway, we are going to do the one zero two, right anyway and Matmata

this with the master.

OK, so let me close.

Instead of in the next lecture, we are going to do the content negotiation.

So at the time, once that is completed completely, one section will map it to the master and then

we really don't need.

So I'll see you in the next section with the content negotiation.

So until then, bye bye.

Thank you.


### Step 90. Step-06: Implement & Test Content Negotiation.md
Welcome back.

In this section, we are going to understand and implement the Springwood contract negotiation, so

this is a very small section.

So they didn't like we are going to test whether our respective sprinkler services will be allowed to

also generate the XML and send similar response or accept the XML as the input furler create or update

requests.

OK, so we are going to test all those things and then understand as part of that.

If you see here, the steps are very simple, OK?

As usual, we are going to create.

Good brunch for the Arab Spring, but content negotiation and in addition to that, first, what we

are going to do is we are going to test our get all users method with accept heteros applications,

assemble and in the same way for our creatives user.

Also, we are going to send the content applications to assemble and then tested.

So if we test one, that should be more than enough because it is going to anyway fail.

So then there will be one dependency in Springboard, which we can use the external dependency from

Jackson.

So which is nothing but Jaxson data format XML.

So we will go and then add this in our palm, that XML and then restart our Tomcat.

So once we restart and then we'll go back and then again start testing Alvira, that allows us and then

create user methods.

OK, when we are doing the data use this method, we are going to provide the accepted applications

like XML and then tested in the same way.

Whenever we use that method, we are going to send the content type applications less XML and then created

the body.

Also, we are going to send the XML body and then post it and then will verify that the user got created

or not.

OK, so let's go ahead and then implement this now.

So let me copy our.

Blanch name and go to our lady flight, so 11 01 is the current branch we are using.

So we are going to create a new branch from that which is nothing but LAVANDERO to Springwood.

Content negotiation, right.

OK, so I will this should be in the starting state, no.

OK, so I will go back to our postman.

Why?

Because the next step is to get us with Accept Araz application slash exam.

Right.

So let me close all these things, OK?

What we're going to test it with our.

Getúlio says we are going to create a new folder here because we are going to change everything to.

Right, so which means our we need a springboard postman's request, say we're here for our future purpose,

right.

So why?

Because we are going to send accept her daughter's application that exam applications less similar our

for our client request.

We are going to send it as the applications letter example for our country, Antipater.

So we will see you for the content negotiation.

Well, OK.

Association.

OK, create.

Let me make this simple right and request, and I will say that all users OK and Sue.

All these are a little uneasy, but that's fine, OK?

Get all users from opening continuously for us, right?

So let me send close to users and then see.

All right.

So first, let me send it and see the response.

OK, good.

So that pubis, whatever we have created so far, we didn't touch that user controller too much.

So we are getting the responses as expected.

OK, so now what we will do is like our header, right?

So first we need to add our accepted header application slash XML.

So I will say that heteros accept and the value is application slash XML, save it and then send it.

OK, so for 06 not acceptable.

So that's what is their response we are getting.

Right.

So let me go back and then add our dependency.

No problem.

Got XML.

So for disrespectable content negotiation section it is only one change for us from the code perspective

that is also another problem that XML.

Right.

So let me go here and make it bigger.

Will add as the last dependency here.

OK.

So let me.

OK, yeah, and let me save this, OK?

One city saved.

Let's stop this.

JVM.

And start the Davian back.

As we have that changes like new jobs will be added, so those changes to reflect, we need to restart

our embedded Tomcat.

OK, so it started OK, so let's go back to our postman now and then send it.

OK, so we can see our response here back.

Right, so we got the list of users, the item one is user I.D., right item to user data, and then

item three is user 83.

So we have got everything we're XML.

Right.

So let me also change this name as.

Content.

Negotiation and we are getting that example right, so civil servant, all right.

OK, good.

So the next one is we need to create light.

So let me copy one data here.

Right.

So one item.

OK, so this is bigger.

Will copy the third item.

Right.

Which is this one.

OK, so let's go ahead and then create a new request, let me minimize these things.

OK, so I'll see.

What happened here?

Yeah, I'd request and I would say create Mozer content negotiation, right.

You're testing in content negotiation.

This is killing us, OK?

So in great user fustiness post.

And you all is going to be localhost users right from our base, so to steer clear, so the next thing

is Broady.

So from body perspective, we'll see the and then copy the body here.

We didn't get this or I copied it and then prepared it here manually.

So we really don't need use the radio remolded because it is going to alter net and the username we

needed.

So I'll say it as user one, one, two, two.

And the first name is user YAF name and last name is user name.

And I can say this says you have name every name at the register, simplify dot com admin and an SSN

one zero three is going to fail because the SSN is the only constraint we have defined in our entity.

So and one zero three is already there.

OK, is this in double one, double two.

I'll be OK and address.

I can give us California whatever it is.

OK.

Right.

So I can leave it as is and then let me copy this so and then go back to our postman.

Right.

So let me copy it here and once you and know what we are sending, the thing is XML application slash

XML flight and from content type perspective it auto selected.

Right.

Whenever I said here xml application slash XML.

So let me save it and then send it and see what happens.

OK.

OK, so one created.

We got the success response.

We'll also see in the headers the location header.

You can see it here, road users and then slash one is missing.

OK, so this is because of this is one more bug which I want to fix it in this respect to branch.

So that is because what happened is.

During the process of our implementation, incremental implementation, if you remember that we are

doing the hopeless implementation, so the idea, right long idea is changed to use aready because in

the hato is one of the libraries we have seen that we have a conflict, that this idea and then whatever

we define and in the research library where we have seen the idea, we are having the issues OK, and

it is not happy with that.

So we changed this name to user lady because of that.

So because of this in our country.

Letellier Right.

So I'll go to our comptrollers and then I'll go to our user controller.

OK, so we changed the user idea in our service layer as required, but in our controller, layer it

for the builder.

Right.

So for the Head Start set, location builder part will build and expand.

It is like good idea only.

OK, so that's the reason it is feeling OK and it's not giving the right value.

Good user data should be there here.

So let's put this OK and then save it.

OK, so now when we started Maddieson user might have gone.

OK, so let me send it back again.

OK, see now we have fixed our bug which we have seen also.

OK, so user slash one.

It looks good.

OK, and it created let's go back to the users and then send it and then see that the first user came.

Yes we got it.

OK, I did one and then used one to two and that whatever we have given SSN one one two two.

We have got it.

OK.

So if you want for our convenience we can create one more user.

OK, so I'll see two zero one and SSN also is the only constraint we have.

The issue right now is like not issue.

We define it as a unique constraint.

Rightside also define this all says yes to zero one.

So and then let me send it, OK.

So it has created and we got to use it as two and two zero one created.

OK, so let me search it now.

OK, using the all users use that one is there and then we also get the user to zero one.

So this confirms that our respect to the services are also accepting the XML based or instead of dison

now that using the content both in and then out with XML.

So we have seen everything in doing so related to reiterate what we have done.

So from the users perspective, we have to accept Hydra's applications, XML and then we have tested

it before adding the respect to.

Library, the library name is Jackson Data Format XML.

So before this, what we have seen is it is not working and we have got some for 06 not accepted some

error.

OK, so now what we have done is like after adding that, so we have got the proper response.

So then we went back and then created the create user we have created XML responded by copying here

and as we don't need the user ID, so we removed it because it autogen IT and SSN.

It is a unique constraint.

So we ensure that whatever we have the data in our system properly, the data and your decision is with

a different name.

And then we created the content and then then put that idea in our postman request and then added the

data.

And then Senator, the content applications XML, which are populated here with headers content, is

equal to applications less XML and then we have sent it and the user got created.

So then we have seen the status quo to zero one created.

But in that area we have seen the location header with all the.

Heidi, so which we went back to our user controller and then fixed it, which word this Bob got created

during the Hatteras implementation.

So we have fixed it now.

So this completes our content negotiation section.

So in next section, we'll come up with a different topic.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 91. Step-07: GIT Commit Code & Push for Content Negotiation branch.md

Welcome back.

In this lecture, we're going to complete our committee push and then make the things normal from get

perspective, right?

So we have completed our country negotiation section just now.

So we need to push the content.

The content will go to good standing.

So primarily we will have to endure the problem that axman in addition to that, as we are fixing one

bug which created as part of its implementation.

So we have also fixator that.

So I'll say content negotiation first come.

Right, so and then I'll come out and push.

In addition, we have also fixed one more, but that's fine.

I could commit and then.

Whoosh click next.

And click finish.

So this should also create about 11 zero 02 Springbroot under negotiation in our the report also.

So let's go back to our gut.

So we have this let me close these things closer.

OK, so now let me open them, master.

Right here, we have already had brands created.

So let me check with the local master.

Right.

So let me also start the journey and we don't need it so from our local master and say much and local

master Robert Maginnis, Lawrence Springborg, content negotiation.

Right.

So let me add to that.

OK, so I have it right.

So let me refresh to see that touchiness reflected.

OK, you can see it here to continue negotiations nine nine six seven F six is the same year C nine

nine six seven five six.

And coming back also you can see containerisation first come in.

So now let me also push this to a remote branch.

Right.

So I'll say push and then Proview.

And then I will push it, see?

So push completed and we can see the change in our origin, Master.

It looks good.

OK.

Meantime, everything from the IDL ones will go to a Web browser and also ensure that we are bought

from all branches perspective.

OK, so we have the branch, the springboard building blocks in our GitHub slash stack.

Simplify, right.

So I'll go build.

And if I see here, my masterbrand, OK, just now had a saying content negotiation first come two minutes

before.

Right.

And I can also see all my other branches here, one ground zero zero two Hollowell G.P.A. exception

handling validations, SpongeBob, probably one too many Springhill to bring international utian spring

filtering spring filtering with mapping the and values springboard filming this and View and Springwood

model Mirpur between some abstract springboard versioning and then Springbroot content negotiation.

That's very nice.

Which means every section, whatever we have implemented all we have the blanches here so any branch

we can check out and then test for that respective functionality.

Very good.

OK, so.

I'll see you in the next lecture.

Until then, bye bye.

Thank you.

