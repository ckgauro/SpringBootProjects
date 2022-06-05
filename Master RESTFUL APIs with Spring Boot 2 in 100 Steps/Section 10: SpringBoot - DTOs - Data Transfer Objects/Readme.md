### Step 77. Step-01: ModelMapper Introduction.md
Welcome back.

In this section, we are going to understand and implement the divorce using model Mappa so that most

for data transfer objects.

OK, so exposing identity objects to resting points can make security issues provided if you don't take

enough care about which entity forms should be made available for publicly exposed missteps.

The library, which supports to convert into objects to be diverse and also be transformed into the

objects.

So intelligent, insightful, but there is no manual mapping needed, so when we're using it and automatically

projection when it flattens the complex models, whatever we have.

So it's also refactoring safe.

So a simple flying paper for handling special use cases.

If you have a different model for entry to detail conversion, a conversion perspective, the APIs,

typesof and also refactoring.

So if you see here, it's a conventional convention model.

So model map approach predefined conventions and if you can also create his custom conventions if required.

So it's also extensible model, motor support, integration with any type of data model.

In short, model mapping does the heavy lifting for us.

So from the forensics perspective, we can talk and model that are getting started for an additional

understanding and documentation perspective.

So the implementation steps, the Swiffer model, Mappa, so fustiness, as usual, we're going to create

a new plant using Idy for our model matter implementation.

So and then we're going to add more than dependancy from that XML that will go into a core implementation.

That is.

First, we need to define a model Napperby config and then annotated with a do put it in context.

So then one more detail layer.

So which means like we're going to create a new package database and under that we're going to create

a new class with names user.

And so just to identify, we can directly reduce the debt.

But in our next leftest, we're also going to implement the similar type of model method implementation,

which is nothing but abstract.

So I really don't want to have different, different things, which means we really don't want to have

a single thing used for implementations when it's for more than apparent benefit.

Mastech, so that's the reason I'm getting closer to a meteorologist Zimmermann's model Knepper in the

same bed in the next section where we are going to deal with an abstract for the same type of detail

to entity and entity to detail conventions that I use it.

Yes.

So Emmis means map stability so far that what changes are required in order to be there and then here,

whatever is required for this respective model, Napperby will remain with you.

So if you see we're going to create a different package under which we're going to create user data,

a file and from controller perspective.

So what we're going to do is we're going to create a new user model, better controller and copperplate

usability plus from our regular user controller and then implement the model metallurgic, whatever

is the conversion logic we're going to implement.

Finally, we're going to test it and then come out and push it.

So let's see one more time the detailed steps from a federal court perspective.

Right.

So here are the steps serpens unspinnable to this model.

Knepper So if you see here, the first thing we're going to create with branches in Nidhi and then we're

going to implement, it works for the user entity using model Mappa.

So we're going to update the bombastic symbol.

Right.

So this is update from the XML.

With more than Mirpur dependancy, later, we're going to define moral Napperby conflict.

So we're going to create a conflict package, conflict class and then define model Mathabane in that.

At the same time, after that, we're going to create a bit of a class with who's was right in the name

fields.

Once those two are completed, will go and then move on to competing in the country.

We could use a model map or controller and then annotated with the rest controller in the request mapping

at the class level.

We are going to give us the services.

We are going to have as model maps, users, users, if you see here.

So I have organized all over the place whatever we are creating as part of this project like this.

OK, so your basis initially, whatever we implement to get all users created will create order based

usability and all these things right after that.

When we're doing the implementation, we are in need of creating a different context with different

controllers.

Right.

So we have to do these things there.

So this is the same way for internationalization.

So in the same way for filtering.

We have done these things for the assembly and then mapping Jackson.

So in the same way, no further details.

Also, we're going to have a separate from the here and then we're going to create a model map related

to services, whatever we're going to build in that folder so that this of package Posman package you

can input and then you're in your Posman client and then use it whenever we're implementing the course.

So we are going to create a separate contextual model map of users and then implement that which is

a bit of a bad idea, and then implement the model mapper little there and then best using replacement.

And then we want to to the corporate idee.

So that's all we are going to do, step by step process.

So we are going to implement everything in six steps.

OK, so excluding the additional steps which are the latter two, step one and then step six, which

are the letter to commit quality to it.

So you can say two, three, four, five, within four steps you are going to understand and then implement

a complete model mapper.

So I'll see you in the next lecture, basically going to the idea and then implementing it.

So .

Thank you.


### Step 78. Step-02: ModelMapper Configuration Setup.md
Welcome back.

In this lecture, we are going to create a new good brand using idea and then add model, no dependency,

no problem, but axman and then define that model Mathabane inner conflict.

So these three steps we are going to implement in this respect lecture.

So let's go back to the idea.

You know, so we have already seen a lot of steps, whatever required further these three things, one

is branched out.

So if you see here, so you need to create a branch with nine 10 zero one, sprinkled it with model

Malpaso.

Let me go to the idea and let me go to the get perspective.

Right.

So and then in the branches so far, we have completed to do some use, which is zero nine zero three.

So and then it is in the same level.

Right.

So if you see the master in 1987, three one nine four four is the code you can see here.

OK, so now I can create a branch from Master stating 10 zero one springboard to this model mapper.

Good.

So I created in the local what checked out.

So I'll go to the general perspective now and then I the next step is to implement that XML.

Right.

So let me copy the dependency.

If you see here the dependency or that model, mapper the group.

And then I perfected his model method.

And I want to be like the latest version is three fourths of you are using the same putrefy version.

No.

So let me copy this and then go back to undertake a similar project or kespin the building blocks.

Let me make it bigger and I'll go down.

And after this, what started this dialogue at the end so that we don't have any issues.

So.

Let me say it, OK, so rather than dependency, let me go back to our steps, so now we are going to

convert the modern Napperby, right?

So which means we are going to create a class package config and then add conflict class.

And then they just added model Mathabane with it.

That had been annotation.

So what I'll do is I'll go here.

I minimize this.

You go to source main Java, I'll go to stack, simplify the services here.

Right, click new class.

Right and lasciviousness.

What I'm saying is I'm going to create a package named.

Config, right in config package.

What I'm going to create is my model Mirpur config so I can say that you and I have configured I can

even say model Mirpur config, so I'll set up config, OK?

And then I click on Finish.

So my app config file, God created light.

So anything configurations in spring we need to annotated with configuration related threat configuration.

So coumarin shift in our makk to improve the package.

So finally now we need to create a building for model Malpaso al-Said Public Model Mirpur.

Model Mappin.

And I'm going to return the same.

OK, so come on.

You've got to import the model mapper so we can see here that model, my product model, Napperby imported.

So I'll return.

And new model.

Mappa now let annotated with a direct beam and then come, you have to put the bean related package.

So let me save it.

OK, so this completes our app configuration.

So the first three steps, which is creating the good plan and then updating the Pontotoc Saiman and

also updating the creating the config package and then config file for our model Mappa and then reinstalling

the beam.

So in the next lecture will focus on other steps.



.


### Step 79. Step-03: Implement Methods using ModelMapper.md
Welcome back.

In this lecture, we're going to create a bit of a layer with the user class and we're also going to

work on the country level by creating a new controllable user model Malpas controller and define the

model metallurgic there and then test everything and then come out and push the code.

So if you see these are the detailed steps which you going to implement.

So first thing is to create a user.

Remember that you class.

OK, so let me go back to the idea.

And here I'll see in the main package area services science class and the name is user name.

And in the package we're sort of created create this bracket and then it will create the user and then

it you'll let me finish this.

OK, so now we have the video.

So if I see here in our existing entities, we have the user.

Right.

So in the user you can see that we have a user, 80 user name, first name, last name, a lot of stuff.

OK, so far this respected model matter demonstration will just try to use user and user name.

So I'll go and then say private long user lady named.

Private string username, so undescended the Gators inciters required for this source generate getters

and setters and then select all them gentled.

So this completes our.

Digital creation, OK?

So now we'll move on to the next step.

So the next step is to create a new country.

Let me introduce user model, map controller.

Right.

So let me come here.

So.

Right, so here we can see the controllers new plus and then created Model Noppen controllers.

So as usual, we need to define it as it must controller come and shift to implode.

And we'll also see request mapping.

Right.

And then request mapping.

We are going to say that as a model mapper slash uses.

So that is going to be our context and.

You've to import our package.

So that said, OK, so now what we are going to do is incorporate user controller and bring the the

operating stuff, OK?

So our primary automatic thing is use service.

OK, so let me get that and then put it here, OK.

So now we'll go to the same user controller and then go down and then we'll find our data useable by

the method.

So we we're going to implement and then test using this respective service.

OK, so I'll come here and then copy this.

So if you see here.

So I believe you can even define the model Nabatean, this aspect, the standard development patterns.

OK, so we need to define our model map related business logic in our service layer.

Right, so that when you are learning and then referencing the code, you need to reference in multiple

places to understand.

So just to ensure better things should be easier than understanding.

So I'm glad that you're defining it in the country layer.

So what I'll do is I'll just remove this and then I'll also try catch block everything here, OK?

So and then I'll say from user surveys that we are going to get the user.

So I'd say user user is equal to this.

So we start good use already.

So it says watching the type of the user to use an optional right.

So I'll change the variable name also to use that optional right.

So now let's implement the exception.

Handling for this user is not found.

Okay, so let's complete that first.

So user optional dot is present, OK.

So if not optional, that is pleasant.

So let's see.

Theroux's new user, not fond exception, and you can also see user, not font.

OK, so that's good.

This one, this looks good.

OK, so also add that to the declaration here, it was a not for an exception.

So now let's go back and then retrieve that user.

Exactly what user object from that user optional.

So user user is equal to user optional dot that will give us the user.

So now let's move on to implementing the model mapper.

Right.

Model number, which means like converting the object from existing user to user dateable.

So Bueso, what we need to do is first thing is to map a model.

Mappa yet.

Right.

So model.

Mappers.

Come and shift to import and also.

Of what?

OK, so now what we'll do is we'll see you a little.

User data is equal to more than a product map, right, and we need to provide our source and destination

right.

So my source is going to be on this user, right.

From user to I'm mapping it back to their destinations.

Destination is user data about.

Plus, OK, so come on, you've got to import the user, did you write?

So we don't have a user data.

All right, so we have implemented user MDT well, OK, so let me also give the same OK, and then import

that package so it literally nothing but.

Admiral Napperby to object, OK, so that's good.

So I'll also say, here you go, sir, I'm OK.

So now we have completed the conversion so next year to return that flight.

So return you, sir, and get you right.

And when we're returning.

Obviously, this wouldn't happen through there because here it is optional.

So let's fix that, OK, so we can fix it.

Your team method written by user random Nativo.

OK, so this completes our model, my personal conversion.

So it's only Holomisa and he had lines on the right, so only one line.

So it says that.

More than a map of that map and provide the source and the destination sources are the subject and the

destination is Richard Metuchen with that is nothing but user data, a dot glass.

So that's all.

So it's only a one lane to convert from.

You said to him, did you also let me save this and then let me start our application?

So as we have added the new package named the map model mapper, already aware of our American, that

in start date we need to ensure that we to restart that one so that new job files will be reflected

right when we added when we do any changes to the bomb and we add new libraries.

OK, so that's one thing.

OK, so if you forget this again, you'll be troubleshooting with different details there.

So that's the thing.

So now we have started it and we'll go back to.

Posman.

OK, so I'll create a new format for this, OK, so add that here and I'll say the four leaders meeting

was that so create.

Let me minimize this.

So in divorce, I'll create a new request, so the request name is.

Giddap.

User.

By I.D. and with the map.

Right, so safe to do so.

Let me minimize this.

We don't need this and this is the one and I'll say localist and what we're going to say here.

Model Mappa slash user slash one zero one mark and then send it.

OK, so we've got the response, you can see it here.

So you've got one of musical Chiaretti.

So if you see here, it is the same thing, right?

So whatever.

No.

Let me open our user MDT, so we have defined the things you wrote in the user name and then we got

the same.

So let me add one more here.

OK, so private string, Alsi first name, Adonal.

Right.

So.

And then also had the excellent getters and setters, OK, so set the tone and then generate blood and

then save it.

So we have saved it.

Now let's go back to our postman, so we've got my first name also.

That's all.

So which means now we really don't need to change anything at the entity level in the sense like any

changes to the core entity where we have multiple services exposed.

Right.

It's going to be a big thing from development effort, perspective and then testing and then talking

to the people.

But if you see if you are going to change it, respectability, which means like this picture of you

like this respect data, all the data will be used for only Swayne.

So get all the service out, get ABC service or whatever it is.

Right.

So now if you change that data, then you need to test only that respect to service zero breakage.

But if you change the entertainment entity is exposed for the services directly, then you need to do

all testing for that entity with all the services integrated with that.

So like this, there are multiple things come into the picture if you don't use the data is not only

from security but from a maintenance perspective.

To solve it is to use the tools.

So that citizen is I have of this also like other types of data, will mappers be available in the market

and then how people are using it.

I just read those two things in other quotes.

So let's also add one more.

Right.

So we have something called orders, right?

So let's add that and see what happens.

So list.

Provide a list and then it is order and orders.

OK, come on, shift o entity orders and NWT list, let me say this and then here, let me add that

getters and setters for the orders so that in order to deploy along too many S. we have either the orders

in our user entity.

Right.

So we are mapping that here in the B2 object and then see what happens.

OK, I select orders and then generate.

So we have generated the waters and certain flood orders.

So let's go back here.

So we can see we got the response back.

OK, so I'll see one zero and I got the response was that it was an embarrassment.

And also the orders.

So if that's all OK.

So more than that, it is going to be pretty easy to implement and we're going to get whatever we want

from data was perspective.

So now another important thing here is like whatever I know, it's like when the very, very complex

scenarios I have heard that people are having issues and then they are slowly migrating to abstract.

OK, so what is the very latest and with which auto generates everything?

OK, so we really don't need to worry about the multiple things there.

OK, so let's see how it is going to go in our next section, ok.

So, but it's our chance to use that model, my partner or my stepdad, whatever we want in the market,

multiple things are available, but these two are in a high trending area.

So that's the reason I have included these things in our courts.

So we have completed the complete changes related to.

Model Maponya.

So what we need to do as a lasting so we just need to go to good staging view here and then.

Push them here and then say so, um, uh.

Model Mirpur first comit.

Come out and push.

So this will continue the branch you never.

GitHub repositories tax simplification, springboard building blocks, and this project is exclusively

dedicated for this cause.

So and then are integrating it with our Ballymun at an incremental manner.

So which means any time you can check out this list, but to brand and then test it or the tester features

whatever we have implemented and then understand those things.

So I'll click on next and then click on Finish Load.

So it's pushing it.

So we have completed our commitment and then push step, so I'll see you in the next lecture in the

next section with our map step implementation for the date was so.

.

Thank you.


### Step 80. Step-04: MapStruct Introduction.md
Welcome back.

In this section, we are going to understand and implement detours using Napster.

So Napster is a code generator that simplifies being mappings.

So mapping classes are generated, a compilation and more runtime processing.

That reflection is used here.

So mapping classes use simple method in location, which makes them really easy to debug.

So we generally notice a lot of boilerplate code converting pages to other products.

So very common type of conversion we see regularly is in between persistent backed entities and data

that go to the client site.

So the problem Napster solves is it can generate between upper classes automatically.

So if you go by implementing those been upper classes manually creating being Napoli's, the time consuming

process, and here with Napster, everything will be very much automatic.

So Napster, it also requires a processor plugin to be added to the problem.

But in addition to collector dependancy, so the Napster process is used to generate the matter implementation

during the build phase.

So let's see the series of steps we are going to enroll in Napster implementation.

So as the first thing we're going to create, they will get Branch using idee, as usual, for all of

our steps.

OK, so I'll take the pragmatic semmelroth, necessary dependencies.

We'll see what are the dependencies in a lot of detail steps.

So then we want to create a new user and data, a class record for mousetrap implementation.

If I see here, user and data is nothing but user maps that do so to differentiate our user.

And it is nothing like model.

So we are seeing this as a misleading and we are going to create the abstract mappa interface and then

we'll create web services by calling the method defined in my abstract mapper.

So in the abstract Mappa interface, we are going to define the method and those methods.

We are basically going to call from our controller area.

Finally, we are going to come and then push the caller ID.

So if you see our steps here, right.

So step one is to convert it into the Springbroot Matchstick branch and then they'll go to a letter

from that example and then add the properties for our abstract version and then Aperture now and plug

in version for Mastretta processor.

OK, and then we will also use the one three zero final, the current version, which is going on with

the map struct.

And we are going to also add the maps that dependancy and we are also going to add more abstract processor

plugin.

So in our total plan that XML, we are going to make three changes, OK, and then go to the step three,

we will create a of class and then we'll create our fields and then we'll also create an argument and

then fill constructors and also generate the data centers.

So then we'll move on to step four off map Strittmatter interface.

So in the map and interface, this is a key thing now.

Okay.

So we are going to create the interface with methods for mapping between objects.

Okay, so we are going to annotate our Mappa interface.

We will create a map and package and inside that we are going to create a map interface and that neighboring.

Our map interface, we are going to annotated with maps.

So then they will configure the maps to use spring dependency injection, so then we'll move on to nothing.

But we're going to add a component model with a spring as the string.

OK, so then we want to create methods, which is nothing but user to use a dual.

Right.

So this is first method we are going to create and one another user to user details.

So far, the improbabilities going to the user and the output object is going to be user remise.

DTL So in addition in know local select no exact user entity.

We see the name as e-mail and whenever we're creating the data, we'll give it to us email address so

that we also understand about the mapping annotation available here.

OK, so in the source we have the email and then the destination.

We have the email address so we can map that on top of things like we can add the sanitation on top

of those respective methods so that this email to your email address will be mapped accordingly.

So there will be some situations where our data addicts need a different a few names instead of whatever

is present in the entity.

So in that case, that's how we're going to use the mapping.

And when using the maps, truck mapping annotation, how we are going to use when we're using maps,

we're going to see that.

So this is for our user to use the data.

We can say that to get usability, you can use this one or create user.

You can use this one.

Right.

So why?

Because it is its user object.

OK, but here, if you see it is like you said, you said it was nothing but a list of users.

So input this list of user and all the stuff that I'm listening to us.

So which means it is for all users method in our control.

So these two things we are going to implement in detail and understand much more effectively.

Additionally, we are also going to see the mappings, which is another additional feature for mapping

the source and destination letter fields with the different name.

So when they have different names, so finally we are going to create a service and build even better

service.

We are going to offer better service.

We are going to create a new user maps that controller so that all maps regulatory implementation is

separate for us.

Right.

And we are going to propagate user by user methods from user controller and then implement them effectively

in relation with other users, what we call integration with our map interface methods, which means

like in mapping interface, these two methods are that we are going to call when we are implementing

these two matters.

Finally, we're going to test them and then commit and then push the code where Iot.

So this is what we're going to implement for the entire.

Mousetrap implementation, so let's go ahead and implement that now, so I'll see you later.

.

Thank you.


### Step 81. Step-05: MapStruct Configuration Setup.md
Welcome back.

In this lecture, we're going to create a new good brand using idee, and we're going to update the

problematic symbol with necessary dependencies for map abstract.

And we're going to also create user data for plasticware, for map implementation.

So all these three things we are going to implement in this respect lecture.

So let's go back to the core steps which we have defined here.

So let's start with 13 zero Springwood.

That is an abstract brand creation.

So let me go to the idea.

So let me go here.

If I see here, I have the model map.

But OK, so those changes computer and then we have committed the code.

Let me close all these things so we create a new branch from Model Mapper because that is the latest

road.

So I'll send you create a branch and then I'll see 10 to spring.

But it was my abstract implementation.

I said finish and then continue.

Right.

So I'll stop this and then restart once I read all the plan that simultaneous are completed because

it is going to add new job files and then if you forget to restart it, then we will have multiple issues.

So let me stop it, OK.

So now we have checked out the map struct.

Branch, so let me go back to over Java, right, Java perspective, so our first step is to go and

update the plan that simultaneous.

So the first thing is add properties, right.

So let me copy this and go to the.

Thrombotic Semon.

And what I'll do is the first thing is to add the properties so I already have the Java property here,

so let me put the cursor here and then paste it.

Right.

So let me remove these things, OK?

Why?

Because.

Yeah, so now we have added the maps clipped version and also the map and plug in version.

OK, so might be three eight one not there.

Let me see your Katmai to another, but we'll see how it goes.

OK, so the next is at the dependancy maps track dependancy.

We can see our maps checked and maps to for Kate and the Russian it is going to pick from our properties

folder.

Right.

So let me copy this and paste it at the end of dependencies.

So we added earlier model maps.

So now we are adding.

Mobster dependancy.

So we completed the maps that dependency.

Currently we have in the plug ins area, we have a springboard and plug in only one plug in, right.

So we are going to add one more plug in, which is required forever, which is nothing but the abstract

processor plug in.

OK, so I will take this and then copy it and then.

I will put in terms of Kesari.

The culture are here and then pierced it, so now I have added the more abstract plugin also.

So let me save it.

So if you see here for the Malvin plugin, it is throwing the right thing that we have already managed

to create one firmament plugin.

OK, so I'll say.

So and this, in a sense, like the Russian declaration, OK, and then say, OK, so that's good.

So let me go back to our steps now so I have complete change.

One change to and then change.

Three, change.

One is our properties.

So this property is irrelevant for us, not currently change to some abstract, which is nothing but

the abstract dependency we added.

And the change today is an abstract process plugin.

Also, we have added successfully.

So now the next step is to create user dual class.

So let's go ahead and then create that.

OK, so let's go back to the idea and then in the detail section, we have user MDT, so we are going

to create a new class user in this video.

It is more abstract that you write.

So we are going to say.

Robert.

Long U.S. lady and private string username, and we also discovered that we are going to add a mapping

annotation when we are implementing the map interface so that e-mail address in detail will be mapped

to e-mailing our existing user site user entity.

So I'll see private string.

al-Saadi says e-mail address.

OK, so we have defined the three fields here.

So in this respect to the two object, so I'm going to gender equality getters and setters, right.

So select all getters and then generate them.

So I will also generate.

OK, no argument.

Constructor so constructed using full time generating.

No, I will also generate no argument constructor.

So let me do that now.

Right.

So here I am and then source and then construct them from superclass, right, dendrite, remove these

things, OK, and then save this.

OK, so in this lecture, what we have done, just to reiterate what we have done, so we have done

three things.

So one is we have created a branch required for this master.

We have made the problem that simultaneous three changes in that one is adding the properties with Martian's

and adding more abstract dependency and then adding more abstract process plugin.

Finally, in the step three, we have created the user Nativo plus required for master implementation.

So we have ensured that here the string e-mail address is with a different name here because in that

user we have the name that email so that we can use the mapping annotation and even test the mapping

annotation so that.



.

Thank you.


### Step 82. Step-06: MapStruct - Create UserMapper and Implement getAllUsers Method.md
Welcome back.

In this lecture, we are going to understand and then implement the following three steps.

One is clear, the maps try to map out interface and then we'll move on to once the interfaces that

will create the equal interest services and then calling them methods defined in this map interface.

And then we will test them and then committed posterboard.

So all these four, five, six, these three steps, we are going to combine into a single lecture now.

So in the years code, we can see those steps in detail.

Okay, so this is step four to create the magic map interface.

So let's go ahead and implement this step now.

So my mapping interface name is User Mapper and I'm going to create a map of package now.

So let me go here.

So the PWP created the database, right.

So now we'll go to our.

The services, your main package, and then see a new interface, so we are going to create a new interface

named User Mirpur, right.

And I'm going to create that inner mappers package.

So I'll click on Finish.

So first thing you store, I'm going to put the Mappa annotation and then caecum and shift over to import

the package.

So our abstract Mappa package got imported.

So to satisfy the spring dependency injection.

So I'm going to say component model.

Is a cold spring, right, so that looks good.

Let me save it.

Now we are going to define two things.

OK, so before defining them, we need to create our map, for instance.

Okay, so user mapper, I will say this as it stands, is equal to map a start, get Mappa and use that

map or dot class.

Right.

So now I have created our map, for instance, and I will create the two methods.

So one method is for either a regular user object.

OK.

OK, so I'm doing to get service.

Right.

So which means like from user to user data so I can see.

User to user data, and the second is a list of users, right?

So a list of users to list of user data was right.

My data on user enmasse.

Did you vote?

Yeah.

So we need to do user to user data and then user to list of users to list of user.

I must do.

So let's do that now.

Right.

So let me create our first method that is so true.

Tintype is going to be user data.

All right.

So we have the two method names defined here.

You can see here.

Right.

So user to user data will.

So I'll say user to user data.

And so what are the parameters?

Which means what is the input for this?

We are going to provide the input as user and then output as user data input is going to be user.

Right.

And we can do any variable here, entity Y because user is entity.

You can even say does entity also or you can see user, user, whatever, it is convenient for us.

OK, so now we will also say it is user and mass data will always.

I forget this.

OK.

OK, so that the naming convention will be good for us, OK?

Yeah, so this is good.

And then let me also introduce a package that looks good.

So now we completed the.

First one, so now the second method, so we are going to convert users to user data was so that's our

method, right?

So which means we need to get the return type list of user hamis data was faked, user did videos and

the method will have.

List of users right here, I can say it as entity or even the users, whatever I want to something,

and then let us import the Java util list.

So we have completed creating methods now.

OK, so let me save these things, OK?

So this completes our.

Maps that map our interface creation, so we'll go back to our next step, which is step, right.

So if you see step forward, we have created a user interface and it with a direct mapper and to satisfy

the spring dependency injection.

So we have also user component model and then added the spring there.

OK, and then we have created two methods.

One is user to use additive and the other is user to users dual.

So user data was OK and we didn't add this for now currently.

So we will add it later.

So what happens?

You will see and then add the mapping later, OK.

So if you have multiple mappings, what we are going to do also we will see.

OK, so that Fano will step Face-To-Face to create the list services by calling the method defined in

the abstract map.

So I'm going to create a new user map struct controller.

Right.

So let's go back.

So you're.

And we'll go to our comptrollers section.

A new class and alsi username abstract controller.

So first thing is to create it as it the controller and I will also say request mapping and I will say

an abstract slash user's comment of total import, OK.

So now we are going to define two methods here.

My abstract controller.

Before that, what we'll do is we'll operate our user repository, user repository.

Right, and then there are two world coming on.

All right, so the next year, we also need to upgrade our user interface, what we have created just

now.

Right.

So we will also automate that right to what I mentioned to import.

Right.

So now finally, we have everything ready.

So we need to create two methods.

One is get all user details and then get all users by user.

Right.

So those two methods we will implement now.

So let's start with creating the list of user slide.

So we'll start with that for now.

OK, so I'll set list and then user data will.

So, as usual, I made a mistake.

It is a user and must do so.

My name is User and messaged you.

OK, and then let me put both the things that.

So, Joe, are you to list?

And.

Import that must do so, it'll get all user data was.

Now we need to return the users, right?

So let's start with the user mapper, Dot.

OK, so we have the list of users returning.

We have one method inside where users to user data will.

Yes, OK, so I use that and the input should be a thorough list of users we need to bring and then

send it to this respectful method.

So I'll say.

Use a repository, but find out.

OK, well, we'll get me the list of users and that I am going to pass through the m'appelle interface

and this will convert and then send it as a list of user names data was.

So now this is going to be a request once we get mapping.

And Comanche's, total important one, so, OK, so important.

So let's go back to our postman and then test this right.

So let me copy existing elsea new request and request and I will say get all users from abstract.

Right.

And let me minimize these things.

So we are here, Getúlio, this abstract and our thing is localhost and we need to see a map struct

slash uses map SWC is slash uses, that's all.

So they use this method.

Right.

Let me see it and then send.

OK, so we got the response successfully, which means our transformation worker.

So it brought all the users and then sent with only user data username and then email address.

Now what we need to do is if you see here, email addresses null because if you see in the.

User, you have the email and in the user, unless you have the email address, so by default, implicitly,

it doesn't matter because we have the difference in the names.

So what we need to do now.

So we need to go into our Mappa and then define the mappings.

Right.

So let me go to the Mirpur and we need to define the mappings in our entity.

Right.

So here, which is nothing.

But if you define here, it will be applicable for Distel.

So I will say a delayed mapping and we need to say target is.

E-mail address, which is nothing, but I can even say email address I started and I can even say a

source here, quote sources.

A.M., right?

Good, so sources e-mail and then target this email address and also let me put a mapping from our abstract.

OK, so now I have computers or mapping sources called e-mail and then target to email address.

Let me save it.

OK, so let's go ahead and start Getúlio, this one more time, super.

So we said Kennedy addressed to simplify dot com divide the reverse tax, simplify dot com b mark.

We are getting all the email address for the three users which are present in our history database.

So this completes our recreation of how you get all users matter using the device and then model Mappa.

So one thing here is now you have one thing.

You have mapped it.

If you have multiple things, what we are going to do.

Right.

So let's also complete that before going to get usable ID to you.

Right.

So let me say that I have something here called OK, private string of.

All right.

So I'll say here, real name, but there it is rule.

OK, so I'll say C so I'll regenerate this one.

At least under the rules constructor.

Right.

Source and gingerbread constructor using fields.

OK, so I have also out right now.

So now I also attended the getters and setters for the real name, right.

So gender getters and setters and for the real name, we are generating it generally.

So now you have the name also added here.

Right.

So and then there it is.

Rule.

So let's go and test what happens.

OK, so a name is coming null and we are going to define multiple things here.

That's the important thing we are seeing in the user map.

So what we need to do is we need to see it.

Did it mappings?

And let's open it.

And.

We will.

Close it so we have to find one mapping.

You've got to import the mappings from abstract.

OK, now will they find one more mapping?

Seeing source is equal to what is that?

It is all right and the target is equal to fullName.

And then see, so if you have multiple mappings, what we are going to do, we are seeing now.

So let me see that we got that.

All right.

So that's all.


### Step 83. Step-07: MapStruct - Implement getUserById Method using MapStruct UserMapper.md
Welcome back.

We are going to keep it getting better for details.

OK, so let's go ahead and then create that.

No.

So here.

So let's go to user maps, traffic controller.

So we have created so forget all users.

So now we'll create our get usable idea.

Right.

So.

Public, so what are we going to return?

We're going to return in user.

And Miss Lady will back, OK?

And then I will say get you there by Heidi and the input, what we are going to take is already right

but variable and then longer and then, Heidi, come and shift.

Oh, OK.

Apart variable is important.

So now first thing is to.

Get over it first.

OK, so I'll say user user is equal to the user repository dot.

Fine by me, OK?

And then whatever I'm passing is pretty good.

So now what happens is.

We'll give the user.

Let me put the user here.

OK, and now it should be user optional played, so let me change that.

So let me also change the variable name also to user optional.

So now my user is in use.

That option I look at to get the exact unit object.

What we need to do is.

User user is equal to user optional dot dot user.

OK, so I'm not implementing anything here related to.

If that exists and then what should I do, all those things, OK, even we can implement those things

right now, you're OK.

But for now, we'll leave that like that.

First of all, fix these things.

OK, so then we need to return, right?

So what we need to return.

We need to return the user MSJ to you.

So from user my product.

So this is the end user to demonstrate to the user.

Right.

So this method we have defined in our Mappa interface user interface.

Right.

So we need to parse the user.

We have the user here.

I am passing it.

OK, so that's all.

OK, let me save this.

So now we have completed the user by the method creation, so we need to annotated with good mapping

and then provide that I.

Right.

So let me send out as the best variable, so let me save it.

OK, so just to have a little bit more, you can add if you are optional, that is presentments they

give you that is not present, then throw the other and all those things.

OK, but for now and see how it is behaving.

OK, so I am not implementing any exception handling here, just trying to understand and then implement

maps to use map or whatever we're creating here.

OK, so let me go back to the postman and let me create a new method here, OK.

So I'll say and request and I'll get you there.

But Heidi, this is for an abstract right map abstract.

So let me minimize these things.

We don't need these.

Yeah.

So get usability maps trip and I will say localhost.

And here is the map struct.

Right, Sue, so slash abstract slash user slash one zero one.

So let me send this, OK?

So I got the details.

So one zero one cariddi transcendentalism.

So we have successfully implemented the.

That are already using the.

Mappa user, Mirpur, what we have created.

OK, so this computer, the usability implementation, so let's see what we have done all together.

OK, so we have started with creating a brand.

It was abstract and we have created three things here, OK?

One is in our palm that XML.

We have created our version properties, maps, drug dependency and abstract processor plugin.

OK, and we went there and then in our idea we have created the user emsley to class, which is nothing,

whatever detail class, and then define the variables there, which is like user user data, user name,

email address and then role.

And then we went back to the fourth step, which is nothing but an abstract Mappa interface mobster

map interface we have associated with a direct Mappa.

So we have created the interface associated with Mirpur and to satisfy spring dependency injection we

have added the component model is called the spring here.

We have created our map, for instance, here first to initialize our mapper and then we have created

over user data.

User to user data will matter.

One method and the list of users to list of user data was one more method defined those methods.

And finally, when we have an issue related to mappings, when there are different names in our database,

how to map it, we have seen multiple mappings, how we are going to do it.

This is about the user, Mappa.

We went back to our map struct controller and using the user map we have called.

Our methods are defined in our user map, but user Mapplethorpe method defined in our use of mapper

and input we have provided using our user repository.

Those were converted and then when we access to via Posman.

So if you see the data, we got the successful results in the same way when we done the get usability,

we got the successful results.

So this completes the map struct implementation and doing okay.

So now our final step.

Our final step is to check in the code and then push the code.

So let me do that now.

So I are good staging.

So bring all these things to the stage changes and I will say.

Map first, come it right and then I'll take it and then push, so it's going to create a 10 zero two

brand, you know, remote also.

So, Stuart, let me click on finish.

So it is pushing it.

Let it complete, Auchincloss, So now let me minimize this global perspective and then go to other

remote and then see that we have opened the door to the device, OK?

So now another thing is we have completer this data transformation section, which means we need to

push our quartermaster also.

So let me check out with Mark.

Let me start the day with him.

Close all these things, close tabs, close all tabs here.

OK, so check out as master, OK, and then let's.

Not to the master Blanchot, 10 zero to right, 10 zero two latest, OK?

It's probably just an abstract.

So I imagine limiting this to.

My master, so which means if I see a file, refresh Swayne, my master, it should be there.

So let's wait for a while.

File reflash.

So, you know, a local master plan to have the maps tracked first to gains.

That looks good.

So then we'll put this branch to our remote, right.

Nothing but a remote master also should be in sync.

Right.

So I'll push your OK.

So now let me push it.

So successful in the remote master, if you see Napster first, come it, so this completes our complete

data transformations section.

OK, so data transfer objects section.

OK, so in the next section we look on a different topic.



.

Thank you.

