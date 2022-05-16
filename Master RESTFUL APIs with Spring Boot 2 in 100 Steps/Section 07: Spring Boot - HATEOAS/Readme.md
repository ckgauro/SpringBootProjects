### Step 58. Step-00: Introduction to Spring Boot - HATEOAS.md
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

Until then, bye bye.

Thank you.


### Step 59. Step-00: Create git branch for HATEOAS.md
Welcome back.

Later, we're going to add, you know, but I'm not exempt, so, I mean, if we already have absolute

and started state, OK, it might not be sufficient there.

We just need to start our the new dependency.

This because as a springboard starter happiness.

So new jobs will be added.

So let's go over Bombeck someone and then.

Oh I better spring bookstaber hater's dependancy.

So we are in the eye you know.

So let's open Bombeck Semmel.

Let me make it bigger.

So Independence's.

So if you see here we will copy other existing dependancy for Springboards Totowa.

And you're going to see spring up started here.

Yes, right here, too, yes.

And then going to save it.

OK, so that looks good.

So let me start my app also one spring app.

So it will start now.

So there should not be any issues.

Yes, OK.

So it started successfully, we should be good now in the next lecture will go on for the implementation.

No, we have added the dependency.



Bye bye.

Thank you.


### Step 60. Step-01: Add HATEOAS Dependency in pom.xml.md
Welcome back in step, we're going to extend both identities to resource support, which means we have

both been identities.

So we're going to extend both you and other entities with the research support so that we get the option

of that ad and then all that add to add links.

OK, so let's go back to what I know and let me tell this pandemic symbol and we'll go to the Entities

section.

Let me.

You said that it was that entity.

And if you see here, public class user.

Extends.

We source support, right?

And then come on shift.

All right, so it should impose the necessary package required for us so we can see here it has imported

papers and resource support package.

Right.

So let me save this, OK?

And I'll also go through a lot harder and also do the same.

So I see.

Extends resource support, command shift and then save it.

OK.

So we have completed watching this, but if you see that user entity, we are seeing error, so let's

go down and see where it is either.

So it's doing better for the Tidey.

So because the results also we have the similar thing here, OK, similar implementation, same that

look of battery.

So that's the reason it is strong there.

So what we do is for our current, Heidi, I'm going to change it radio so that we should be good.

So this is going to be use radio and generate the data centers accordingly.

Right.

And then construct it also in the same manner.

And it will generate a need string here.

OK, so if so, very remote.

So we will generate all these three things accordingly.

So first things I need to compute source and then generate getters and setters.

So select for use that I generate.

Right.

So they generate headquarters in that area.

So now I also generate field constructors.

OK then generated.

And I.

Kopit had this place right, finally for troubleshooting, use this to string, so I really not needed,

but I don't know when we need it, so I'll see gendered to string, right.

I have selected a first name, last letters and orders, and then I cut this and then post it here.

Right.

So now we have.

Control your control.

Shift F to farmer the court and then save it.

So now if you're seeing that you said that job of achieving the user entity better got resolved.

So across the users are telling you that?

I do.

Yeah.

There might be some issue that will see that.

No.

OK, so let's go down slowly.

See here.

OK.

So user that set idea.

Right.

So we need to change this.

So I will say that as user that said you said Heidi, then I can say you idea.

Right.

Anything is fine here.

OK, so that's it.

OK.

So.

This after saying this service should be good.

Yes, good.

So this completes our resource support extension for both our user and then other entities.

OK, so in the next lecture, we'll focus on the other steps of haters.



Until then, bye bye.

Thank you.


### Step 61. Step-02: Extend User and Order Entities with ResourceSupport.md
Welcome back.

In this lecture, we're going to create that and order controls for its implementation.

So instead of using the existing user controller and then our controller, we're going to create a user

interface controller and then all that matters controller and then add necessarily that that's the code

for the implementation.

So this is to ensure that our existing user controller and other controller related functionalities

were not disturbed as part of heteros implementation and also completely isolated people's implementation

for better understanding, instead of the number of lines of code during the learning process is very

high per controller, then it becomes a little difficult to understand what we have done over a period.

Right, because there are other multiple sections planned as part of this code.

And then if you only use a controller and then order controller, then it will be like a huge amount

of code with different different options available right away because future will be implementing filtering

with the static filtering dynamic, filtering all these things.

So that's the reason we try to isolate the user base implementation of the two different controllers

so that it will be easy to understand and easy to implement.

And then when you are replicating or following the codes and then implementing it, it will be very

easy to implement.

Only thing is, we just need to ensure that we are implementing this step three extra before doing the.

Implementation of the controls for this method.

So let me go back to the school and if you see here, this is the step three, we're going to create

new user random order controllers.

So that user interface controller, we are going to create a controller annotated with rest controller

and request mapping.

We're going to give us a little slash users.

The existing user and then other controller has direct only users.

So now we are doing it with Hater's users.

OK, and annotated with a direct validator.

And after the president receives a repository and copy networks, we're going to copy two methods here,

which we are going to use for our hater's implementation.

So we are going to copy that user by word.

We are going to implement them self linking of heteros and we are also going to copy that.

They can use this method in this.

We are going to implement board self link and then relationship linkable that are larders.

So that's the reason we are copying these two things.

OK, and from ordinator controller perspective, we are going to create that and then out of it with

the controller annotated with request, mapping out of both repositories and then copy methods that

all us from rather controller to controller.

OK, so this one is a method which will be used are called and we are implementing that all users relationship

linking.

OK, so that's the reason we have this here.

OK.

And then once these are done, this implementation, we need to ensure that both our alternators controller

and the controller are retaining proper results for the three methods which we are going to use for

headways implementation.

So having them in the Posman by creating a request for Hater's, you are right.

And then we'll move on to the next step for Hater's implementation.

That is nothing but that user by itself linking.

OK, so now we'll move on to a better idea and then start implementing this, OK?

So if you see where we are and the controller section, so first thing is you need to create a new class

and then say user interface controller what?

And then finish.

So we are going to annotated with the controller and request mapping with.

Why is it called to smash hapless slash users, right?

And one more we are going to do is validated because we are doing your part, the variable party, the

validation rates of others.

So come on, shift over to import and then you are going to auto where the user.

Repository user.

Repository, right, come on, Shifta, and then.

Out of white, right, one more lottery's private user service, user service, road alerts are the

words that also right.

Got MindShift.

All right.

So we have completed this.

No, let's go back to our user controller and then copy the method.

But I'll use this method.

Right.

So that is first method, which we need to copy.

OK.

And the other method, which we need to copy is that the user by idea, right?

So this is the one gate user by idea.

So let's copy this and go to user hitless controller and then copy these two things.

OK, let's modify one more time.

So we have created a heteros controller added rest controller request mapping, validated and operate

both the user repository and then user service.

And we have copied the data user by the method.

And also we also copied look at all users methods.

OK, so now let me see this.

Right.

Good.

So now let's also do the same for our notorious controller, so.

Plus, and then I'll say, oh, there he is, comptroller.

Right.

So now let's add the.

Wrest control and did it because mapping and value is a call to slash, it is useless, right?

And then government, you've got to import those two things and then you need to alter both the user

and then the.

Of the repository.

Repositories.

OK, so we need to order both user and then order repositories here, so I'll see

private user repository.

Use a repository in the same private order depositary.

The repository and even Ottoway them, right?

OK, that's good.

So now let's go to the artist controller, which is nothing but order controller and then copy the get

all orders for the user.

We are not going to use any create order here.

So I didn't even order repository is not needed when we are using get all orders, but just a map.

OK.

So you see here, it's not your stock so that's the thing.

So now we have completed the.

Other people's control also.

So we'll go to Alberto.

First man and then implement the methods.

So when the postprandial so let's increase the fun a little bit.

Yeah.

So now if you see here, we are going to create.

Request and request, and I'm going to say that all users.

He is right so that all users hate us and say, here's to DP localhost and then context is Atrius slash

users, right?

So save it and then test it.

Right.

So now we have got all the details required for the headways.

Right.

So which means like a.

That all users in the haters, but I hate this controllers working as expected, so next year get user

by 80 so we can duplicate this, OK, that was a priority and then say that it was a way for her to.

Yes, right.

So I'll see.

Hitless, OK, and then I'll add the headless part here is Slash uses one zero one and let me send the

request.

I got the request.

OK, so let me save it.

So we're seeing some reference here, which is related to links.

You can see it here, right.

So this is because we have extended other entities with the resource support.

After that, we started getting these links.

Currently, we didn't set any links.

So that's the reason those are empty.

So I will go back to Alberta, get all us and then duplicate that.

OK, and then this is also forget on orders to slide.

Hato is OK and you need to add up here to spottier here to your slash user, slash one zero one orders.

Save it, send it.

So now this looks good.

So this completes our up.

Yeah.

Step three, which is nothing but a creation of a user heteros controller and copying these videos are

about and get all users method order heteros controller and get all of the SM.

Copy that.

OK, and the best of all the three requests, get usability, get all users and then get all orders

in the next lecture will go ahead and then implement the self linking.

Forget user by using headways.

.

Thank you.


### Step 62. Step-03: Create new User and Order Controllers for HATEOAS Implementation.md
Welcome back.

In this lecture, we're going to create that and order controls for its implementation.

So instead of using the existing user controller and then our controller, we're going to create a user

interface controller and then all that matters controller and then add necessarily that that's the code

for the implementation.

So this is to ensure that our existing user controller and other controller related functionalities

were not disturbed as part of heteros implementation and also completely isolated people's implementation

for better understanding, instead of the number of lines of code during the learning process is very

high per controller, then it becomes a little difficult to understand what we have done over a period.

Right, because there are other multiple sections planned as part of this code.

And then if you only use a controller and then order controller, then it will be like a huge amount

of code with different different options available right away because future will be implementing filtering

with the static filtering dynamic, filtering all these things.

So that's the reason we try to isolate the user base implementation of the two different controllers

so that it will be easy to understand and easy to implement.

And then when you are replicating or following the codes and then implementing it, it will be very

easy to implement.

Only thing is, we just need to ensure that we are implementing this step three extra before doing the.

Implementation of the controls for this method.

So let me go back to the school and if you see here, this is the step three, we're going to create

new user random order controllers.

So that user interface controller, we are going to create a controller annotated with rest controller

and request mapping.

We're going to give us a little slash users.

The existing user and then other controller has direct only users.

So now we are doing it with Hater's users.

OK, and annotated with a direct validator.

And after the president receives a repository and copy networks, we're going to copy two methods here,

which we are going to use for our hater's implementation.

So we are going to copy that user by word.

We are going to implement them self linking of heteros and we are also going to copy that.

They can use this method in this.

We are going to implement board self link and then relationship linkable that are larders.

So that's the reason we are copying these two things.

OK, and from ordinator controller perspective, we are going to create that and then out of it with

the controller annotated with request, mapping out of both repositories and then copy methods that

all us from rather controller to controller.

OK, so this one is a method which will be used are called and we are implementing that all users relationship

linking.

OK, so that's the reason we have this here.

OK.

And then once these are done, this implementation, we need to ensure that both our alternators controller

and the controller are retaining proper results for the three methods which we are going to use for

headways implementation.

So having them in the Posman by creating a request for Hater's, you are right.

And then we'll move on to the next step for Hater's implementation.

That is nothing but that user by itself linking.

OK, so now we'll move on to a better idea and then start implementing this, OK?

So if you see where we are and the controller section, so first thing is you need to create a new class

and then say user interface controller what?

And then finish.

So we are going to annotated with the controller and request mapping with.

Why is it called to smash hapless slash users, right?

And one more we are going to do is validated because we are doing your part, the variable party, the

validation rates of others.

So come on, shift over to import and then you are going to auto where the user.

Repository user.

Repository, right, come on, Shifta, and then.

Out of white, right, one more lottery's private user service, user service, road alerts are the

words that also right.

Got MindShift.

All right.

So we have completed this.

No, let's go back to our user controller and then copy the method.

But I'll use this method.

Right.

So that is first method, which we need to copy.

OK.

And the other method, which we need to copy is that the user by idea, right?

So this is the one gate user by idea.

So let's copy this and go to user hitless controller and then copy these two things.

OK, let's modify one more time.

So we have created a heteros controller added rest controller request mapping, validated and operate

both the user repository and then user service.

And we have copied the data user by the method.

And also we also copied look at all users methods.

OK, so now let me see this.

Right.

Good.

So now let's also do the same for our notorious controller, so.

Plus, and then I'll say, oh, there he is, comptroller.

Right.

So now let's add the.

Wrest control and did it because mapping and value is a call to slash, it is useless, right?

And then government, you've got to import those two things and then you need to alter both the user

and then the.

Of the repository.

Repositories.

OK, so we need to order both user and then order repositories here, so I'll see

private user repository.

Use a repository in the same private order depositary.

The repository and even Ottoway them, right?

OK, that's good.

So now let's go to the artist controller, which is nothing but order controller and then copy the get

all orders for the user.

We are not going to use any create order here.

So I didn't even order repository is not needed when we are using get all orders, but just a map.

OK.

So you see here, it's not your stock so that's the thing.

So now we have completed the.

Other people's control also.

So we'll go to Alberto.

First man and then implement the methods.

So when the postprandial so let's increase the fun a little bit.

Yeah.

So now if you see here, we are going to create.

Request and request, and I'm going to say that all users.

He is right so that all users hate us and say, here's to DP localhost and then context is Atrius slash

users, right?

So save it and then test it.

Right.

So now we have got all the details required for the headways.

Right.

So which means like a.

That all users in the haters, but I hate this controllers working as expected, so next year get user

by 80 so we can duplicate this, OK, that was a priority and then say that it was a way for her to.

Yes, right.

So I'll see.

Hitless, OK, and then I'll add the headless part here is Slash uses one zero one and let me send the

request.

I got the request.

OK, so let me save it.

So we're seeing some reference here, which is related to links.

You can see it here, right.

So this is because we have extended other entities with the resource support.

After that, we started getting these links.

Currently, we didn't set any links.

So that's the reason those are empty.

So I will go back to Alberta, get all us and then duplicate that.

OK, and then this is also forget on orders to slide.

Hato is OK and you need to add up here to spottier here to your slash user, slash one zero one orders.

Save it, send it.

So now this looks good.

So this completes our up.

Yeah.

Step three, which is nothing but a creation of a user heteros controller and copying these videos are

about and get all users method order heteros controller and get all of the SM.

Copy that.

OK, and the best of all the three requests, get usability, get all users and then get all orders

in the next lecture will go ahead and then implement the self linking.

Forget user by using headways.

.

Thank you.


### Step 63. Step-04: Implement self link in getUserById Method.md
So welcome back in this lecture, we are going to implement self linking what you said by any method.

So if you see the steps involved so far, that user by the method, we are going to extract the user

data from the user object and then we're going to create a link using controller builder and then adding

battling resource, which is nothing but user data add and then instead of the user return type.

OK, so we are going to use resource user, we can type change to resource.

So we are going to do that.

OK, so let's go ahead and then implement it in other I.T..

So next, coproducer, haber's controller.

And if you see we're currently reading the optional user, right, and the end of this completer implementation,

you are going to return the resource user.

So let's do that.

Not one by one, step by step.

So the first thing is to.

Extract the user using this idea, right?

So what I need to do here is first thing is.

User user is a good start, but user about 80, so it says that change type of user to optional user,

right.

So now this has changed.

So next, let's get the user right.

So we will make this as user optional.

So whatever we got is user optional.

So I'll say user user is a to user option on top get.

OK, so now we have the user in this.

Variable know what we'll do is we'll see how long you.

Use or not get used it.

So now we have the authority, why do we need to use that 80 for linking?

We need that user 80 because we are doing the self-locking right.

So which means we need to add the prospective user 80 when you bring the self linking.

So to do so, we need to extract the user.

Right.

And you can use this idea, but it's not the right way.

Right.

So we need to extract that from our object.

So we have extracted it.

So now we have the user ready.

So now what we're going to do is we're going to create this self link.

So to create a self link, we'll say link.

Self Link is a quadruple controller link builder.

So this is the one which are going to use to construct our rail link.

You are Isaach Controller, Link builder.

Not.

Link to right and a link to this class.

OK, so they start to get class, right?

And then.

In this class, it's a selfless right, so we need to see slash slash off after slash.

What is it going to be there?

It is going to be.

All right.

So I'll see you, Zahradil.

Whatever we have extracted here, that is one.

And then we will see with.

Self-determination and self-regulation, you know, you are going to have self-regulation.

So now.

We have the SilverLink details.

So what we need to do now is as we have extended our into the story soursop, we have an additional

method under yuzu, which is nothing but use a dart ad.

So not only that, extracting the user from user option is not good for extracting the user, but also

to the user.

That ad for the SilverLink.

So let me add this, OK, so now we have the SilverLink and what's next, right?

So now if you go ahead and then test it, right.

So it's going to give a lot of other data and a lot of stuff, OK, so we can save it and then do it.

So what I can do is, oh, you can say we can use that optional, but we have to date that.

Absolutely.

So that means we need to define our resource here.

OK, so resource and then which is nothing but user.

And I will say this as says final resource is equal to human resource.

You said, and it will have no value, as you said.

Right.

So, come on, you have total input.

And if you we have different resources available, the resource which we need to improve our framework

here is resource.

Right.

So now we have important.

So now we are going to return that.

Right.

So I'm going to say return final results.

So when I am returning this year, it is optional and then I'm returning resourcing to last for the

change rate change method, return type resource user.

OK, so this could change it now.

So let me save it.

And now we have implemented the get user by itself linking no.

Right.

So let's go back to our Posman, OK?

So and this is the one right to get used to this.

So let me test this.

OK, so I listen and now I got the user details.

Let's go down.

So if you go down here.

You can see here the links, we have got our users details.

OK, said, I link to slash user slash and you know, this is the same thing, right?

Whatever we have accessed and whatever we have got, it is the same thing.

If you want, we can click on that and then send it and then verify.

And that link is working as expected, which means we have successfully created it.

Self link.

OK, so if you see the code here in the self link creation, we don't have any other methods used.

OK, but when we are doing it in the next section, we'll also use unmetered and then understand about

that one also in detail.

But for now, if you see here, forget about it.

We have created a self link losing control, that we have created the link.

And after that we need to send the user ready because it is it is what is there in the you are already

doing nothing but the idee.

So that's the reason we have extracted the user idea and then placed here.

And we have said that relation is going to be central.

And then the ATM, which we have got as part of extending into this to restore support.

We have users that use about ADD and then we have posted the self link, whatever we created here.

And then the response for these resources for resources is going to be heteros resource.

So I said that resource user, final resource, a new resource, and then we have sent the user.

Right.

So the final resources.

OK, so we have sent the final resource and then we went back to a replacement and then tested it.

And then we also ensure that we have got the self link, which is nothing but itself.

You are in here in the links.

OK, so that's about the complete implementation for better user by any method with self linking.

OK, so in the next lecture will focus on getting all users and then we will implement both self link

for each user and also implement a relationship link for our basketball orders.



Until then, bye bye.

Thank you.


### Step 64. Step-05: Implement self and relationship links in getAllUsers Method.md
Welcome back.

In this lecture, we're going to implement some friend relationship links and get all users method so

relationships will be with the data or this method in order to control it.

So if you see here, the first thing, we're going to do something for each user so you can get with

this method that each user retrieves the user details, each user detail will be there for each user

detail will have the self link and then the relationship link with the data that so far about.

Each user will have the relationship linked with that, all others for that respective user.

So that's where we to implement so far that Facebook user, the beta users, it will have that all of

us link.

So that's the key thing here in the next days for the entire users method, we can even create self

link, right, so that we are going to do it.

So that's about the entire implementation, which we are going to do as part of step five.

OK, so let's see the next level of detail of steps, what we are going to do.

So if you see these are a lot of steps here, close to 35 lines.

So I describe them in a very high level.

OK, so first firstly, we have seen in the previous letter also that we are going to put this as these

are multiple users in get our users method.

We are going to put them in the for loop and then extract the user and then create the link using controllability

builder slash and then add the user right with the slash.

Whatever we have done in your previous section, Sambit, and then we're going to add that link and

also to embedded in type from list user to resources user for the Internet users method and then tested

where Posman that complete the self linking of each user, then the relationship link with the data.

So we're going to build tables and other headways controllers and then we're going to make changes in

both of them.

So if you see here in all the papers controller, we have got all this method.

So which currently is a list who's written by list order.

So we are going to change it to resources, order for that firstly.

And we will come to you with as controller and then we'll create the link with controlling will that

in the same loop and then add the link and then post where postman finally Milada Self-locking for better

users and then we'll get the controlling builder for self link for all users and then add a link to

the resource and then we are going to test it.

So let's see all those things, how we are going to implement in our idy.

So let's go back to the idee.

So here we are.

And if you see this is the best way to use this method, which we have currently in the user, Hato

is controller.

So the first thing is to implement the Self-locking for the user side, which means for every user to

have its own self link available.

So let's do that now.

Remove this return here.

And then what it is going to return is all users.

Right?

So I'll see list user and it returns all users, so all users and then we start the users.

So next year, let me bring this up to the top.

OK, so now it looks good.

So we have got all users in all user.

So what we are going to do now, we are going to create value.

Right?

So I say fun user, user, all users.

Right.

And I'll say that.

Let's start working on building the SilverLink, OK, for you, sir.

So what else is long?

You, the lady is equal to use.

I don't get to use a lady.

So we have the user here for that.

We have got to get you to it.

So now we have the videos already next year to create the link.

Right?

So I'll say Centrelink.

OK, and then Fustiness controller link builder DOT and the for self-locking we can directly use the

link to instead of Metaldyne.

Unless if we are not able to construct the user using Lupul, then we need to go to things like we can

barely go to class instead of going to Matheran.

OK, so now will go to the class itself.

So I say this dot.

This third grade class, right?

And after that, I'd say about.

Slash, right?

And then I'll tell you that I do whatever we have extractor here.

OK.

And then I'll say that.

But self.

Nation flight and.

That's good.

So now I'll see you saw that ad and then also SilverLink, right?

So now what this does is so for every user, it will create a self link and then add that to the prospective

user in all the data that if we have our users for all four users, each user will have its own self

link.

So this looks good.

So now instead of a list, we need to return to resources, right as part of it.

So what we will do is.

Resources, and then I will say.

Yuzu and final.

Resources is equal to.

New resources user.

And I'll pass here.

There are losers.

OK, so copy and paste.

That's good.

OK, so come on.

You've total in the resources.

OK, so now next we need to return these resources.

So I return final results.

Resources, right.

And and final resources.

And if you see the return type will have the issue here.

So let me select your team, the metropolitan type of resource user.

Right.

So that looks good.

So now let me save this.

So this got saved.

I don't see any errors here, so this compared to the self linking, whatever we have done right, self-locking

off for every user created self link.

OK, so now let's go back to our postman.

And then go to people who hate us and say, send, right.

So now let's come back down here, see you see the user list here and then come back down.

So for every user you can see, it's equally self got created.

This is for one zero one.

No, this is for one zero two and this is for one zero three.

So we have successfully implemented the self link.

Forget all users method inside of it for each user.

We have implemented the self link.

Right.

So now we will move on to creating the relationship link.

So to create the relationship link, we need to first go to the happiness alternators controller and

then return resources of other things like order as resources instead of lists.

Okay, so let's go back there now.

So now we have completed the self link for this and then now we are going to work on OK.

Relationship link with the Toys R US.

OK, so let me see April here and then we'll go to our alternators controller.

In this, we have only one method, OK, which is that all orders in our hitless controller.

So I'm going to change this method to ensure that we open the sources instead of alist.

OK, so let's do that now.

So if I see here, we are going to use adoption optional, that others will give all orders for us.

OK, so I'll set list and then order and then space and then I'll see all orders is equal.

OK.

So now I have all orders in all orders variable.

So now I can add that to resources.

So I'll save resources and then order.

I'll say a final.

Resources and new resources and order, and then I'll pass the holidays here, OK, so let me pass it.

Yeah, yeah.

Holidays.

So come on shift to import the resources that.

So now we will return the final resources.

You can even say final orders are final results, orders, whatever the name we want.

OK, so now let's also change the return type of disrespectable tolerance method to resource order.

OK, so we have changed this too.

So this completes that changes for the regular haber's controller, all the controller now that all

orders will be returning in the resources format instead of at least resources.

OK, so we can check that here.

Heteros resources, the package.

OK, so I will go back to our user here to this controller.

Right.

And user hater's controller.

We are going to build the relationship link.

We get all orders.

OK, so we are first going to build them and we are going to facilitate the orders and then pass it

to the other Slinker controller to do that.

OK, so everything we can construct in a single line, which means like in a single line or we can do

it in lines, OK, so far better understanding and implementing two lines.

And then I'll also show how we need to convert it into a single line.

OK, so but I prefer to build a bit more if I if someone wants to read the code or understand the code,

it should be more clear.

So I prefer to two lines.

OK, so what I'm going to do is I say.

Resources.

Well, because of the resources stuff, OK?

So all this is equal to.

Controller link builder, not flight method on Glide.

So this is the method which we are going to use to pass the other haber's controller here.

OK, so I'm going to pass the order to this controller so that all the methods listed in order here,

birth control will be shown after this.

Once you pass that.

OK, so I'll say that it was controller dot class.

Right.

So now I'll see what you can see here.

The method presenting other people's controller is listed here, which is nothing but get all orders.

Right.

So now we have to get all orders here, OK?

And forget all about what is the input parameter for the specific user.

Right.

Right.

So I'll pass you that idea, OK, for that respect to you that I didn't get all of that thing.

So I'm passing you ready.

So for the specifications that I get all the orders.

OK, so no input.

So if I see here that this is another important thing, OK, so we can see that there is one order class

available with X persistance criteria.

So if that is important, then we are going to have issues.

So we need to ensure that we are importing our Arbella class here.

OK, which is nothing but our identity here.

OK, so.

So what are those local tribal corporate identity and then pasted here directly OK in the input.

So let me go up and in the airport.

I will import our Comstock's simplify the services into this order directly.

OK, so and let me say it, OK, so that.

That should be good.

OK, so it's unhandled exception, soils are trust, escalation, or we can surrounded by cattle cars.

I'll just say I trust declaration form.

OK, so our focus is not an exception handling here.

Our focus is on creating a relationship link.

OK, so we'll primarily focus on creating a relationship link.

OK, so let's do one thing now, OK?

And now we'll get the link link.

We're going to create our best link now.

OK, so I'll say controller link.

Builder dot link to and then I will pass the orders.

Whatever I have created here.

That one here and then not with.

The rate determination and what I'm going to say, which is going to be and all are, that's OK.

So and then.

I say use a dot ad and then I'll also add Hodas.

Link.

OK, so now we have also created this link and then added that to the results.

OK, so if you see here, one important thing is whatever we have built here, this complete thing,

OK, can we pass it here so that it becomes a single line?

OK, so and this controller linkable that you can change it to static input and then just copy from

Method on the link to you.

And that is possible.

But this looks more clearer for me.

So I followed this style, OK, so that you can convert it into other styles too.

So whatever the way we want.

OK, so now let's go ahead and then save this and then tested were Posman right.

I saved it.

Let me go back to the postman and then say it was almost a what was said to let me say it sounded so

no facetious here in the links here we have only phone, but now we have got the all other sling.

So if I click on user one on all of those, it will open a new tab.

And then if I send it so far, you were wondering what all others are there.

Those are displayed here.

That's good, right.

So which confirms that our better users method, which we have implemented for both self and a relationship

linking, is working as expected.

So which means for the user, we got both the links for itself and also for it has a one to many relation

with the others.

And then those are the limited information also we have.

So which means from our friend and client, if we are accessing the user and then I want to also display

the others, then just like Klein will try to handle using this link instead of instead of storing these

links in separate places are handling everything.

We have the link ready to click on it to get for disrespectable users while others are available.

So this completes the second part of our implementation, which is nothing but Fabi relationship link

would get all orders.

So now the final thing, self link for BATTAL users, this is a smaller thing which will do it now.

So if you see here how.

There is this Getúlio that's right.

So let me make it a little small.

OK, yeah.

So if I see you down so we don't have any self-loading further and further use, at least, which means

for better use, this method.

We don't have any self link here.

Right.

So let's go ahead and then create it now so that also we can do it with the one line.

We are saying that self-learning first.

They tell you this, right?

So I say blink, blink.

I can even say this as the link link is final.

I can see SilverLink.

Forget all soccer.

So.

Controller link in the DOT, link to flight, and then I'll say stop.

That plus and their self, not self regulation, OK?

Now, I have this feeling that values us right, for this so called pastor, send it to our resources.

OK, so that's all and then save it.

OK, so let's go back to our postman and then test it, OK, so now let's go to the end.

You can see that we'll have the self link for the complete almost a this method service.

So I'll click on that.

And in the new screen again, I listen when I got the data right.

So which means it's working as expected.

So this completes several facing section, which is self link for what, all users.

So just to reiterate what we have done in this entire section, so this is a little bigger section out

of all other sections.

So what we've done is we have created it self link for each user in the data users method so that every

user will have that self link.

And in addition to that, we have got a measurement uplink with the button riders.

OK, so every user has multiple orders.

It's a one to many relationship, right?

So from users to others, we have created a relationship link with the rail.

And when we are doing that, we have completed our entire code into two lines, which gives us more

convenience.

OK, so we have done that.

OK, so in the second the last one is we have also created a self link for this complete get users method

and then pass it to our resources here and then test it on the postman.

So this completes the complete implementation with the different different options available for us

from information perspective.



Until then, bye bye.

Thank you.


### Step 65. Step06: GIT commit code, push to remote, merge to master.md

Welcome back.

So we're going to finally get it caught and then close this section, so let me go back here and I will

copy this.

I copied this.

This will be more than enough for us.

OK, let me go back to our comment line and then I'll get a status.

And then I am in 07 spring.

But it is OK, so I'll say it clear and then I'll say get.

Had good commit.

I'll say it was first it OK, and then I'll put this to the remote repository branch, OK?

I got so I'll clear and then I'll get Check-Out Master, so now I pasted here, which means I'm going

to and springboard here to master and then I'm going to push this branch also to wherever the remote

repository.

OK.

Good, so this completes our completed section.

So in the next section, we'll discuss about the internationalization.



Bye bye.

Thank you.

