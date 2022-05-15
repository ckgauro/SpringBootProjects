### Step 92. Step-00: Introduction to Swagger.md
Welcome back.

In this section, we are going to understand and implement Swiger integration with Springboard.

So if you see here, swagger like is primarily for documenting over the EPA.

So documenting the EPA is very important, primarily from a consumer's point of view.

Yep, documentation helps consumers are the consumer developers to understand and implement their client

applications without any confusion.

So which also avoids the costly mistakes at the later stages.

One of the most popular documentation specifications is Open API, formally known as Swagga, so Swagga

allows us to describe API properties, either using Jessner Yamal metadata could also operate a website

which transforms the metadata nice Hesterman documentation, which we are going to implement and see

in our upcoming lectures.

So I can also be used as a test client, which means earlier we have seen Posman as well as client for

testing over the stapes so we can use even the very word as it was claimed for best director.

Yes, yes.

We'll see how we are going to do that.

The same swagman integration framework can be implemented using spring flux dependencies.

They have the dependencies which we're going to update in our problematic segment to implement the Swiger

integration with the spring framework.

If you see here, this is the sample swaggering, right, which we have generated, so the top part

here we can see is our header part so far, our respect to our organization for our respective apes,

we can generate our head.

That means like we can customize our head as our need.

So I can say that here it is to simplify user management vestibules.

I also provided a description saying that this page lists all APIs for simplified user management.

In addition, I have also provided the complete contact details so it has the website, email and license.

So now moving on to the services.

So we have who controls your user management controller and then other controller.

So you can see here we have customizer here.

You can see the other controller name here, but you can see your user management, restful services.

So we have customizer with this name.

In addition, we have also provided the description and the symbol for the method.

Also, we can see we have provided the customized description.

We are seeing the true list of users create new user.

But if you see for other things, you can clearly see it's like the method name update user by the delayed

user by 80.

So which means.

Swagger, parades, different connotations at country level, modify these things.

In addition, it also will help.

Listen to controller level annotations, we'll also have more than level annotations from Spatt Swagga

to also describe our model class and also the model fields in detail.

So we will see all those things in our upcoming lectures and then implement them with HANDSON.

So let's move on to our implementation steps for this aspect of Swagga integration.

So Mobilizers will start with the new brand for Swagga implementation and then we'll move on to other

dependencies in other problematic Semmel for Spring Flock's.

Then we'll move on to creative swagga config file.

So we'll try to add one in two steps in over one letter and then we'll accommodate the lectures accordingly.

So.

Next is adding a plane for a modified header, part of other documentation, if you see here, we're

going to modify the overhead of so by default swap that provides a default ahead of seeing the documentation

in some stuff.

So we will modify our needs are our organization standards and then our organization will like based

on our our nation name or our application name, all those things we are going to change and our contact

information, etc..

So the next is the scope of swagger Bachmann generation using your base packages and then bot's.

So the first thing that we have built multiple controllers as part of our previous sections.

Right.

So by default, whenever, as soon as the inevitable swagga, all the controllers will be listed and

then all the APIs will be listed.

Right.

So in step five, what we're going to do here is we are going to control that using best, best packages

and also the parts.

So let's see how we are going to do that.

Another step.

Then we'll move on to the step six and see how the swagga documentation can be on how to populated for

desaparecido.

Three validations, nothing but the bean validation API.

Right.

So if you remember, we have added another user entity it and then added marksman's like annotation,

annotation, Max, we have added and this commander asserted that revalidation sabeen validation APIs.

So so these annotations when we apply them.

So swagga integration like the Spring Fox can also generate those additional documentation information

at the model level.

But then it can do that is we need to add additional problematics which is provided by Spring Fox and

then we're going to add that and then see those details in detail.

So in addition, we are also going to use.

Quote, annotations for model flashes to describe our films and then class in detail so that we can

see that on other documentation.

Finally, we're also going to go and then implement our contralateral annotations for Swagga and then

also verify them.

And then we are going to out and push forward it.

So if I see all these steps in detail, you'll also go through them once and then we'll move on to the

next lecture.

So let me go back to Albert.

Fiasco.

Right.

So here are the detailed steps that we are going to perform.

So if you see steps zero one is going to be able to springboard swagged IPE documentation and then we'll

move on to adding other dependencies listed here.

That is playing Volkswagen, too.

And then spring from Swagga UI.

And the latest version is to Ninetto, which we are using again today.

So and then we're going to create our swagga config file and define the target, be inside that and

then tested both the Swiger metadata Eurorail and also the.

So are you are you worried and then as I said earlier, we're going to customizer that part of our documentation

here in step four with EPA for and then verify that swagga your way.

Next, we'll move on to implementing the scope of Swagga document generation.

All this three, four, five will be in our docket been only and it's like in the swagga config file

on level playing in that area to implement them.

Then we'll move on to step six, which is nothing.

But there's a three zero three validations which need adding of additional dependencies.

Spring Fox being validators will add that and then we'll add an input on the swagga config file and

then we will test it under Swagga.

You will go and then verify our model.

Whether those details came automatically are not.

In addition, one more step seven, which is nothing but model class annotations.

We have two types of model plus annotations.

One is the AP model and then a pay model property.

So we are going to apply them on each of the fields like we are.

The fields will apply and then understand them so we'll know about what is required field.

In addition, what is the position field we are going to understand and then implement them.

And also what is on our data on our that we are for displaying the field, then position is not in place.

So but also we are going to look into then we'll move on to the step that is Swagga called annotations

to the controller classes.

So we have a PPA operation and then para, so we are going to see them in detail.

So once that is completed, will move on and then come out and push the code where I said let's go ahead

and then implement all these things step by step.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 93. Step-01: Add Springfox Dependencies to pom.xml and Create SwaggerConfig file.md
Welcome back.

In this lecture, we are going to be good brunch and then add our Spring Fox Swagger later dependencies

to our problematic symbol and then we'll create our swagga config file so that our application, Springwood

application will be enabled with the Swagga.

And then we will test both the Jason and Jason who are in this world that you are you are you Warren?

And then we'll move on to our next lecture.

So let's go back to where we are here.

So we create our first step that is adding the new GI branch, OK?

So our master is in sync with our previous brand, so contract negotiations will create a branch from

Master, right?

So I'll say to Wellspring, good swagger, API documentation, so continue.

So my JVM isn't running straight.

Let me stop it, OK.

So anyway, we are going to make from that simultaneous right.

So anyway we need to restart it and stopping it.

So let me go here to our Walmart example.

Right.

And copy our two dependencies.

One is Spring Fox Swiger and the other is Spring Fox, Swiger UA.

And both has the version about nine that to OK, which is the current latest version.

So let me go here and then added at the and.

So one thing we need to remember here is we need to restart our Ambre Tomcat whenever we make or add

any new dependencies to our Bombach XML, so I have already started it.

We should be good.

In the step three, we are going to create swagga config file annotated with configuration PAPEN Spring

that it's a configuration file and then annotated with the swagga to OK to enable the swagger to so

and then we're going to create a had been.

And then once that is completed we are going to save it and then verify the following things.

OK, so optional user response fixes we will do in our next lecture.

OK.

So for now we'll move on with implementing these things.

So later I have made a note of it here.

Right.

So fix optional user responses.

I'm going to do it at the step five.

OK, so we will discuss about that in detail when we are implementing it.

OK, so now let's move on to our role creating swagga config file.

So we have a conflict package here.

OK, no application.

So in that, I'm going to create a new class named Swagga Config, OK, so I'm going to.

So first we are going to annotated with configuration.

Right.

And put it.

So next is enable.

Swagger, too, right?

So done so the next thing is to create our docket, Bill, so I will say a public docket EPA and then

I'll see it on the new docket.

Right.

So when returning, I'll provide the arguments.

So documentation type that we are going to tell that that we are going to use the watch and two of swagga

specification.

So documentation type is swag that we are telling the docket that we are using the swagga to.

And we are also going to say Sellick.

So what does this relate to is what's happening so we still don't import the docket.

OK, yeah.

So and then once you select OK, so the Senate creates a binder which is used to define which comptrollers

and which of their method should be included in the generated documentation.

So under that will select the purpose.

Right.

So EPA's defined the classes, which is nothing but controller in the model classes to be included.

Here we are, including all of them, but we can limit them by this package.

Are class sanitations and more options available.

So in the next upcoming lectures we will restitute with the best package is Fano.

We will say request handlers let us not any.

So I will say.

The Quest handler, selector start any light, so now APIs are completed, so the next part's OK.

So but select us OK, so Pott's allow us to define which controller method should be included based

on the part mappings.

OK, so in a single controller also we can hold specific parts and then provide a part of it and buttons

to be finally specific methods to be exposed.

OK, so something like that, whatever we want, we can do even it allows the digits and then and buttons

for it for us.

So I'll support select test that any so that fano all parts are included.

Finally I will say.

All right, so what this does is like no it will be built.

OK, so now our application is enabled with swagger.

I need to restart this.

Has it been in the spring context.

OK, so come on, you've got to annotate it would be the important stuff.

So one final thing here is.

Our swagger, metadata and our swagger.

You are you are OK.

So I'm going to write them here so that whenever we are testing, it will be handy for you.

Right?

So I'll see localhost.

AT&T slashed me to slash Ippei hyphen dock's.

So this is our swagga metadata.

You are.

And this is swagga.

You are you all right.

So that is nothing but localhost AT&T slash.

Swear that you are not looking.

So let me save this, OK, so now let's start our application.

Then, as I can say, Springwood up.

So it started OK, so no issues, so let me make it bigger.

So let me copy our metadata.

You are all first, OK?

So and then pasted here so that all the control information, everything will be provided here in the

Swagga Jason file.

OK, so this is the address and metadata we have got the same thing will be shown in the nice format,

which is nothing but our swaggering way.

So this is a little uneasy, right?

So what we will do here is we will try to take this unmoral and then we have the same Gissen using UI.

OK, so let me see Swagga.

You write out his HTML.

So if I see here that part you can see here, this is the API documentation.

So you can see here the documentation and the basic rodell and the API documentation subheading terms

of service license.

You are a lot of stuff.

We can put our contact info for everything.

So that's about this area no matter what.

So no one coming to the controllers.

You can see that we have the basic error controller, Hollowell controller or the controller or the

notorious user.

So whatever the controllers we have created as part of all the previous sections, we can see all of

them listed here, including the very least incision's like user media type in controller, user model,

map controller, everything OK?

Everything we are able to see here.

This is about the controller section in the same way will also have the globals.

OK, so whatever the models we have in our application, but also will be much like nothing but the

beans.

Right.

So we can see here everything.

OK, so this is our user model.

OK, so user details, user data will be one, user data will veto.

So whatever that means, we have defined all those things were displayed here.

Right.

So that's about the models.

Now let's look at something here, which is nothing but the basic error controller.

OK, so this is we didn't define this.

OK, so how will this coming?

So that's coming because we have selected nothing but the request handler select us any, which means

from all packages it will scan and then send it.

Know what we are going to do in our next step is we are going to restrict it to the package level,

which means we have something called our packages are at the level of.

To simplify the services controllers so we will even less dictate the services or code packages here,

right, Comstock's simplify other services so we can restrict so that only our controllers and then

our models will be displayed instead of everything.

OK, so this basic level of control is coming from the spring.

OK, so that's about the first three steps which we have planned to understand and then implement.

So those are creating a brand, adding dependencies and then creating a swagga config file and then

using our swagga metadata, your model and then reviewing our swagga you where you are.

OK, we have also created the bucket built and then annotated it with Swagga two and then configuration

both the things.

OK, so in the next lecture we are going to customize our header.

Right.

And we'll also look into adding Guevarra restrictions to our request time slots and then also the part

select us.

Let's see how we are going to do that in our next lecture.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 94. Step-02: Adding API Info to modify header part of our documentation.md
Welcome back.

In this lecture, primarily, we are going to focus on adding EPA for to modify that part of our documentation.

If you see here, we have the documentation very generalized here.

OK, so this one, we are going to change it to ask.

But our organization needs, like our application is user management service.

So we are going to change to user management service documentation and we can update our terms of service.

What else are license information?

Additionally, we can add our complete contact information with email.

Why?

Because these API documentation will be consumed by the dollar parts who are building the client applications.

Right?

So client applications are going to consume our APIs.

So definitely they need some reasonable information here stating that this is the contact.

They can go ahead and then contact me if I have any issue with any of this service I am accessing during

the development, even though we are providing a very detailed documentation that will be needed like

that.

OK, so for that purpose, providing the complete contact information here would be a good option.

And Swagga provides a method.

New contact method will be available here to even provide that email you Wadle and also the name of

the user.

Right.

So like that for the contact.

So by default it provides one method internally in the spring Franck's.

So we can use that.

So let's go back to our detailed steps.

So in the step forward, we are going to add a painful to modify header part of our documentation.

So we are going to create a new class named Hyperion four, which will have the airplane for bimbette

inside that.

OK, using that, we are going to generate it.

So let's go back to our idea and then we are another swagga config file.

Right?

So I will say private.

A plane for get a plane for.

And I'll start with you new.

EPA info builder, right, and so we'll say the title, right, let's start with the title.

OK, so I'll say Stack.

Simplified user management service, right, and then we'll move on to giving the description, OK.

So in description, we'll say that this page lets all types of user management OK.

And I can also find the version.

So I will say Russianness Grubert zero.

Right.

And once version is done, this comes to the contact.

But so you can see here contact, you can basically give it away, click on the operating table, but

you also have the contact contact.

So which means you can create a detailed contact information.

So I'll send you contact.

And then I can go inside that and then see what is that OK, so first thing is to import contact from

swagger.

My models is one thing and then Spring Fox Documentation Service.

So we are working on the documentation service.

So the contact me to be imported from Spring Fox Documentation Service.

OK, so we have imported that.

OK, so it has the three Single-Use contact string, string, string.

OK, so if you see that in detail, so if you see the open implementation of the contact you can see

here, one is name address you are and then another is email.

So we need to go that way.

OK, so let me go ahead and then name you all and then email so you can contact.

OK.

Ready.

OK.

And your are is going to be.

Stacks simplify dotcom, and finally the e-mail writes, tax, simplify and direct Gmail dot com.

So I give some email idee, some name and then everything.

So the contact part is completed.

So the next year we can also provide the license details.

OK, so license the string.

Right.

OK, so I'll say the license says license 2.0 or something like that.

OK, just to give something.

OK, and we can also give you the license you are able to, which you are allowed to reference doing

that.

OK, so I can say that as ok.

Dot com slash license, dot hesterman, look, some you order.

And then finally we will build this response, OK, and then save it.

OK, so if we go here and then see we have created the EPA info but this is a plane method which we

have created.

We need to call this in our bucket.

Right.

So let's go ahead and then call this in our bucket.

So here in the bucket we have something called EPA in four.

OK, so EPA in four.

This is the OK, and then let's call the Mitra's get EPA info.

So now we call that in our docket.

So let me say it right and let me go back to our.

Browser and refresh our browser.

So sorry, I typed commander here, I really it is Windows, right, so now you can see here, right.

So I have reforested you can see here STAC Simplified User Management Service, and it lists the description,

whatever we have when this person is all a piece of user management.

So we have also provided the contactors calendar day and this website has some stock simplified dot

com in the same way we have also provided the e-mail stack simplified direct Gmail dot com.

So it said that send email to collaborate with that.

Again, the license to Bobzilla, we have given the name and you can see that the link also pointing

here.

In addition, the version we have given here.

So it is also displaying.

So this completes several disrespect to step whatever we have listed here, adding your playing for

to modify header part of our documentation.

Right.

So in the next lecture, we will focus on implementing the restrictions for the Swagga document generation

at select US level and also the base package level.

OK.

And in addition, will take our swagga, Jason, and then verify in our Ed and then fix a few things.

OK, so we'll see all the details in our next step.

So I'll see you in the next lecture.

Until then, bye bye.

Thanks.


### Step 95. Step-04: Restrict scope of swagger document generation using API Base packages.md
Welcome back.

In this lecture, we are going to restrict the scope of the documentary using your PBS packages and

then Putzel.

So let's go back to our detailed step here.

So in this tape, we are going to update the best package and request handlers and actors with the best

package and the combat stacks simplified out less full services so that whatever we are seeing currently,

it is nothing but basic error handler will be disappeared.

Then we will move on to the parts and actors and then select the and partner and then use user our star,

which means we will limit the scope only for our other controller and also the user controller.

And in addition, we will also verify the format of our swagga in the sense like we will take over Swagga,

Jason, and then put it in a little box that able to validate our Jason.

Complaint's right.

Whatever we have generated, whether it is in 100 percent compliance, are not will verify it online.

OK, and we are going to see if few compliance issues and then we are going to fix them once we see

those.

OK, so let's go ahead and then implement all these steps now.

So let's start with implementing the request handlers that select US based package.

So let's go back to our swagga config fighting now.

So here is our Smadar config file.

So instead of.

And we are going to change it, too, so before that, we'll crosscheck what we have extra we see that

we have the basic error handler controller coming in now currently.

OK, so let me remove this now.

OK, so I will say that the best package.

OK, so what is our best package.

Our best package is.

We can see it here, our best package.

Is going to be this one combat tax simplified that the services, we're mainspring application are present.

Right.

So let me go to Swagger, that swagger config, and then I will provide our base package here, OK?

So this is our best package.

So combat tax simplify, not less services.

So let me save this.

Right.

OK, so it's Godsil.

OK, let me go back to work your way and then enter.

See now the air controller gone.

Only the controller is present in our respective controllers packages coming up here.

So which is means like only it is restricted to this package.

OK, so this this is the best package.

So now we'll move on to also fixing the Pozzallo.

So we have multiple controllers displaying.

No.

OK, we'll try to fix that.

Only international.

That's for which controller we have slash users.

Last stop, stop.

We are going to use them.

See if you see the user controller, it starts with the slash users.

If you see the controller it starts with slash it in the same way.

If you see orders controller again, it starts with slash users.

OK, so now we are going to put the portal slash user slash stature and button so that whatever is starts

with slash users, only those controllers we are going to see.

No.

So let's go back to our swagga conflict.

OK, yeah.

Yeah.

And then in the pod, select us.

What we are going to do here is so H.M.S. and string pattern.

OK, and I will say that slash user slash starts to OK and then double code and then say OK.

So now our division got rebooted, right?

So let's go back here and then refresh it.

OK.

So now you can see only two controllers are coming for us because only these two controllers have starting

with you.

So now we have only two controllers and then we can see them here clearly.

Right.

So let's move on to the next step in this.

OK, so which is nothing.

But now we have completed both the base package and the Pozzallo testing.

So now we are going to verify what this and whatever generated in the edit about Swagga that I want.

So let me copy this.

You are all OK.

Go to the browser and provide this.

You are here.

OK, so let me remove whatever it has currently, OK?

And let's refresh our metadata.

You real fast rather right.

And then copy the content which is present inside that Jason tag.

OK, so let me copy this and then put it in our swagga ed.

OK, so we should throw at us first with optional use in an optional order.

Let's see.

OK, so currently the string only four other optional user because optional either way anyway didn't

implement here.

OK, so it is saying that semantical apart user slash which means like that user I.D. service.

OK, line 166, you can see there is some issue, right.

So you can see it's retaining optional user.

OK, I really need me to return user object.

OK, so let's go back to our idea and then open our user controller.

So I am holding this one from multiple releases, which means like from multiple sections just to demonstrate

that in our swagga config, OK, so that nothing but in our swagga we can whatever the decent generator

using swagga, we can go ahead and then on line in the online swagga ed, we can verify whether it is

open, API compliant or not.

So for the purpose I just hold this.

OK, so let me come here and then fix this, ok.

So currently it is retaining optional user will try to return this onto the user object instead of the

optional user.

So I'll say user user optional is equal to user service.

Don't get usability.

Fix the broken pipe here.

OK, good.

So now finally we'll return.

Use it optional, but get.

What happened this week?

Right.

Yeah.

Is it optional that get little he can use that for us?

OK.

So let me also fix that we can type here.

So now this metadata is about I will be returning the user.

OK, so let me say this.

It is saved.

So let's go back and then remove this complete content.

Refresh our Apaid Jason data here.

OK, so one more time I'll reflect just to be on the safe side.

Yeah.

And then I'll copy this complete thing here.

Right.

I will copy and then go to Swagga online editor.

OK, copy.

Right.

So now if you see that, I admire that.

OK, so which means would so I got this and whatever it is generated we can validate it online and then

ensure that it is open API compliant or not.

OK, so that's a very good feature.

Right.

So that's what we have done to install.

Things are coming as expected.

OK, so let me go back here.

So now we have done the fix optional user thing also we have completed.

Right.

So let's move on to implementing the other steps.

So before going there, we can do one thing here is I can add one more step here, OK, seeing that

test flight test using.

This kind of swagger, swagger can act as it just claimed also, right, so I'll add one more step here

and then let's do the testing now.

Right.

So this is our swagger your way, and this is our user controller.

So we can click on get OK.

Right.

And if you see here.

We can say it says that right out here, right?

So get all you the slave trade.

So far, there are no parameters required.

So I just can say execute.

So I have executed it.

OK, so let's see, what is the response here in the Southwest response, OK.

And I got the user one zero one, user one zero two and the user one zero three.

And I also got the response orders right.

Applications, Ladson and then everything, whatever is required there.

And then it's said 200 or so, which means now in addition to that, we used to use the post mandate

to do our testing.

So now we are using the Swagga UI, OK.

So that's a good thing, right?

We'll also do one more testing using.

USERRA, right?

So this is the way you should try it out, right?

So what we need to send we need to send the user to get that user data right.

So I'll say one zero one user and then I'll click on execute.

Right.

So if you see here the responses that I did file the request and then request you, our listeners users

dash one zero one.

The response is 200.

And you can see one zero one data got displayed.

Right.

So with everything entering, so that's about the address to client means, like even the swagga, you

can act as it was claimed to do our testing.

So that's about the.

This client information about swagga, OK, so now in our next lecture will focus on implementing other

steps.

.

Thank you.


### Step 96. Step-05: Auto populate documentation for JSR-303 Validations.md
Welcome back.

In this lecture, we are going to highlight appropriate documentation for these three validations.

So in the spring frogs, we have an additional dependancy here to do that.

OK, so.

For our entities, we usually apply our are three zero three validations, even we have applied it if

you see here.

So only for one in one field, we have applied it also.

Right, because the state is for our implementation purposes.

Right.

Just for our learning purposes.

If you see here, you can see see it that size is equal to minimum two.

So this is one of the three zero three validation.

OK, so I can even see.

Max is equal to 50, OK, and I can even say we're talking right.

In addition, we can also say for the other thing also.

Right.

So I can see.

Here, right, so I can write for the username, I can do the same thing, whatever we are seeing here.

OK.

OK, minimum.

Minimum one and then minimum two and then maximum 50, right?

So I have added for you that and then I have added for first time we can have some other things like

Batton and all of that stuff also will be available so far, seeing what our Laura.

Oh, yes.

At Revalidation related annotations, we can do it for this mini validation, that argument that you

respect the respect, pick whatever is available currently.

OK, so let me go here.

Take your.

So latest, I think, is 2.0, I didn't remember.

OK, yeah, it's 2.0.

OK, so let me review this.

OK, so good.

So Bean Validation 2.0, we can find all the details about what all this Paektu annotations are available

for us.

OK, so but for now, our core goal is to ensure that forto attributes we have under them and annotations.

Right.

Which is nothing but that there's a three zero three complaint annotations.

So what we are going to do now is like we are going to ensure that its related documentation generates

automatically for the models.

OK, so you have seen the models here, right?

So these are the models.

So if you see here in the models for the user, right.

So for first name and then we have applied it for water.

So you can see here it is for the first name and then user name.

You don't have anything auto generated currently.

I can even refresh it once, OK.

OK, so let me go to a user model here, and you can see there is nothing generated from the user name

in the first name currently, right.

But after making these changes, right after adding the spring Fox validators.

Right.

So disrespectful dependancy once we added so minimum lengthy Swainson maximum Lindstrand so the beam

validation related, the documentation will be auto generated.

So let's go ahead and then see that now.

So let me go here.

Copy this dependency group with the product XML.

OK.

So here is the problematic symbol.

Right.

So let me go down.

Yeah.

Pierced, right, so.

Let me say it, OK?

So now, as we have added the new Josephite new dependancy, I have stopped our JVM and then I'm restarting

it, OK, so it should be up soon.

Let's go back and then verify it, OK?

So now it should not be there.

OK, because we also need to perform one more step.

OK, so if you see here and use us, we don't see that for use right here.

First thing we don't see other bands to any other extra information.

So let's go back and then add the validation plugin configuration class at our swagga config.

OK, so let's go back to our swagga config here, OK, and then import this.

So sorry.

So come on Shifta.

OK, and then see.

Right.

So now we are at the beam validation plug in configuration class in our swagga configuration.

So let's go back to our swagga you way and then refresh this, ok.

So now go to the models and then go to the user.

Now you can see that for the first name is two and then maximum Leontes Whuffie and for the user name

minimum length is touring the maximum Leontes 50.

So that's all about this respectable step, which means Harbage ended up being validation related documentation

on this swagga.

OK, when we do the following steps, which means like at the spring Fox being validators dependancy

and then Imperva being validated plugin configuration class on the swagga configuration file.

OK, so and then that's all.

And then it will generate these values means like what.

Whatever have been validation related things are there all those things will be auto generated.

So that's about this step.

OK, so in the next step will focus on swagga code annotations related to a pay model and then a pay

property.

OK, so I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 97. Step-06: Adding Swagger Core Annotations to Model class.md
Welcome back.

In this lecture, we're going to add a swagger calling attention to our middle classes.

OK, so you see the steps here.

So we have two primary annotations here.

One is AP model and then the AP model property.

In addition, for all the swagga core annotation related things you can read for this document I have

provided here.

OK, so for easy reference.

So first, what we're going to do is we are going to implement a class level annotation and then test

it in the class level annotation.

I'm saying that AP model is that annotation I'm saying and then describing that what this model is for.

OK, so let me go here and then see a pay model and then provide the description of this model.

OK, so.

I said this model is to create a user, right, and then I will save it.

OK, and let's go back to our this one, OK, and then let me refresh it, right.

OK, for the user you can see here, the description is this model is to create a user.

So for the models, we have got the description.

So the next is to create the model property.

Right, EPA model.

Property rights primarily, it will help three things, OK, come on, you have to OK, so one is not

OK, I will say.

Auto generated, unique, Heidi, like this one and the next one is so whether this film is a required

field or not.

OK, so it's quote, because it's a highly rated primary key, but it will auto generate.

OK, so and the final thing is position, OK, position and status one and then say, OK, so understand

step by step what is not what is required.

What is position now.

OK, so let's go back to our

Google Chrome and then refresh our swagga you way.

Right.

If you see here I can control plus plus.

OK, Immortal's, if you go here in the users you can see here you sat, right.

I said it does.

Required to do so, then it started listing WordStar here.

It's a required attribute.

And another thing I said, the note says op generator Unicode.

It is displaying that here.

That's a good thing, right?

So far it is clear.

So now I told position is equal to one.

So then why it is showing at the end.

Right.

So that's the key thing, right.

I said position is equal to one means like in the other it is going to be the first one.

But these are whatever you are seeing here are not all the fields, which means this doesn't have any

position defined.

So those will be listed in the order, which means take the address after that e if you or are in alphabetical

order, the rest of all other things so fast on other things will be listed and then after that the

other thing will be listed.

So we'll go ahead and then apply the proper title username and then give position as to when it should

come after USERRA.

So let's go ahead and then do that now.

So we have seen the required property through further use that lady with the red mark here.

Right.

So in the same way now what we'll do is we'll copy the complete thing and then paste it for our username

username.

I will say that.

User name should be OK.

Something like a.

You have any name?

OK, which means first character of your first name and then your name.

In addition, I will say example also you, Halsy Cariddi.

Right, and I'll double coated.

OK, so I'm also giving one more thing here, which is nothing but example.

Right?

So we have it in our package.

OK, pay model property dot example.

So I'm saying be quiet is for this one.

I don't need to be.

They're OK.

And finally, the position is going to be OK to right.

So now what we have defined for our username username should be if Ellner should be informed, I'll

say just something like informative and then I'll just return something.

OK, so don't worry about it, OK?

And then example is Cariddi and then and said quote is false and then position is too and then let me

save it.

Right.

So now what should happen.

It should display that username as the second one after he was already in position and also displayed

normally without any register.

Right.

So let me see, refresh it and go to the model and go to the user.

And if you see here, your idea is good.

And then you got the user name right at the second one.

And you can see example Cariddi came in from lambkin max length game and then username should be in

format F.L. name plate.

So that's all.

So we have explored the following things in this.

Model Sweida annotations for Swagga, OK, for model classes, we have put annotations on his AP model,

which describes the model.

So we have given the description and then this model is to create a user in the same way.

We have also worked unfillable attribute named Ippei model property for level annotation.

OK, so we have given the models for the description and if it is required true then it looks like says

Red Star.

OK, so that we have seen currently that start right in the same position.

Also we have same position is equal to one and then position is equal to do how they are displaying.

In addition, we are also given one example and then provided located here.

OK, so like this we have implemented the model class with the swagga annotations.

OK, so you fabara validation.

The letter DSR three three validations are not sufficient.

And if you feel like we also need to provide additional information that to the user of the consumer

who is going to consume our reps, then we can use the AP model property and then a model.

These things are the model class level to implement them.

So in the next lecture will focus on implementing the annotations Swagga annotations for a lot of Sakakibara

annotations for our controller classes.

OK, so I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 98. Step-07: Adding Swagger Core Annotations to Controller classes.md

Welcome back.

In this letter, we are going to add Swagga Common Core annotations to our controller crisis.

OK, let's see what all those annotations are and then what we are going to implement them.

So if you see here in our step out here adding Swagga Common Core annotations to our controller classes,

look at the controller level.

We have something called API.

And at the method level we have something called API operation.

Under the parameter level, we have something called API Barum.

So for these things, every attribute we are not exploring, but at a decent level, what is good for

us?

We are trying to explore and then implement them.

Oh OK.

So let's start with the API for our controller level, ok.

So let's go back and then we'll go to our user controller.

Right.

So on the top we can add the controller annotation here.

OK, it did it, Ippei.

OK, and we have three things here, one is tax, OK, I will say user management.

First, full services.

This is my bad name

and the value I can say it is user controller.

And finally, description description, I think is deprecated now in this new version.

But we can add it just controller from user management service.

OK, so we have completed adding this now.

So before saving it will go ahead and then see what is currently present.

OK, so.

If you see the user controller, you can see it here it is user controlled user controller, that is

what you are seeing.

OK, so let me save this, OK?

And how the tags changes that display of that.

OK, so now I saved it.

And then let me refresh this.

See if you have seen user control or user control.

Now you can see user management, restful services and controller for user management services.

This is coming from the description part.

So that's why I do the thing which we have done with the API annotation.

So the next thing which we need to focus on is the API operational level annotation.

That operation is nothing but the method for us, correct?

Right.

So what else is like for Catalist users method?

What I'm going to see is API operation.

Right, that is that AP operation.

And.

Depen.

Are missing attributes, I'll say value is equal to.

Gritli list of users and first before saving, let's see for a list of users what we are seeing there.

OK, so here we can see.

First one is the list of users.

I'm getting the method name that all users.

So let me save this, OK?

It seemed OK, so let me refresh and once we refresh, you can see that really ugly stuff.

User took a more detailed explanation about this, OK, which means like a more detailed text about

it, saying that it retrieves that list of users.

Right.

So in the same way, we can copy this and then pasted from our post mapping, which is our clear user.

Right.

So I can see.

Creates a new user say.

Right, so let's refresh this and see.

You can see we got the great news, and for other things you can see the method name is coming, OK,

so that's about a direct EPA operation, right?

So the one thing which we are going to implement now is a direct EPA parum, right.

So we can even copy this completely and then further create user, so we are seeing that user information

for a new user to be created at the bottom.

So I'm looking at the pyramid and then just go space and then come onshore flow to import the Epuron

package and then say, no, let's go back to our browser.

And refresh.

So far, our create a new user, you can see here the description user information for a new user to

be created.

So whatever we have given in the API Perram, we have got that.

OK, so that's about the.

EPA apparently related annotation, so what we have seen so far is three annotations, so one is in

the controller, one is at the control level API and in the method level, it is Epper operation and

in the bottom level it is API para.

So let's go back to this one.

We have one more call.

It's not annotation, but produces.

So if you see here, forget all users you can see here.

Right.

So.

This content of Slashdot, if you want to get this, has applications like this and what you can do

here is so just go to our users photocell Getúlio.

This is the one.

So I will say in the get mapping producers is a call to media type DOT.

Familiar type, that application, Jason, right?

Application, Jason value, right, and then sell it.

OK, so now let me refresh this.

And now if you see further Twitter users, you can see here instead of starts NASDA, you are seeing

applications like this.

And so like this, we can construct automatically our entire API documentation.

And once it is constructed, it becomes easy for all of our consumers to implement it in a fair enough

manner for their clients.

OK, so these are the things which we have gone through and so far.

So if you see here in this lecture, we have focused on creating the EPA, EPA operation and then EPA

program and also the media type applications.

Yes.

And for our all users.

OK, so this completes the complete implementation of all the Swagga Forever Springwood project.

So if you see the steps again, we have created a good brand.

We have added the spring Fox dependencies.

We have created a swagga config file, and then we have defined the had been inside that.

In addition, we have also defined the EPA in for custom and custom method there and then added all

the Almazan little contact information there.

And then we went back and then also implemented the scope of this document by adding the scope to or

limited area.

We would like only for the users and less users context only to be allowed in the same way for what

we call OK.

We went back to this are three zero three validations and then implemented them and then also tested

them after generating Arato, populating the data by adding a new dependancy there.

And we also implemented the model level code annotations.

And then now let us we implemented the controller level code annotations.

Finally, what we need to do now is commitment push.

We're already.

So let's go ahead and do that now.

So I'll go to the good staging here and then I will say pull all these things right.

And then this this module is swagga, right?

Swagga first comit.

Right.

And then I'll commit and then push so it will create a tool, springboard, swagger, API documentation

to later branch in our remote repository.

We are good with that.

So let me click on finish.

Right, good, so let's see the perspective, go to the remote and then cross-check that, OK, it created.

So now we need to go to the master, right, and then continue stop the JVM.

Right.

Plus all these things which we don't need.

And master, we are going to Margalla, the Wellspring Bushwhacker documentation branch.

OK, so I'll say much.

Right.

And one Springbroot Swagga documentation.

This is their target which looks like this is the Branton margin to the master soil.

So much.

Right.

So now this comet could be triploid one for should come for master.

Let me refresh and then see that.

Right.

So let's refresh.

And we got that, OK.

Now let's push this branch, OK, so that in a remote also it will be in the same level.

OK.

Bush saying first five to seven sections of this entire course, we have focused on working on getting

better things, using our command line.

OK, get commie target Pusha, get set up, get Bush set up upstream.

All those things we have learned now in the last three to four sections, we are trying to do everything

real I.D. so that we are to get the command and I.D. So I'll see you in the next section.

Until then, bye bye.

Thank you.

