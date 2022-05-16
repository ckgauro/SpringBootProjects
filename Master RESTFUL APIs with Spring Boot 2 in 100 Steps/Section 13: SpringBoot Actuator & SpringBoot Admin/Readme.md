### Step 100. Step-01: Add Actuator Dependency in pom.xml.md
Welcome back.

In this lecture, we are going to understand and implement about Springboard Actuator, so Springbroot

Activator monitors and manages springboard applications using the rest or mix actuator endpoints.

So the endpoints offer health checks, metrics, monitoring access to logs, trade bumps, bumps, environmental

info and many more if you see on a high level.

So the following are the springboard actuator endpoints we can see here already being Scotians conditions.

So all these are all the latest Springwood actuator endpoints if you see here.

So these are additional endpoints for spring and we see spring the flux of Jersey.

So they'll have additional endpoints also available for us for the.

So these are the total actuator endpoints.

So we are going to look into in detail about most of the endpoints.

Primarily for us.

What matters here is about metrics and then monitoring.

So will focus on those things as the primary thing and also health.

So as usual, our implementation steps starts with our good brand creation and then they will add the

springboard actuator dependency problem that we refer to.

It then points, then we'll move on to exposing all the actual trend points, using the application

that property settings.

In addition, for the health endpoint, we're going to add additional properties here, then run the

info endpoint and then a better problem that is similar to building for plug ins so that we can see

that building from the info endpoint.

In addition, you'll also see if few other messages, whatever we define, within forbad labels.

So the same can be shown on the infrared endpoint.

So those things we are going to look in step four.

Finally, we're also going to look into the metrics endpoint.

So I'll see you in the next lecture, the implementation.

Until then, bye bye.

Thank you.


### Step 101. Step-02: Expose all Actuator Endpoints and discuss about them.md
Welcome back.

In this lecture, we are going to create a new brand and are the springboard actuator dependency in

our bombed-out example and verify the actual endpoints.

So let's see the detail steps in our RESCORED now.

So we have.

We're going to create the springboard actuator branch now and then we're going to add the dependancy

springboard starter actuator and then we're going to verify the end point using slash actuator.

And by default, only two endpoints will be available health and then in.

So we are going to look into those things and then we are also going to discuss about other endpoints

available and in documentation link whatever we have here.

So let's go back to what I know.

So we are in a good repository.

Get perspective.

No.

So let me create a new branch, so master and the last 12 Springbroot Swagga documentation all at the

same level with the commitment so and to create a branch and 13 Springwood actuator.

Right, so now 13, Springboard Atwater is checked out.

Let me go here and minimize this.

Go to the project and will open the that XML.

Right.

And we are going to add a springboard starter actuator that so let me copy the Springboard Starter Web.

And then.

Pasted here.

And so it does actuator that, so let me save it.

So currently my Amazon stop, OK, so I really don't need to restart.

Just if I started, that will suffice for me.

Right.

So I have added the springboard starter actually to dependancy.

So now I am starting my JVM so I can start using Springwood up of select disrespect to Java application

and Sylvanus Java application.

So I prefer to run it as Springwood app so that I get some color coding here, which I'll be happy in

looking them in the cancela like this.

OK, so.

Our applications started, so let's go back to the browser, so let's access the actual end point.

So we'll say localhost ADHD slash actuator, right?

So as we discussed earlier, we are going to see only two primary endpoints, one is health and the

other is in four.

So let's click on the health.

Right.

So it says that status is up.

So our job is up and it is saying that status is up.

So currently, health is showing only up.

So we have other parameters to add to see additional health information of our server.

So we'll see that later.

So the next is in full, right.

So from your perspective, currently we don't have anything.

So these are the two main points which we are going to see as part of the public endpoints.

OK.

And when we enable all the end points to be public, so we are setting whatever we are going to do now.

So with that, again, all endpoints will be public and we will be able to use them in real time production.

Well, it is not going to be that way, but currently for our exploration, we are going to do that.



Until then, bye bye.


### Step 102. Step-03: SpringBoot Admin Introduction.md
Welcome back.

In this lecture are going to understand and implement Springwood admin dependency.

So this is not provided by pubertal by default, but the corp centric.

There is one company who is providing this and it provides the monitoring features like visual, visually,

seeing all the actual metrics on you.

Right.

OK, so that's about all in all about the Springwood admin.

We'll see in detail.

So Springwood Admin Server is the application user for managing and monitoring Springwood applications.

So it is available as a package or we can even add our respective dependency on the project and then

started and then watch it, OK.

So in what ways are we can customize it to the level whatever we want by taking the dependencies and

then changing the stuff and by default is also available as to what we can deploy in our contacts.

Each application is considered as a client and registered to this Springwood admin server.

So currently we are building Springwood building blocks, application dates or whatever we have done

and then all these sections.

So that application is called the client application and that need to be registered with the Springwood

admin server.

So in the background, all the data are displayed on admin server is using the Springwood actuator and

points enabled on the client application.

So whatever the data we are going to see on this admin server, that is, we are trying to get that

data light from other applications, which is nothing but our client applications, nothing but our

microsurgeons application.

OK, and then we're going to display that is going to be displayed on this Pingle admin server.

So if you see here, it features the dashboard with the stop notifications, so if a game is down at

our respective Microsoft Office application is done, it can show that they stop notifications provided

if it is, if the browser is in the open state in Florida, one of the process.

OK, so the application will be able to use the application, help in finding details, feature using

actual trend points.

Whatever we have seen currently using the list endpoints in our previous lectures, write health info

so those things we can visually see them on the application, so we'll be able to configure a few metrics.

So the important point here is not everything we're going to see, only the light data so persistent.

Our Time series data will be available on Springbroot Admin Server, so we will be able to also use

the long term configuration.

The same will be able to manage log back logs also directly from the Springbroot admin server.

So in addition to notifications and then in addition to using the metrics data, we're also able to

manage the settings in our Springbroot applications using this to springboard admin server so we can

view and use the next Binswanger Eulogio.

So this is also possible and we can also use Reddam.

We can use to request a recess, which means whatever the request came, what is the content, what

is the response going and what is the content.

We can see all our lives only and we can history of registered application only.

We can see the history which is nothing but stop and start other applications.

That's nothing more than that.

OK, so end up in this overall Springwood admin's our perspective.

The top notch feature.

Whatever we see here is notifications.

So multiple types of notifications are available, assuming like the realtime environment, if we deploy

the Springbroot admin server.

So that may be recorded without spending money.

We want something opensource and then we want to monitor all of our applications.

So forget about the metrics and then forget about the health.

And then all those things are managing.

But what this can do, it can tell us our application updown situations and we can write custom code

to capture stuff like that at this point.

So I'm so captured and then all those things we can write and then we can finally the notification channel

so that we'll be able to get the notifications about our applications.

So if I see all all of the light monitoring and alerting solution without any persistent data, are

we can even say that time Cedar's data is not available, it doesn't store any data.

So whatever is coming from the spring actuators in principle display for us, that's all.

So Spring boot admin service notifications, we can see these many notification features are available.

As I said in my previous slide, you can see here, oh, notification is the top notch key feature.

Right?

So in the same year you can see here so we can define remaindered notification notifications made,

notifications page to be optioning notifications, slack notifications.

Let's let's check notifications, even the Microsoft PIMS finally telegram and even the Discard notifications.

So like these multiple things, MORALEZ it's like it like monitoring with notifications.

So that's above this spring boot admin server.

So the steps, what we're going to follow and then implement that will look into.

So we're going to build the best product, which means would have been several different product, which

means like it's not on our current building block server project, whatever we are building.

OK, so we're using spring initialized.

We're going to build a new project.

And in the project, what we're going to do is like we are going to select the spring, which started

as one of the dependancy, and then we'll go ahead and then.

In the project itself, Milada dependency related to admin server and then the stepped waterloo's primed

Springbroot client application, nothing but our building blocks application to the admin server and

posted the features in Springwood admin server.

So so we are going to see all the metrics and then all the details on the admin server, whatever is

coming with the actual end points.

So let's see the list of steps.

So we are going to implement this in totally three steps, right.

So when is this project set up?

And that is trying to the building blocks application to this admin server and then finally test it?

OK, so I'll see you in the next lecture by implementing the best project.

OK, so until then, bye bye.

Thank you.



### Step 103. Step-04: SpringBoot Admin - Base Setup.md
Welcome back.

In this lecture, we are going to build the springboard admin server based project now, so let's go

back and see the dependencies and what we are going to do.

So what we are going to do is we are going to create a new springboard project from Springwood initialised

and other social dependancy that's being built Administrator Server, which is coming from the Corb

Center.

So we are going to add it to that one.

That is the current latest version, which we are using as of today.

And we are going to annotate it would enable admin servers that Springbroot main application class and

we are going to change it, but also two nine zero zero because Arab Spring based client application

building blocks application is listening on AT&T and we are going to access the springboard admin server.

So in addition.

So for you to reference any time if you want.

Okay, so if if by any chance.

If you want to look for the documentation, so I have provided the link as it reference, right.

So now let's go back to the project.

Right.

So we have so far.

So we have Springboro Building Blocks project, so let me close these things so far.

No, we don't need.

OK, so we are going to create a new Springbroot project with the spring board initialised directly

from the city instead are going to start that spring.

That I will.

So I'll send you and then I'll Spring Start Starter Project.

And the project name I'm going to say is Spring Hardeman.

Right.

And group name is.

Stack simplify, right, and you're also going to give the package namers considered stack simplify

dot.

I mean, right, so the style looks good packaging, it's language is our version is Yade, so all this

looks good.

OK, so artifact name is Spring boot Typhon admin.

So let me click on next.

Right.

As I said earlier, I'm going to select the spring, but the starter.

OK, so let me also click on Finish.

Currently we are using two one six but find two one seven.

OK, so click on next and then finish seven years.

Springboard admin project is getting created so it will take a while to load the dependencies.

It's loaded already.

OK, so now what we are going to do here is we are going to copy our enable admin server.

Right.

So before doing that, we need to copy other.

Hopes and click Springboard Administrators', our dependency, right?

So let me copy this and go to the form that XML.

You are the dependency here, OK?

And it.

Good.

So let me.

Start the server.

Mostly a through the roadway because we didn't change the port.

OK, that's the thing.

So let me go to the application that properties and I will say sarva that port is equal to I'll say

this as a nine zero eight zero port.

OK, so that's good.

And one thing we need to do is also we need to annotate it with a direct enabled administrator.

Right.

So let's also do that with the MAINSPRING admin application that.

We're also annotating and telling that it is admin server.

So let me save it.

So let's start the spring springboard server now.

So it came online, so let's go back to our browser and then say local lost and instead of four eight

zero eight zero, we need to say nine zero eight zero.

Right.

So our springboard admin project is up and here are the details.

So we don't have any applications here.

So zero zero and nothing, no applications got registered here.

So let's see here.

We have completed our step one.

Now, in the next lecture, we will focus on pointing out Springbroot client application to this Springboard

admin server.



Until then, bye bye.

Thank you.


### Step 104. Step-05: Point SpringBoot Client Application to SpringBoot Admin Server.md
Welcome back.

In this lecture, we are going to point out Spring boot client application to the admin server so far as

our client application is nothing but just know we created this department is nothing but a springboard

building blocks.

So let me close other files related to the admin.

And now we are only in the building blocks project.

Okay, so he had admin is already running with nine zero eight zero.

So let me go back to our Vizquel steps.

And if we want to add our application right now to our means, like if you want to register our client

application to the admin server.

So we need to add springboard admin, start our client in our client server, OK, which is nothing

but client applications, product XML.

So it is nothing but springboard admin starter client.

OK, so let me copy this and go here and in our Springboard Building Blocks project in the form that

XML.

So let me make it bigger.

We are going to add this right.

So we are adding.

Springboard admin, starter client.

So let me save it.

So.

We need to stop and start because we have added the new dependency.

So let me stop this and again, started back springwater.

So it's back online, so the next step is to in the application that properties, we need to point our

application, right?

So the spring dot dot admin dot climbed you.

All right.

So we are going to point to the admin server.

So we need to add this.

The naming convention, I felt, is not right from proper perspective, but whatever they define, we

need to use, right.

So what it says is that would not admit that claimed that you are OK.

Really, we are telling clients this is that manual.

But whatever it is given here is claimed that you had it.

OK, so that's the thing.

So but that's fine.

Okay, so whatever they have given as per the documentation we need to follow.

So spring that would that I'd be not lying to you.

And here we need to give our admin server your order.

It is nothing but nine zero eight zero.

So I say point to admin server.

Right.

And then let me save this.

OK, so we also need to ensure that all over again.

Points out in open state include star.

OK, so they are accessible.

Right.

So let me see star light management and point that the exposure.

I said star and then I have saved it.

So let me come back here.

So one important point here is it also supports Springwood, Cloud, Discovery and claim dependency

also available here.

So how we have your administrator client for the cloud Biscardi also we have the excellent client and

then for all the micro services or whatever we are going to create with the Springwood Cloud.

So all those also can be registered with the Springboard admin server and then manager via Springbroot

Admin.

Right.

So that's another thing.

So now let's go back and then see our instances and then after that are the tags for that.

OK, so let's go back to browser so we can see it here in the 1980s and then applications, we can see

that one application is registered.

Right.

So our current application.

So let me click on this.

So here I don't see any tag here, OK?

It's like name of this application I'm not seeing.

So I have two options to add the tag.

One is use the metadata or use the inflection point.

So what I do is I like the metadata.

OK, so let me copy this and then go to the properties.

And then.

And that metadata, right?

So let me save it.

So let's go back here so you can see environment.

I got there immediately as soon as I added the bag.

Right.

So that looks good.

So let me click on this environment and then go inside.

So let's start exploring the environment now.

So in this lecture, so far, what we have done is we have pointed our Springburn Building Blocks project

using this respect to dependency to the admin server.

Right.

And then we also updated the application that properties with spring that butat admin that claim that

morale to our admins are very real and ensure that all of a sudden stahmann, which means all our endpoints

are accessible so that we can see each feature on the admin.

OK, so only if you run poorly informed then a few specific things.

We can only annable those things, but as far as we are demonstrating it, we are going to see everything

and to have the tax information for our applications of real Saradha tax.

So in the next lecture we're going to focus on testing all the things, whatever from endpoint perspective

on the admin UI and then see all those things.



Until then, bye bye.

Thank you.


### Step 105. Step-06: Test the features in SpringBoot Admin Server.md
Welcome back.

In this lecture, we are going to test the features in what's being administered, what we are going

to verify our features.

So let's either step in our yasko.

So we are going to see the health and point in point biometrics and point in history.

Bootlaces, everything OK?

So let me go back to our browser.

Right.

So if you see the inserts in the details, so this year it primarily populates the Healthpoint so and

influent points.

So from Hilton point after enabling that thing, whatever details of health, we got the baby information,

nothing the database has to.

And we also got the disk information right.

So 251 Dibia Inventory's 119 GB in the same way.

We also got the instances up.

So these are the health endpoint details coming from the actuator endpoint mnemba health.

These are the important point in the information point we have built.

One is big information and the other is that right?

So we created hello.

We have provided these properties in our application that properties.

So those things we are at least seeing them here.

So now influent health completed.

So we'll have additional metadata and then process information here and also towards information and

the memory and then keep all this information will be available in the detail section.

So let's move on to the metrics area so we can configure all the metrics, whatever is required for

us using this option.

OK.

Reconnections, Aquatica, reconnections active.

And if you see here, I have the GBM threads.

Lipe So it is showing 13, OK.

So if I run some loops here, I can see more here.

So like that process files open 126 currently just now we have seen 125.

So like that we can get a lot of information here.

And the next is.

Environment, right?

So but metrics you are able to see here, right?

Other than that, nothing, which means you are going to see some information, but there is no graphing.

There is no or what we call OK.

Clearly seeing and we are only seeing the lack of information.

The reason I'm trying to point out these things is in the next lecture we are going to look into micrometer

and micrometer integration with genomics and micrometer integration with one more application.

Nimda acrobatics, OK.

So in the app optics, also, what we are going to do here is.

We are going to.

Captured the metrics on our application and then send it to our publics and then create the dashboards

there.

OK, so all those things we are going to see, I'm trying to show the downside of multiple areas.

So I got the metrics, information, but how much I can see that means nothing.

All these are no metrics.

OK, so what can I do?

Only I can see only like metric which is consistently changing.

So that's what.

OK, so in from environment perspective.

So we get the environment information here.

That's good.

OK, and here we can see the base information.

So this is nothing.

But you write off that the services are for actual points and these are configuration properties which

we are able to see here, whatever we have.

Right.

So config properties then try and try to see all those details so we can see here we can see there's

two console pathways to information, all those things.

So we don't have any scalable tasks or task and is empty.

So next, moving on to the logger's.

So as I said earlier, will be able to handle about logger's with whatever the things we want, which

means we can enable in for debug tracing.

This is one good feature, which means like we can manage.

So managing our application features like logging and all those things, we are good feature.

So it is like good for managing and not good for Matrix.

So something like that.

Yes.

I'm not saying it is good or bad, but what I'm trying to say is like in some areas it is excelling

and then in some areas it is not excelling.

So these are the laggards.

And then we'll be able to handle like we continue to debug and then we continue to run from here itself.

And the next is JVM.

So from the union perspective, Jim X-Rite, so all the beans and beans will be able to manage year

and then edit and then change the details and then edit and then manage them here.

So that's again, one excellent feature, which means we'll be able to handle all the configuration

changes here.

Right.

So this is like trade monitoring and what he will be able to download our dump.

Right.

And this is trade monitoring.

Now, let's go to the is nothing will detainable anything.

So we are not getting anything.

And from audit logs, we didn't enable anything.

So we are not getting anything currently.

But if we have something in our application, auditing is enabled, we are going to get it here.

Let's go to the web now and see the mapping earlier in our endpoint.

Also, we have seen the mappings there.

So in addition to all our applications.

Right.

Hello.

Hello.

You need user user arioli orders.

You can see all the endpoints present in my application.

We are getting it here.

Right.

So if you see this many points we have built so far.

Okay, so that's good.

So all these things we are seeing here.

So now let's come to the history to be tracer's right.

So here, whatever the like requests the request and response we can see, OK, how we're going to do

that is we have something called in our Posman.

So in Posman, I said that some project name I can rename this right.

So I can say springboard

building blocks monitor.

OK, so monitor is nothing that I'm going to download best.

So that's the reason I made the Nimetz monitor and I hope for three requests.

Year one is that our users get all our orders for one zero one user and get usability right.

And what can I do from postmodernists?

I can click on this, add a link here.

Right.

Or so whatever you are seeing.

So let me make it a little bigger.

Yeah.

So this add a link and I can see are right.

This is Control Kaneda Posman.

So if I click on this one, it opens the collection to Nazeri Collection Drowner.

So this collection, what we are going to do is we can run any number of iterations of these requests.

OK, so I can say I can run 400, OK, and when I'm running it, so the details will be displayed here.

So I'm sending the request.

Hundred requests now.

So run Springboard.

So let me come here.

See you are seeing the request coming here, right.

So users, users orders and then everything you are seeing here.

Right.

So if one zero one I can see the information here.

Right.

So this is a wopat has to assess what we are able to capture from our application.

So, OK, so ideally it's not request response, but basically Petreus details.

OK, so what is what method get postman host connection means like request headers and then response

headers it is capturing here.

So that's about this.

OK, so and this is only line which means like once the requests are completed that's all done.

So other requests are coming.

Only when the requests are running we'll be able to lively watch.

But if for example, I can see if our users are something right.

So we can capture those things and then see it.

But how many?

OK, so there is one third of the 150 limites thousand we can even in.

It is OK, but all in all, everything is life, there is no persistent part time series data, so that's

about this.

So we have gone through all the features available in Springwood admin server from inside slugger's

the left navigation perspective.

Right.

So one more is wallboard, right?

There's nothing but it's being built.

Application will come here back.

OK, and another is applications, which we have seen here.

And then when there finally it is the German journal.

OK, so there is nothing.

But this is the place where we are going to track the history of our application.

OK, so our application registration updating for changed.

OK, whatever happens it will do that, ok.

And it also provides the desktop notification.

So let me go back to my idea and let me stop my Springwood building blocks application.

OK, so I'll go here and then this is the application.

Right.

Let me stop it.

OK, so ideally I should get their desktop notification, so we'll get to it shortly.

Oh yeah.

It's Topsy Springbroot application is now offline.

Alright, so let me go there and you can see the application is offline.

Instances are down in the journal so you can see our application status changed offline.

So this is nothing but the history of our application tracking whatever it is.

Yes, OK, but here I don't see how we are going to manage it if 10, 20 applications are there and

then it's the I so we can see.

But there is no tracking of searching and then finding it.

What is its current status are in by instance, are by application, are by time, are by then.

We don't see all those things here.

OK, so let me also start back our application.

OK, so likely that ah so it's a good feature but it's evolving.

Furneaux ok so and for small scale and then small business will be able to use it for monitoring Guevarra

based Springboard applications.

And then in addition to that, if you have multiple instances and then if you want to change the configuration

to do something, and those are also only limited from their mix perspective, from logging perspective,

you'll be able to change those.

And all in all, it is restricted to actual primally.

So if I see here, we have completed our testing, but even including there has to be Trace's.

So this completes our two sections, which we have focused.

One is actually third base and also the spring boot admin server.

So in the next lecture or in the next section completely, we are going to focus on Springwater, Micrometer

and Actuator in that combination, how we are going to do it.

So as we have completed all these things, let's go and then complete our final step.

Nothing but commute and passcode via I.D. So let's go back here.

And did we make any changes?

No.

Right.

Any additional changes?

No.

So I'll say our application and that axman, only two files.

And the other section of what we discussed is the actuator and then admin server.

Right.

Actuator.

Admin server first come into light, so let me comment and then push this, OK?

And it is going to create 13 springboard actuator in our.

Mod GitHub server, OK, so let me click on next and click on Finish.

Good.

So this concludes the check in process, so now I'll see you in the next lecture and then bye bye.

Thank you.


### Step 106. Step-00: SpringBoot Actuator Introduction.md

Welcome back.

In this lecture, we are going to understand and implement Springboard Micrometer, so Micrometer is

the Matrix collection facility, including Spring Bapu's actuator.

Micrometer is a dimensional first matrix collection facher, whose aim is to allow us to time current

and gods, our corporate vendor neutral API.

So to talk more about this vendor neutral API.

So this micrometer will be able to integrate with any type of monitoring application.

So it's not that we'll be able to integrate with one or two monitoring applications, will see the list

of monitoring applications.

We'll be able to integrate and push.

All of our metrics are generated by the Springbroot application and that's a very good feature.

Both men slept through class, but in consideration, we can just select one of several monitoring systems

to export other metrics data so we can even send to one or even multiple metric end points so we can

send for all of them, which means like a dinosaur race or a class, or if we have multiple monitoring

systems, we will be able to send the metrics to all of them.

So how many of you configure that much?

So next year?

It is again simple.

Just one config file and then one property file, one or two properties, and then we'll be able to

make the changes.

And additionally, it also has been back to older versions of Spring one, that 504 and then one that

triggered the addition of another dependancy.

So it's not the micrometer dependency, but we have a different micrometer, additional dependency available

for porting back to older versions.

Yes, Cindy micrometer timer is capable of producing time series related to property total time, maximum

latency of recent samples, pre computed percentiles, percentile histograms and SLA boundary.

So all these things, OK, are a lot of features will be able to see using this micrometer time as OK.

And we are going to see a few things in real time.

We're going to integrate this micrometer with our A game console, which will be available in our local

servers.

And also we're going to create one more trial account on solariums, APAP pixel product, and then we're

going to push this matrix and also see those.

And then we're going to generate some dashboards.

And then in the dashboard, we are going to generate a few graphs and then also view them.

So we'll see all those things in our upcoming lectures, but that the change to the micrometer, the

result of a desire to better serve a game of dimensional monitoring systems.

This these lines have Buckett from springboards, documentation about the importance of this micrometer

and then how we are going to use it.

OK, so it's like I felt when I'm explaining about it, like I'm very happy.

So to know that, OK, we have one feature named Micrometer which can collect the Matrix and then push

to multiple sources for monitoring applications.

So pick your choice.

There are almost like 15 to 18 months of products available and for any of the monitoring product,

I'll be able to send the data.

So which means our possibilities rate increased, which from springwater perspective.

So when we are building the service and springboard so we can say that from Matrix perspective, I am

happy.

Well, what is your monitoring tool or this one Springwood supports so all major providers.

It has maximum support for maximum monitoring tools.

So let's see what all those Spring boot enabling us to choose one.

That's what I'm saying.

You're saying the same thing here.

Springboard is enabling us to choose one or more monitoring system to use today and change our mind

later as our needs change without requiring it.

Levator for custom metrics, instrumentation.

So this is the documentation you have put out here for your reference micrometer that I was Nasdaq's

so.

If time permits, you can even go through those things whenever required, so monitoring systems supported

by.

Micrometer all these things, so if you see here, haptics in blue, jambox in blue and simple in memory,

Bakary back and used as fall-back option.

So these things we are going to look into in our next lecture's, but it also supports a class about

by with elastic canula.

Graphite Homeo inflects in STONA careers may be neurally and Prometheus signal effects start the engine

for your friend.

So it's a good amount of tools it supports.

And it's not that it only supports on premise.

Data is like a it's an SAS solution.

Dominatrices solution elastically supporting US local right and humoral graphite is a solution as far

as I'm aware.

OK, so new remixer solutions.

Tincknell effects solution, wavefront solution.

So like this, it also supports the solutions, which means it will be able to push the metrics to the

source solutions also.

So that's about the beauty of implementation, about the micrometer.

So if we go for the implementation steps, as usual, we are going to create our standard grandiflora

micrometer, an actual implementation, and we are going to add a micrometer dependancy for metrics

and metrics using simple in-memory back and look, which is nothing but just the metrics point.

So metrics and point currently, whatever is their access, the default in memory back and so that we

are able to see the metrics.

So we run the test and then keep watching them and then see that OK, and integrate the same mix and

view metrics in the concern so they can solve nothing.

But as part of a dedicated chipset, will open the concert and can see in the next area in the area

one specific one, which is nothing but metrics folder and delmonte, all the all the metrics are available

deadman's like all metrics are available there and then within the traffic, both keeps changing.

So we are monitoring that mix.

But these things are monitoring, right.

We don't have any persistent data.

So that's the reason.

I also want to demonstrate one more brewskis where we see the persistent things like our data is Parchester

there?

And then we'll be able to generate the graphs and all those things for that purpose.

What I've done is like I have integrated it with our expert metrics and view metrics in other popchips,

which is nothing better.

So Ludwigs product so.

We'll go ahead and implement all these steps, so they'll perform the steps using postmen collection

and finally will come and then push the caller I.D. so to see the steps from the school perspective.

So here are these steps to bring you back to.

Then micrometer implementation will create our Springboard Actuator Micrometer branch and will implement

two, three and then four.

What we discuss are just not all the steps we are going to implement step by step now.



Until then, bye bye.

Thank you.

