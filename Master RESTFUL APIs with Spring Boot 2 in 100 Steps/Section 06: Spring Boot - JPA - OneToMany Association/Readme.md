### Step 49. Step-00: Need for JPA OneToMany for HATEOAS.md
Welcome back.

In this lecture, we're going to work on Springboard, Japie, one too many and many to one.

Mappings, heart associations, so the primary reason for implementing this whole section of one too

many are many to one in this building blocks schools use for implementing this concept of some hideous

concept.

We have something called safe linking in the relationship linking.

OK, so in the next section we're going to implement the concept.

So for herbals, you can implement the self-loading and also the relationship linking.

So a relationship thinking I can just take a simple example and mortarboard and then complete it.

But the idea here is if we do something, it should be like look like in real time.

Right.

So until and unless my perspective doesn't have the relationship, I can't implement that in the head

with Facebook it as a real time relationship.

Right.

So that's the reason I plan to implement Disrespectable section with Springbroot GPA.

So it's an additional cover for implementing these things and it's a good thing for all the men in the

building blocks course itself.

One of the major important mapping in which is one too many.

Even though these things will be covered in causing a battle here, we're going to try to explain it

and then implement it for two years.

So they use case is going to look like this.

OK, so we're going to build a simple Arbors controller and then Arbour's entity and then we're going

to say that for one user we can help many others write one too many.

So the same self-locking will implement both self-locking and build relationships linking in the base

and then get the complete clarity on the relationship linking to.



Bye bye.

Thank you.


### Step 50. Step-00: Introduction to JPA OneToMany Association.md
Welcome back.

In this lecture, we're going to understand and then implement SpongeBob G.P.A. one too many annotation

so I one too many association.

So if you see.

In one community by both, association can be represented by three to one or one community association

or even, but all depends on our requirement and then need so many different annotation allows to map

the fortnightly column in the chain identity mapping so that change has gone into the object reference

to the parent entity.

So this is the most efficient way of implementing the JPA one too many.

So in such a way that almost the minute one should act as a role model, the entire relationship and

Franchi of parent entity should be present in our child entity.

So in that case, it becomes the most efficient way so we can perform.

The associations in the member state was for this one too many.

So one is any directional association on a is bidirectional one association and interactional one with

difficulty.

Everyone knows that we can be better by XML in that manner storable.

But in addition to that, we have an option to do with the one with the query.

So like this, we can implement in three ways the rules by association in our implementation here.

OK, so if you see our use case introduction use first, we are going to implement that all orders of

user.

OK, so this doesn't.

The repository or anything, because we are going to fetch the others.

Well, that's OK because that uses the Specter entity.

We have the list of all this already mapped.

OK, with the implementation.

So we really need a new repository for this because we're going to fix these things from user so that

these get it out of our user and we're going to create an either for the user.

OK, here we started with the repository and used to pivot to that same method, see borders for that

particular user.

So we are going to.

OK, so we have a mistake here that should be corrected.

It's not getting it, so it should be posted.

So I'm corrected and the next is get all the details that I didn't use.

Right.

So if you want to get a specific order offered aspect of user, you can implement get all the details

using that user ready.

So be ready and then others are ready to get those details.

So on this level, the implementation steps looks this way.

OK.

These are very high level steps and every step in terms of steps need to be administered in a separate

of what's called file.

And then I'm going to show the implementation process.

Those things are key for every implementation.

We are going to have one separate branch, right, for convenience.

So we're going to create a any association brand.

And that's what we're going to do.

We're going to create another entity a minute to one association and like from other vendors related

association, we are going to implement in our other entity.

And then we're going to discuss more about it and we're going to discuss about fetching and all those

things.

And then we move on to updating the user entity with one too many association.

And once that one too many association implementation is completely user entity with the and so does

call it, we're going to implement the return of this method, the controller.

OK, so we'll implement this method and then move on to the implementation of the method that are supposed

to create the repository and then so that we can use the repository, that same methods and more and

better implement that all the operating method and that this one, you can take it as an assignment

for implementation.

And then we're going to get kind of code so that you can commit corpus to remote repositories in the

local market with the local master and then push that most around to do all these things will implement.

So this completes the relationship and implementation.

So introduction.

So I'll see you in the next lecture for me now with the implementation.

Tiki, bye.

Thank you.


### Step 51. Step-01: Create git branch for JPA OneToMany Association.md
Welcome back.

In this lecture, we're going to create a good branch for a deeper one community association.

So we are going to be the steps to get the same.

So let's go ahead and then explore these steps.

OK.

Going to copy this and I'll go to the command line if you see I am in my Springboro Building Works project.

So what else is Legget Branch hyphen maybe.

So what it does is get plantlife and it shows that my local and my remote branches come with questions.

OK, so if you see here my local.

Right.

So here it is.

OK, validations exception handling within one six six f the same remote also validation global exceptionality

nine one six six F so which confirms that our local and remote for previous branch is good.

But no, we need to ensure that we're taking it from our master.

Right.

So our master in 05 you'll see it is the same here and then in local.

In the same.

So it is a zero for validation if you see in here in master also if you see anything.

So all four are on the same commit conversions, which means we can check up from our existing master.

Right.

So and we need to ensure that we are in master are not.

So I said get status Anirban Masterbrand.

OK, so let me clear.

OK, so let me copy and paste this.

OK, get your code hyphen B which means new blood.

Draw six hyphens.

Playmobil Pyfrom GPA hyphen one too many.

OK, so let me clear.

So if I say get status now I'll be in my Spring boot GPA.

One too many branches.

OK, so no more created upstream.

OK, get push hyphen.

Hyphen set.

Upstream.

All digital and will copy the.

Brand name.

So we create the same brand with the upstream, OK?

So now we have created a virtual branch in our remote GitHub repo also, if you see here, it is created.

Now I say get a branch hyphen U, which lists the remote branches also.

So you can see here remotes are written six zero six one too many.

So we have completed our creation of the branch in step one will also go for I.T. and cross-check the

same.

OK, I see it is checked out with zero six.

OK, so now let me go back to what I do and we should be good now, OK?

So in the next step we move on with implementing the Springboard LaPier one to many implementation.

.


### Step 52. Step-02: Create Order Entity and @ManyToOne Association.md
Welcome back.

In this lecture, we're going to create another entity and to one association are that entity.

So let's see the series of steps involved in creating this other entity and translation from user.

So let's go back to the code.

So if you see here in steps, we're going to create the entity with many to one mapping.

So in the entity layer, we're going to create another entity and then annotated with able annotation

what the problems are this.

And then we're also going to add user found in addition to the other or the radio, the description

forms here.

And then we're also going to map annotate the user from the minute one association and then we're going

to add the first step as and also annotate the user feel with Gisenyi.

And we're going to generate Wooderson letters and not non-human constructor.

So these are the steps that we are going to perform on the intermediate for other entity.

So let's go ahead and then implement them.

So very much so in the NTD package and growing up in class named.

Order.

Right, and then I'll click on Finish, if you see this is in line to this package.

So this is a order.

So as this is the entity and being annotated with entity command, shift in product package, Jarra

X persistance entity.

So as we discussed in our introductory section, we're also going to say that people.

Right.

So people and it's me is going to be hard.

So come on, you've got important jokes, persistance people.

So now the next is the phone's in order.

And so one is private, long and I'll see you already.

Right.

And one more I'll.

Private string.

Audio description, so and if you see on radio, I'm going to annotate it with Heidi, which is nothing,

but I'm going to make it as primary key and I'm also saying that so let it happen.

It will keep generating the upper income for the ladies.

OK, so generating value and for both the things come and shift to important dynamics, persistence

idea and it's equal and generated value package is OK for persistence.

So now the next thing is finally the user.

So if you see here, so I say first let me write it down.

Private user.

User.

Right.

So we're going to create the association of the relational mapping between user and the order.

Right.

So there is no other entity now.

Right.

And we're going to create a relation to the user.

So let's consider like this so one user or multiple orders can associate with one user correctly.

So this is the other entity.

And we are saying that multiple orders can associate one respective user, which is nothing but many

to one relationship.

Right.

So multiple orders in the other entity are those can be associated to one user.

So let me add.

To annotation an additional government yiftah, so no unabating use.

Whenever we are fetching the data right.

So, as we are saying, this is going to be a by election mission, which we have discussed in our introductory

section of this JP one too many.

So what we said is it's a bidirectional relationship, which you are going to implement.

So when we're implementing bidirectional relationship, so when we are not careful about the types,

then it's going to end up in the recursive loops.

Right.

So we are going to say to want to listen in for this user object, we are going to see a fixed type

as lazy.

So what we are saying that, OK, so when you see a first step as lazy, which means until and unless

I say either BOBERT user, this user object is not going to be fetched in this other entity whenever

the request comes.

OK, so which is a good thing.

OK.

So.

Which type not lazy, so that's the reason we made it easy for Stip lazy.

So another thing is we are going to also add Jason Egnor.

So if we don't see this anymore for this, so what happens is whenever we are creating the order.

Right.

So it also expects user data to be sent and that's not right.

Right.

So like this, multiple things will occur here.

And the first thing here is we're trying to implement the first set of very high level of abstract layer

of annotations, OK, which is manyatta one one p.m. Napperby, these things.

OK, we're not going to the next level with your giant column, giant people.

OK, so JP has given annotations in multiple orders.

OK, so if you're dealing with a very high level, which means like the first level of first order of

annotations, like one too many, many to one and then Napperby and not using the second order, which

is nothing but than column design table, all these things, which means like we are writing a more

cleaner code.

But if the necessity and pressures are still going to join Kormann joint, we can definitely use them.

But first, we should try to implement our things with the primary level annotations.

And then if that is not possible, if the situation is too complex, then we need to try to jump into

adding the giant column.

So here you can even see gyne column and then say you already saw that.

It can be possible, but why you need to use the second order annotations, let's use the first order

annotations is the core logic here.

So that's the reason we're using Minetta when he said what we will try to use the Napperby so that the

association becomes TUTTO.

So we'll see that when we're discussing about any association that we have implemented a minute one

with typos.

So now the additional things, what we need to implement here is.

No argument constructed, and that hasn't set us suspended constructors from superpower's.

And the other is sports and Janet Bettison, Setas Selectable and generate.

So now if you see here, so we have completed creating the other entity.

No.

So let me see this.

And this completes the identity creation.

In the next step, we're going to work on creating the user entity, which is nothing but other side

of the equation.

So I'll see you in the next lecture then.

Bye bye.

Thank you.


### Step 53. Step-03: Update User entity with @OneToMany Association.md
Welcome back.

In this step, we're going to update our existing laws, that entertainment, 1:00 p.m. association

with that entity.

OK, so let's go ahead and then move the steps, what we are going to implement in this respect lecture.

OK, so if you see here, you're being provided with an entity with one to make an addition.

So, Bueso, to define how this will be from, you know, what was identity.

And then we're going to add one to many mapping.

I did this artist with the one many mapping.

And we're also going to add about Napperby, OK?

And.

My with.

Identity and we are going to get a sense of desperados and more about this killing, so many resources.

OK, so this is a very important thing.

So we are going to keep in such statements forever.

That's OK.

And we have two options to do that.

One is as soon as we complete these mappings, we can just start overSpringboot dletop and then go to console

and been ready for the column order.

Right.

It has created for all that stable and then good with the.

Certain borders in this manner.

OK, this is option one second best option to which is maybe ready for the baby before converting the

insert queries.

OK, so that is one more thing.

So that's more important.

So if you ever need to be a problem in waiting, that option to the order of these things doesn't matter

because we are going to.

Give the data by mapping these two things, but here the order in which it has created it has to be

and then in search terms accordingly.

OK, so now let's go back to.

I mean, then start implementing the step right now.

OK, so you go to Idee and we'll go to a user entity and then use that entity now.

So let's go ahead and on the orders here, OK?

So if you see it and then order harder.

So if you see where a user can have a list of orders.

Right.

So it is a list.

So let me see a list of part.

So let me find out from those orders and then command shift all to improve the utility list.

So now let's work on the mission.

So if you see what their mission is like, all this has like you want to manipulation, OK?

So for one user, we can have multiple orders, right?

So it's a one term installation, so I'll see one too many relation.

So, I mean, come on.

You've got the package.

OK, so now it is one too many.

So if you see here in these two in order order in the order of the interpolation.

So what we're going to say is like, I don't want to be.

Foreign key elements in both peoples, so what can you do?

It is like I can use it as a foreign key element in the other entity, right.

So which means so I can see Napperby.

And what is there to be present in order?

Right.

There's nothing but you said so when I say this, it is nothing.

But we are going to create.

You we call column in the other people, right?

So.

Let's say, like we're going to create a foreign key element here that are that stable, so that's the

Napperby importance.

We really don't want to Kahuta both terrible state relations.

So this side of that side of the equation is always referencing side and our side is always on our side.

So what is the objective?

I will not say what is developing the other side.

I didn't use that.

So I'm saying Napperby use it.

So, I mean, let me say it.

OK, so now if you go ahead and you need to do one more thing is we need to generate the watterson's

you set us for.

That's right.

So let's go ahead and do that now.

OK, so a source and then gendered getters and setters, fathers select get us select setters I can

select.

All right.

What happened?

OK, so.

So it's gendered getters and setters for other selectable gender.

OK, so now we have also generated the brothers and sisters.

So we have complete that entity in this world for one too many and many to one association so far this

and user and then all their bidirectional relationship.

So let's again reiterate what we have done for the user entity, OK?

So we have created it fully with a list of orders here.

And then we have created one permanent solution.

So others has one that many relationships here.

So we have the final one too many.

And then we have mastered this one with our user founded in our own identity, which is nothing but

order.

So that completes the.

So let's go back to the steps here and then let's also.

Better skin, better enforcement resources with these things.

OK.

So before going to do that, let's go ahead and start the spring up now.

OK, so let's say nice spring boot up and see if you're facing with any of these errors.

Right.

So it started successfully.

So let's go pro here to console now and see the order.

Right.

So I'll say localist has to console and then interconnect.

So if you see here, I got the orders to be created and with all that, I was the first thing and all

the description as the second one.

And I we saw that it has created OK, so that means buying certain products and values that are the

description and which you said we are associating.

So this better looks good for us.

OK.

So for user one, we have the models and we have two orders.

And the ones that are three, we have one order.

You can also create this way.

So this word means if you see here so repeatable orders and then.

I was at a field so we can also pretty dramatically use the radio also like this.

OK, so.

Because we have the use of Elderfield.

So in this way, also they can create the data, so I was this, which is small and then looks good

because we're in the order model, so we should be good.

OK, so I'll copy this and then go back to the.

DataDot Esquibel, OK.

And then I'll say open with.

Text editor and I will put these things and then I'll clear this and then I'll see.

So if there are any errors actually through here, OK, so no errors.

So let me go back to the head to cancel and then let me see connect.

And if I say so, let's start from Hoarder's.

So it should be split the data.

Good.

So you can see that on 123456.

And then audio description is one one 12 13.

OK, as I said to two one one one zero one one zero one zero to one zero two and one zero three.

So everything looks good now.

So this means like we have completed our user entity association with the one too many and also updated

a bit about the scale in the step in the next step will go ahead and then move on with that, testing

these things.

OK.

So before the next year, we can also be one thing, just like as we have implemented one to many relationship

from users and we have also.

Populated with some of the artists here, so they can even fetch the details from either side.

OK, so which means like we can do better and then our artists need to bolster their because we have

one too many.

Right.

And then we have created a list of everything within the idea.

You have also said that for the.

Users, you said that stuff like this and then you have also created a data center that's for the same

thing, so which means we'll never be safe with all that snow, ideally in that the other subject with

the list of all that's associated with that user should be listed.

So let's go back to our postman here and then see the suspect.

So let me send C4 one zero one.

We have 2000 to 2003 to protest for one zero two.

We can see it for two quarters and then for one zero three, it featured more orders.

So that's about all you users saying if you want, we can even do that.

Did you celebrate your Saturday night so I can see one zero one so we can see our Scott Fetcher, which

means the donation from one to many, which is from you to others.

We have started now using get all users in that user base Heidi.

Right.

So in next lecture, we are going to create a method which only store orders for their respective idee.

OK, so we will see how we are going to implement that.



.

Thank you.


### Step 54. Step-04: Implement getAllOrders RESTful Service.md
Welcome back.

In this lecture, we're going to implement that dollar, get all this matter in our arms control.

OK, so let's go ahead and see the series of steps we are going to perform further.

OK, so if you see here, we are going to implement the telemedicine.

That's the other controller.

So before going to other controller, we're going to make slight changes in our control and therefore

user controller.

So the controller currently for each of the methods, we can see that we have the.

Youssef says a permit for every method at the third level, so we are going to move this user said the

class level using annotation, request mapping and then other things inside.

OK, insert method level.

So when we are doing this, this will help us in creating self things in our section, which we are

going to implement in our next section.

OK, so that helps the hapless implementation.

OK, so that's the reason we never use this context to the request mapping at class level.

And the remaining things will be that the method level.

Let's first implement this and then move on to the next section.

OK, so let's go back to that idea.

You know, and if you see here.

So let me open the country, let's package and I have that user control over here.

So if I say here, what I'm going to say here is a direct request for mapping and then zip code slash

use.

OK, so it's amount got to import request mapping a package and then say, OK, so now I remove a bitmap

and get all user interfaces.

The data should be displayed here at method level.

I don't need anything.

OK, so I'll receive it.

OK, so in the same way for post mapping also I don't need anything near the method level and certainly

most large users here.

OK, in the same way that users by Iot.

So we have a very different user context at the mass level.

I just remotes, not users for a bit.

We were sort of saying we have defined it.

Nice living here.

OK, and we'll have an idea here.

OK, the same for delete users.

So I'll do the same and for getting user by user name.

Also, I must ask users, OK, so this completes our first step of updating our user controller with

the user's context at the last level, which is going to help in our hater's implementations.

OK, so now let's go back to the steps here and discuss these steps and go ahead and then implement

it.

OK, so in the control, we're going to with the controller and then annotated with rest controller

and also annotated with request mapping with slash users.

And then we're going to define this method so that this method is nothing.

But we get all those for a particular user so I can see slash users and then send the user ID and then

best context.

And what happens is all the orders associated with this respect user should be displayed so that the

users method and then we're going to use this method directly with users and then one zero one slash

orders.

And also we're going to test what we tested in our previous step.

But all users can get used by it and then verify the Arbour's presented those things one more time.

OK, so that's all.

So let's go ahead and then implement it.

One more important thing here is we are not going to define a service layer and then add service layer

methods and all those things from here on.

OK, so as a standalone, we are going to have shown those things in Nevada G.P.S. We're deeply into

the position where we have created the user service and then user controller and all those things.

OK, but if you start with every in every one of these steps, OK, so I'll leave you with a standard

that we need to define a service and then those methods need to be user in the controller.

And any business logic is that we need to define in the service layer.

So we've already discussed those things earlier.

So not just to ensure better for the.

Timesaving purpose and also for implementing little.

For the easiest manner, which means like if you define multiple methods in service layer and then again

call them in control and there it is, going to take more time and been more or less akin to duplication

of methods.

Let me bring in a standard mode that is good, the way to do that.

But no, we're going to just add the controller.

We're going to create the methods directly under other control using the user depositary.

OK, so let's go ahead and do that now.

So it isn't I mean, the controllers package, I'm going to create a class named.

Other controller.

So I'll make this bigger and then I'll say I'll take this with the controller and then come on shift.

Oh, OK.

And I'll also say one more thing here, that they did request mapping.

And then I will say slash

value is a call to slash users.

OK, come on.

Oh, OK, good.

So now I'm going to of two things here.

One is primarily I need to use a repository.

OK, so I'll see a private user.

Repository user.

Repository Glenmorangie of total import, and then I'll see the word.

Or to word.

OK, so we got the operate annotation imported, so it took a little bit of time to resolve.

So now we are going to create a method named

get all orders for the user.

Right.

So I'll say.

Public, it's a list of orders we are going to read and write, so I say get all orders.

And what I'm going to take as the input is long and then use already, right?

And Chief, go to the harder.

List and also as a battery, but also important, good.

So first thing is do whatever the past you need to check if it exists or not.

Right.

So I'll see you.

User user is call to user repository not find by.

Heidi.

And then I'll see you Saturday, right, and.

It will put you, sir, right now, in addition to that, it also just 30 changed type of user to optional,

right?

So I'll say this as user optional.

Right.

So now one important thing here is.

So if you sat optional, that is present, right?

So if you use that option, a lot is present, not off, which means if you use that option, a lot

is presentments.

If you.

That is not present.

OK, then I am going to turn you OK.

I can see your response to it as exceptional through user, not from exception with some string here.

OK, so I can say user not fun.

Right.

And it also says that OK, protocols are not for an exception and also Atrous declaration.

OK, so that's good.

So if a user is not present then you user not from the corruption.

OK, but if a user is present, what we need to do is we need to.

Written.

He was an optional.

That.

What's happening?

So we are.

Here, right here.

I've done a small mistake.

OK, so little use of small dots get off, I get hardass.

OK, so this completes I get all orders for you said method creation.

OK, so now what we are going to do is we need to add we could get mapping seeing so we need to send

after users slash.

You said Heidi has the best variable rate and Pardus.

And I'm on shift to.

For kidnapping and kidnapping.

See, so this completes the battle that's very user savvy, so let's go ahead and test it.

So just to reiterate what we have done.

We have important values that we are the controller and then are provided and we have created a better

on this matter.

And we are taking the input, as you said, 80.

It is nothing but from the part variable, we are taking that use a ready and then we are going to find

that user, whether it exists or not was a the repository, not fine by it.

And we are saying that if the user is present, OK, then go ahead and then return to the hospital users

orders.

But if that user is not there, not have that, then through the user, not one exception saying user,

not phone.

That's all.

OK, that's all we are going to do.

So let's go back to our postman and then.

Yeah, let's go ahead and then create a request.

OK, so I get all of this for a particular user, right.

So that all of this OK, and then I'll say it is a tall order.

OK, so I'll say localhost and for you that's one zero one.

I need to get the orders, whatever is present.

OK, so I'll see you then.

Send.

So if you see it for use ups one zero one we got the order says 2001, 2002, 2003 in the same way for

one zero two we might get broader circle four and then five and four one zero three.

We will get only one order, whatever is present.

OK, so let's go back to what has to console.

You can see the output associated with one zero one one zero zero one.

So we've got the same here, OK.

So if you see here for one zero one, you said we got three orders.

So this is a above that on this.

Service.

OK, so in the same way, will implement, create order and then get all orders by all the radio also

in upcoming lectures.

.

Thank you.


### Step 55. Step-05: Implement createOrder RESTful Service.md
Welcome back.

In this lecture, we're going to create create all that maternal, so let's see the steps involved in

working order method, OK?

So we'll go to the school.

So if you see here in the repository there, the first thing we need to create the repository.

Right, because we're going to create order.

It needs a repository, the same method.

Right.

So for the purpose, for now, we really don't get a chance to have any specific method related to others.

OK, so now we need it because we need to see that all the data, whatever we are sending to the other

table.

So to do so, we need to find out the repository.

Right.

So next is the control we're to do with the controller and then the third we're to this post.

So for the user's context, we're going to send the particular user and for that particular user, we're

going to post the other data to create that for that user.

So that's about the controller that we're going to do and then the person we're going to test the creator

for the user.

OK, whatever we created, we're going to retrieve those items using that allowed us, which we implemented

in our previous lecture.

In addition, you said the best way to get all users and videos are by idea.

So we are going to fight and then test whether the whatever we have created has been displaying better

not.

So let's go ahead and implement the same create order in our idea.

So let's go back to our idea.

And in our first step is to find a repository.

Right.

So let me go to the repository here to presbyteries, package and interface.

All these repositories are interfaces.

Right.

So I'll see how the.

Repository, right, repository and finish, I'll make it bigger and then what say is are the repository

extends the deepest repository, right.

And what is the entity behind it is order.

Right.

And what is the primary care of this or that is long buried above.

Right.

It is long.

So long years the right.

So that's the thing.

And let me put those things into this or that is imported repositories and put it one final.

We are going to tell Stream that this is the repository site.

Come on.

You've got to look important.

So and then see the other repository.

So now let's come back over other controller first and then let's make it bigger and then lose.

I will dig here.

And what I'm going to do is I'm going to take whatever method so I'll see the public.

I'm not going to return anything initially.

So it's a public wide and I'll say create order and that's all OK.

So for creator, what are the inputs?

So if you see our inputs are going to be two things.

One is so user for which we need to create the order.

And the second is.

He crossed the border.

So let's go ahead and then for you, sadly, we are going to get that from Pat Variable-rate.

So and then I'll support variable law and then use O'Reilley.

So first in the cleared command shift to input pattern.

So next is the.

So I see.

Request body, and then I'd say order harder, come on.

Oh, right.

So now we have Wopat variable and then request bodyboard as inputs.

First thing is to verify whether that user exists or not.

Right.

So for that purpose, we will add this step as these OK.

So in this step, what we're doing is we're going to get the user ready and then whether the user is

present or not, we are going to check.

So the user is present when we want the next steps.

If you are not present, then are going to throw the user not for an exception.

So electron's declaration.

OK, so.

Know what I'll do here is I'll start working on getting the user.

OK, so user helps a lot.

Get so I got the user.

So what I'll do is order dot said user.

So which means I'm going to set that user in a persistent context.

So far, this spectrum user, I'm going to say order dot order depositary.

So we are told that oppositely, all right, so let's go ahead and operate that now, not so private

order repository.

Of.

Repository and I will say, come on, you've got to import and then I'll also see the white.

So now they are the repository, not safe and empty entity use nothing, but.

All right, so whatever we have sent here after.

And this company, it's not clear if you want, we can even return whatever the order created, the

same thing we can return.

OK, so I can see a return order and then change the metal return type to order.

So at this point, no, this method will return the order.

I need to get my pulse mapping work so we'll see a pulse mapping and then first thing is, after slashing

users from the request mapping, we are going to have the user ready.

But he was ready.

And after you said you are going to have the hardest flight.

So that's all.

So this is a border post map and command.

Got to input the post mapping that.

Shouldn't expect it would happen, so we need to also say that what's missing here.

OK, come on.

Yeah.

So this completes the creator of a method creation and then service creation.

OK, so let's go back.

We're going to test create order that allowed us users and then these things.

OK, so let me go back to the postman and then I'll create a new request named.

I request and then also commit murder.

OK, so now in this great order, what we need to do here, we have got the right in this thing.

I can copy here from the previous things and I can say, look, I lost.

You were one zero Roman slash.

Hardass right inside that and the Methodist method and then save your now and go to the body and then

I'll see.

You're right.

So let me make it a little bigger for convenience, OK, this should look good.

OK, so now I might also Sextus Jason applications that Jason and then I'll copy these things.

No, so.

So.

Kopi.

And then.

--, I don't know, it's not getting copied.

OK.

Write it, OK?

It's not a big deal.

So what we need to do is we need to see.

Order.

Description.

Right, and and set the values are there one, one, two, two, OK.

So we have only one friend here because the other one is going to drop it.

And if you see the other entity, you're right.

So we have three films here that identities are generated are the description and the user, which is

obviously commercial.

We are not going to consider that.

So for creator anything, OK.

So now if you see I don't want to see and then I'll say clear.

OK, so if you see the description of an alternative or another that create a little bit more than nothing.

So Second-order that created support after that.

So now let's go.

OK, all this method and for one zero one orders.

OK, we'll see.

OK, we have one, two, three and double one's OK.

So that's a lot of smattered testing.

Same for that user base already.

So I'm going to bed.

The user decided they can see that Mr. here saying they can also e-mail us so we can see all the.

Oh, that's for all those present, OK, so that's about it so far, I mean, we can see already one,

two, three, whatever, we annually in the US, which are represented in the database, does the same

thing for other things, too.

So this completes the create order method, creation method of service creation.

So if you see a high level, what we have done is we have created all the repository and we want to

add a controller and created order method there.

And then we have an integrated with post mapping and then we have written the logic required for that.

And then after that we went on and then.

Pasteurizing Posman, all these requests and then ensure that that method is working as expected.

OK, so in the next lecture we're going to work on that audit because using all that idea and then notoriety.

.


### Step 56. Step-06: Implement getOrderByOrderId RESTful Service.md
Welcome back.

In this lecture, we're going to discuss about it all that way are the lady method.

OK, so this one, you can take it as an assignment for implementation and if you see the steps involved

in making the other controller.

Plus, you need to just create the method, get order by order, ready, OK, and the get mapping is

going to be this way.

But the that idea in the notoriety and insert the logic is like this to verify whether the user really

exists, whatever is sent, and then also verify that the authorities it exists or not.

And if both exists, then are the lady using the repository.

Right.

So you can implement this or you can take this as an assignment and then implement this to have a hands

on on the sections, what we're discussing in this course.

.

Thank you.


### Step 57. Step-07: GIT Commit, Push, Merge to Master and Push.md

Welcome back.

In this section, we are going to understand and implementSpringboot nable Patreus, so let us transfer hypermedia

as the engine of application state.

So if you see here,Springboot dletop is an extra level upon the rest.

So it is easy to present information about this, to apply to a client totally to bring the repair documentation.

It speaks in a written response and claim can still further communicate with the server.

You have to simplify the claim by making it discoverable.

So if you see here, this is what we're going to implement as part of our entire implementation for

Hippias.

So this is on this request.

OK, so if you see in the service we get the user and then it's incumbent on us and.

After this comment, we have another user indexical orders, so after implementing Historias so we can

find these links, whatever we are seeing here can be seen.

So if you see here under the links, you can see two things.

One is self and then another is on orders.

You can see that says it's a link.

Right.

So let's discuss about the self and.

All right, so now we know about products that creates the links like this.

OK.

And then attach a separate upload, which we want to attach it.

So now what is this self link?

Self link is nothing, but we create a link for that object, which means like you're displaying the

user details of a particular user.

So this is the self that user you can create user slash one zero one in the same way that another all

of us link.

OK, so this is nothing but the relationship link.

So which means if you see one, too many of you have already discussed it.

That right.

So user Arbour's is nothing but one too many and one user can have multiple orders.

Right.

So no, we went to the user flow and we want to move on to the others.

We need to get for this user.

We got the user details now.

We need to get for this list to use it while others are present.

Right.

So we're going to go there and then click on all orgasming from our list, from our client, right.

From our client, whatever we are using, like maybe ADHD or whatever.

Right.

So whenever you click, we really don't need to get the details and we don't need to hardcourt our data

API information related to others.

But I think that this framework or anywhere on the end like this framework.

OK, so using this link which has been propagated using to get user variety, you also have the links

so we can click on this to get for this list better user wartell the surplus.

And basically.

So that's the importance of is what it does for us.

So provides links for the flow which we want to define our access after this particular step, what

we want to do.

So this reduces the likelihood of a plane breaking due to changes to the service.

So this is another important thing.

So it's this a claim of the making changes to the service?

Usually in the apps that are like, you know, the version in concept, like we can do the questioning

using partner headers are even there are multiple options available there, but it's a tough implementation

from implementation side to have it implemented both from a client perspective and on the server side

perspective.

But it also solves multiple problems here.

When we're using data.

This is like a.

If we are going to change something relative to others, you are so we say that others.

We want our RSV to something here, OK, but our.

Iran claimed whatever the US or whatever we are using about this primary itself.

OK, so and then he will go and then catch that respect to all others back here and then the speckling

here and then go, which means any changes to the CPA doesn't impact us from the U.S. perspective.

And we are using headways.

So this is one more important thing which we can see about the heteros implementation.

So from Spader's perspective, we can see it.

One visual example here.

OK, so from Ippei Discovery perspective, let's see that here.

So we have a baseline here and it compares with the EPA and then EPA has links to it, B, C and so

it has the relationship plinks B, C, and then you consider this as one has all lot of one as some

of us by specific product or something, something like that.

OK, so now your pay claim was this information while using your per year, it will be able to communicate

with the ABC and then automatically so now the client will be communicating would be considered like

it must be, and then it or there will be.

So now it will be has links to the industry.

So we will go ahead and then the client will be able to access it.

And then even better features are functionalities from the B itself.

So from C also we can see Efendi.

So this is the way, which means like EPA information is discoverable using the EPA, which client is

accessing.

So this simplifies the overall communication.

OK, so this is about the discovery concept.

If you take in example here, like you can see on Amazon, you search for some bowcock and then you

click on and then open that book page.

Right.

And then we're ready to buy that book.

So consider that as EPA.

Right.

So my C and then we are related APIs, which means books by that author is B and then.

Books by that similar name, which means like you are trying to search some book named ABC and then.

Books by the prospect of the president, ABC, EPB and then ABC has some context.

So using that ABC context, similar type of books with the different tortoise's APAC, so those will

be displayed on video screen and click on it is of books by this author or those books by this will

be displayed and again, additional information about that based on those author's multiple books.

Then again, based on those contacts, again, other things will be discovered and then displayed here

so that all these things are like interrelated.

So this is a the spring, but it was a child's diaper discovery problem.

So to speak up.

Its internal data is internal.

OK, so Springhill Prospero's abstractions for Convertino.

You are right.

So one is resource support.

OK, so and the other is link and there is Controller Lochbihler so we'll see each of them in detail.

OK, so we can use these three to build what you mean associated to the resource.

So let's start with the research support.

OK, so support is nothing, but it's to extend our entities like we have user and other entities in

our current example.

So we are going to extend that resource support plus inherit the ATM.

So what is this ATM?

Right, so ATM is nothing.

But so using resource support, we have extended other entities and using the money and control of linkable

that are using these two things we have created.

The link that you have created the link to said that our current PayPal, which for which you want to

display the links.

Right.

So in general we are going to do that.

So we are going to do that in the process means we need to write a lot of manual boilerplate, implement

that and add new forms in your existing entities to do that.

So like this multiple stuff will be better implement if you want to add attributes to our API.

Right.

But with headers it becomes absolutely simple.

OK, and it removes one thing here.

You said that had been the information he broke out of that ad and pulled the information here so far,

admittedly provide link, whatever they have constructed to this admitted, and that will be set on

the research context and then displayed to the user the links in that respect resource.

That's all so bad.

But that's what Haber's simplifies right now.

So we have seen what is happening to our problems.

It's also been a lot of things embroiled in this so far.

So no mixed in from implementation steps perspective.

We're going to do the following things as well.

Firstly, we are going to create and get branch federal springboard, hapless OK section, and then

we're going to add dependency, another bomb that SML and then if required, we need to restart the

Spindletop whatever the can get to ensure that the literature got picked up if it was already running

elsewhere and planning issues.

And then we're going to extend both entities use that and then other entities which we have the sort

support.

So for us, this is the primary step which we need to do so that we get the option of adding the links

directly to the user or that I use about the ATM and then other that ATM.

So we will do that and then we'll be able to use it in other companies for implementation.

So this is the critical step for us because so as we are growing the code heavily with the single worst

case for different sections, we are implementing different things here, OK?

So instead of creating little more steps and more coding the existing user and then other controllers,

if you separate out papers related things separately and user controllers and then all the data is controllers.

So from our perspective, it is going to be a clear and clean code, OK?

So for that purpose and implementing it, using that heteros controller and it was controller, but

in these two controllers, for whatever methods we are applying to implement self-locking in the relationship,

linking only those methods will be available for our implementation and then will go to step forward.

We will implement self link in our get usability method.

So once we implement this Elfrink, we are going to test it and then we'll move on to step five, which

is implement self and then relationship work better use this method.

So the relationship which we are going to implement is we get all this matter in either haber's controller.

So next is going to this.

We have divided into three parts here.

One is self link for each user.

So whenever we have for the user surveys write it, it provides the list of users.

So for each year that we will have a self link for that user so that we are going to implement, then

we are going to implement the relationship link with the others.

So for each use, it will have a relationship link with get all other users to order one to many relationship.

So for each user wartell either side person, that link will be there.

And if you click on that for that, all this will be displayed.

So that is a very important step for us.

And when it's a good step for learning and the next is self link, forget all users.

So note this clip of users embed.

This method also makes us Healthlink.

We can also implement that.

How we will going to implement it will do it.

So as part of this we will also learn resources also like what is the resources section in our papers?

We are going to change our Mostafaei methods to types resources.

So as part of that, we know how we are going to use the resources and finally will commit the code

in the GitHub people in the remote Reppas remote branches and then will close the section.

So I'll see you in the next lecture, starting with our step zero zero.

.

Thank you.

