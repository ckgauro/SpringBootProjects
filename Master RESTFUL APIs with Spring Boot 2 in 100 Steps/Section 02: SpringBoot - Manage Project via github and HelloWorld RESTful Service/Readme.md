### Step 4. Step-00: Best way to quickly complete this course.md
### Step 5. Step-00: Github & HelloWorld Introduction.md

Welcome back in this section, we are going to understand and then implement a simple high level dress

service.

So in addition, we are going to manage our entire course project where GitHub.

So we are going to do all the best GitHub setups here in this respect to S. So to see the implementation

steps for the same thing.

So we will start with creating a simple springboard based project by generating the project using Startup

Spring that I will we will go ahead and then understand the basic GitHub concepts required for managing

our Springbroot projects.

OK, well get up.

So we'll do the GitHub based setup and then move on to adding that repository to the spring pool.

So tidy in the get perspective.

So we'll go ahead and then I'll build a simple hello worldclass from April to latency string.

So in the step for when we are building the data repository and then initializing it, we will ensure

that for the rest.

Filipe, we have a separate branch in the GitHub, so both in our local get repo and also in the GitHub

remote repo.

So then we move on to creating another simple hello world service, which latency, which is nothing

but this and response and then finally will go ahead and then get commit and then push for this Haulover

service so we can it in the local and also post the same thing to other remote git repository so that

we have the branches in local and also in the remote.

So this completes the basic implementation of Amidror.

Set ups and also the Bucella wrote a stable introduction, so in the next lecture will go ahead and

implement all those things and see in the next lecture and then bye bye.

Thank you.



### Step 6. Step-01: Create Spring Boot base project from start.spring.io.md
Welcome back.

In this lecture, we are going to create a simple springboard project with requite dependencies.

So we are going to go to Starbucks, bring the table and then generate our product using that and then

import it to eclipse.

So we are going to use the dependancy, says Springboard Starter Web Springwood, dev tools, spring

data dippie and then head to database.

So we are going to use Springboard Starter for building our web services.

The same can be used for building the web applications using spring.

So we are also going to use springboard dev tools.

So which will be helpful during our development process to exclude the steps of compile and run.

And then as soon as we make any changes to our code and if we save the project, save the respect to

find those changes will be artillery to the day we are embedded tomcat immediately.

So for that purpose, Springbroot, the tools helps us a lot and the spring data J-P and to database

these we are going to use at the later part of the course.

Initially we are going to use the static least to implement the things and then get all the building

blocks of Springboard together.

And then once everything the whole project is ready, then we are going to convert that to project using

spring data dippie and then in-memory database Haeju.

So.

Once we create the project, we are going to verify the dependencies in our palm, that XML.

So how this has been populated there and then we are going to just run the app and see that if everything

comes up properly.

So in this lecture, we are going to do these things.

So let's go ahead and then do those now.

So we are in the Starbucks spring that I will, and the project we selected is the Mavin Project.

So we are going to do this using Mavin and the language we are selecting is Java.

And the springboard version we are taking it is a test that is not one, not six.

And the Project Medidata, in that the group we are going to give is.

Kamdar stuc.

Simplified, not less services.

OK, and the artifact, so which is.

Springboard

building blocks, nothing, whatever project name, right, Springwood building blocks, and if you

seen the options, the package name got extended to here, which is after the services, it also took

the Springwood building blocks.

So we'll remove that.

So we'll use the package names, comp, not stacks, amplified up rest services in the packaging.

We are going to use this Java and the Java we are using is Yate and the dependent's is now comes to

the dependency section.

So if you see we are going to use the springboard starter web, so spring the starter.

So which helps us to build web, including zestful applications using spring, MVC uses a party tomcat

as the default and butter container.

So we are going to select this and the other one is dev tools.

OK, so Springwood Dolittle's.

So if you see it Proops Springbroot 2 restart lively load and configurations for enhancer parliament

experience.

So we are going to select this.

So other two which we are going to select our spring data --.

So if we see here.

Yeah.

So this is the spring data J-P, so let's select that in the same.

We will also select.

Hedge to suggest a database.

In addition, we are going to look into Springbroot Actuator and then Spring Hayatou is all these things

in the later part of the course, those details we will add as and when required.

OK, so far now we'll start with Spring Web Startup Spring, beautiful spring day to appear and then

has to database.

So let's clarify all those things one more time before clicking on the gender project.

So if you see here we are in the Startup Spring that we have selected the project as Mammone project

language as Java and springboard us to that one.

That's current latest version.

So we are not using any snapshot versions.

We just using the stable version 2.0 and six and the project data we have given the group has come that

stack simplified out the services, which is going to be our package name and the artifact is Spring

Woodhaven Building Blocks.

So in addition to if you see the dependencies, we have selected Web start tools that are dippie HESTA

database.

So let's go ahead and then click on the gender project.

So our project got generated.

We have seen the success message here and it got downloaded.

So we need to copy this project to the location where we want our all projects to be maintained so that

there we can unzip it and then in particular Eclipse.

So let us copy that.

So I it to my course projects folder, so Springwood building blocks that zip.

So what I'm going to do is I'm going to unzip it.

So using the Arko utility.

OK.

So now my project is unzipped here.

We can see it here, Springwood building blocks and we have got the project.

So we'll copy this location and then we'll import it to our eclipse.

Where Eclipse.

OK, so let's do that.

No.

So we are in the eclipse now, so let's click on file.

And then click on import.

So in import, let's search further, Merwyn.

So here is the moment.

So I will say that existing Mavin products.

OK, select the existing Mavin products, click on next and we can directly browse from here.

Our copy, our.

But so it is nothing but in quotes, projects, we have the.

Project, OK, so it is Springbroot building blocks so I can click on Browse so that it will get populated

here, so it is here, we can see it here, we can click on Open.

So now my problem that XML got referenced here so we can finish.

So now the eclipse is trying to impose the Manhattan Project, OK, and it will also resolve all the

dependencies, download all the dependencies, and it will take a while for doing that.

OK, so let's have it completed now.

So all the dependencies got downloaded so we can see it here, so we can see our main application file,

Springwood Building Blocks, application DOT Java.

So this is our main application file and it looks good now.

So we can see it here in the source main Java.

We'll have all our packages and then it's equal.

And the.

And in the swordsmen, resources will have a static files, templates and our application dot properties

so we can see the bomb that assembled here.

So if you open the Pontotoc symbol.

We can see all our details here, Kamaraj Tax Simplified Outlet Services, our group and over at the

factory and our product name, Springwood Building Blocks.

And if you see the dependencies here, you can see springboard starter, the data dippie starter web

and also spring the tools in the same way.

We also have a little history database.

So Springboro started this will be automatically loaded.

So we also got that one.

So these are the dependencies we have currently Navarra, Baumgart XML.

So let's go ahead and then start once and then see that it started properly so in Sydney's Springboard

app.

And they'll say, OK, fine, so we didn't make any changes, but that's the thing.

So if you see here, our company got started and we don't have any issues.

So if you started putting the building blocks application here and we see that very clearly, so this

completes the first step, which we are looking in.

So we have created our project.

We have selected our dependencies.

We have verified our dependencies in the form that XML.

And also we went and then also started the Springwood app and then verified if it comes up properly

or not.

So this completes our disturber.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 7. Step-02: Introduction for managing Spring Boot projects via github.md
Welcome back.

In this lecture, we are going to understand about managing multiple projects via GitHub get repositories.

So the main idea of doing this is like so for every major step we implement in our code, we are going

to create a new brand example.

Now we have the basic set up ready.

I like that, which is nothing better.

Whatever we have imported, we can consider it as a zero one ground zero branch.

Right.

So now let's go ahead and then check out two zero two for whatever the changes we are going to do.

So ground zero is like whatever.

We have imported the best product.

So now we are going to take out Copel movement from master example.

Now I'm going to implement double get mapping.

So for doing the get mapping and select that zero to hyphen that mapping as my branch and then I'll

go ahead and then implement the changes related to that mapping in my respect to controller and respect

to model all those things.

So once a complete yes, I'm going to come back to that respect to zero to date mapping local branch

and then I'm going to put the same code to the remote branch in the GitHub and then I'm going to check

out the master and merge those changes from disrespectable zero two or get mapping branch to the master.

So that completes that.

I have created a new branch.

I have completed my development there and I have checked in the code to my local and remote branches.

And then I have the code with my master.

And once I match the code to my local master, I'm going to push the master also to the remote repository.

So now I have two applications to it.

If I go ahead and then open the zero one Ground Zero branch, if I check out this branch, it will be

a base project.

And whatever I said here, like for example, we took zero to get mapping and if I check out this plant,

I have to get mapping changes here.

So it's like an incremental we are building our entire springwater application means like applying all

the building blocks in an incremental manner.

So what that will give us is like up from learning perspective.

So first thing what we get, it is like we'll go to the GitHub and check out our project.

Right.

So as soon as you check out the spring board building blocks project, so you'll get all the respective

repositories in your local right or you can clone that were just to on GitHub repository and then you

can clone it to a local.

So in all those ways, you'll get all the branches with you.

So it's incremental map understanding the are understanding and then going through the entire code base

so that your job offer for every step of the code and then import it or GitHub, you need to for every

step you need to unzip your code, download it imported to the eclipse.

So all these things comes into the picture.

And instead of learning, there will be a lot of homework we'll be doing there.

Lot of work which is not useful for us.

But in this manner, learning will be fast and you can change to the states at any point at our convenience.

So that is the thing.

And another thing is at the same time, in the real development world, how we are going to manage the

branches and then how we are going to push the code.

So in addition to learning pinboard, we are also learning that managing the.

Special projects where GitHub repositories, so both hand in hand will happen for us when we are executing

these things.

So basically now what we are going to do is so we are going to do a best set of steps.

So what is that is we are going to create a project in the GitHub repository.

Right.

And we are not going to initialize that project.

We are going to just create a simple project there.

And then we'll go to our local repository, local project location where it is there.

And then we are going to initiate the local repository and then we are going to create Masterbrand and

then check in Cordier and then we will add Gitter remote Autogen.

So this is nothing, but we are going to get the original from GitHub and then add that for our local

REPL so that we know that a.

For remote branches that respect to GitHub repository, and we are going to push the code to that remote

branch.

So this completes our masterbrand setup.

So now my masterbrand is with the spring base project, what we have created.

So now what is our next step is like same.

Our Masterbrand is nothing but a base project, but then we keep on incrementally increasing.

We are going to start with the master, right?

So to ensure that we have our base Ground Zero project, whatever the base spring project we imported.

So what we are going to do is we are going to create a zero one ground zero branch, so we'll create

zero one Ground Zero branch and we are going to push the remote branch up there to zero on ground zero.

So now we'll have zero on ground zero in local and then we'll also have the same in our remote repository

and then at the same time.

In addition to doing all these things in command line, sometimes we fail to use I.D., which is flexible

for us, like you can see that view and then get perspectives.

So they'll go to the get perspective and then add this respect to local repository there.

And then in some places, like instead of every time doing well, come on line by following these steps,

geocode go to new branch and then make changes and then commit, go to local branch.

Sometimes you come online, sometimes civilians get Eyedea Estacada so that what happens is like, OK,

we get the hand in hand experience for both things right.

So let's go ahead and then implement these things.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 8. Step-03: Github Base Setup.md
Welcome back.

In the previous lecture, we have discussed about how we are going to manage Springwood projects where

GetUp!

And then in this lecture we are going to go ahead and do the best set up, implement the best set of

steps required for getting the our GitHub remote repository and our GitHub local repository and our

idea to the Bay State where we can start using furtherer doing Allura document.

So let's go ahead and do that now.

So we are going to do the best set up steps now.

So the primary thing there is to create a project on the GitHub, OK?

So if you see it here, this is our GitHub repository model, which I'm going to use GitHub dot com

slash stack simplify.

So we are going to go there and then create a branch for the spring, the building blocks application.

So let's go ahead and do that.

Welcome back.

We are in the GitHub Dotcom's to simplify repository area, so we have only one repository here.

So this completer GitHub account will be managed only for the production level code, which to simplify

is going to create on the courses.

So this is created for the Codes for Dabblers Code Commit Code Bellecourt JPA pipeline so far

that we have created.

So now we are going to create one more repository now, which is for Springwood building blocks.

So there will not be any other repositories in this stack.

Simplify account only.

We will have the production code level code, which is nothing.

But whatever is used in the code is only those repositories will be there so that any time any student

want to reference from codes to that respect to the repository, that becomes easy for him to understand

and then implement.

So let's go ahead and then create the new repository.

So we have done so in the stack, simplify the repository, we are going to give it a springboard building

blocks, right?

So it's a description is like we are going to land springwater fundamental.

We are going to land springboard all building blocks as part of this course.

So that is something.

And we are going to publish it as a public repository.

And we are going to skip this step because we are not going to initialize this repository here.

We are going to the what we call import the project.

We are going to push the project from our local repository to here.

So that's the reason we are going to not check this respectable option.

So I'm going to click on Create Repository.

So now how created the repository and here is the link for connecting to this site, which is nothing

but getups tax simplified sublingual papen building blocks that get so no will go to four more on to

the next step.

OK, so let's go back and see.

Now we are going to go to our local repository and then initiate the local repository and create our

master branch and then check in the code and I get to report.

I get a remote origin, which is nothing.

But whatever we have got just now here, see, we have got this here.

This is nothing but a remote origin.

Yoran So this year we are going to point there and then we are going to pull the code to the remote

branch and then we are going to also verify in remote branch.

OK, so it is a time taking process.

But once we understand these fundamentals from get perspective or you are going to benefit a lot when

doing the course are when you are doing the development from you're from from your origination perspective.

So all becomes easy for you.

So let's go ahead and then perform these steps.

OK, so so we are in the terminal also.

If it is in windows, we'll have the get bash.

So if we download the data from jizya, so what we'll get is we'll get the get Basche terminal.

In addition to that, we can do that via Vrsaljko terminal.

Also using power in windows are here also become where we ask Yasko terminal.

But from my perspective, I prefer using the Mac terminal directly here.

And so if you see here, if I click on Present Working Directory, I am in my coach project, Springwood

Building Blocks Project.

If I say unless I can see all my project details here, I listed all the files here, so I'll say it

clear.

And now I'm going to initialize this folder.

Springboard building blocks, disrespect to folder as it gets repository.

So I said get in it.

OK, so it initialized the project.

So if I say get status right.

So Node says that on Bandmaster more coming.

See it.

So which means we still didn't add any comments and these files are in the track instead.

So these are not attracted by the git repository.

So we can go ahead and then track these files.

So add to the tracklist so we'll get our space dot.

So then we are saying get ad space.

Dot dot is nothing, but all the files need to be added to the tracking.

So then all these files will be added.

So currently you are seeing in red color these things.

Now if I say the word status, all will be the green color, which means they are tracking more.

So now what we need to do is now we have staged them, right.

So now we need to come with them.

OK, so now what I'll do is get comit minus here.

So I'll see first.

Come it right.

So now what happens is like all these files got committed so you can see your ten files changed, 681

insertions and all these files were checked into the Daytripper.

So let me do the clear and then now we'll get status.

So on branch master, nothing to commit and then working two clean.

So which means now we have successfully completed the masterbrand chicken.

OK, take enough code.

So now we have now we need to add the original.

So let's add the origin.

So remote get remote origin will be the come in.

And let's go back to our gate report.

Here is the thing.

And then copied and pasted.

Right.

So now we are going to add the origin.

So now we have completed adding our origin, which is nothing but our remote gate reporting the GitHub.

So now we have the remote Blantyre so we can directly, Siddharta, get pushed minus U and then origin

and then provide a master.

So what this does is like every time, you know, to get the push and then again origin and then mastered

all the details you need to give if you use this command.

OK, but if you use a different command, so what happens is like a set up stream will be there is one

more command so that always whenever you do just get push from disrespectable or master from the respective

branch, then automatically that changes will go into that branch.

OK, instead of writing a big command, once you set the upstream automatically, you just need to you

just get push from that respect to branch and then it will take it.

So let's do that.

OK.

So let's add this now.

OK, so gate

get push.

Up upstream.

How did you master so what this do is like.

From next time onwards, we don't need to provide a good push username and an origin and then master

all these details, we don't need to provide it.

If you just said get Bush then automatically from this master branch to local master blaster master,

but the genius will be pushed are sinked.

So now for the first time, it will ask for that username.

So I'll see stac simplify and the password.

So now my question is successful and then it pushier the brand, we can see it here to Springwood building

blocks get new blood master to master, a master set up to track the plant master from Origin.

OK, so now we can go to our GitHub and then see the source and then bombard Zemel, all the files on

the GitHub.

Let's go ahead and then do that.

Not so.

We are on the GitHub now, so let me click on Stack Simplify and we have the project here, Springwood

Building Blocks and we can see here all our first coming details has been checked in and currently we

have only Masterbrand.

So now we are going to create one more Blandino in our local, which is not a zero one Ground Zero project.

OK, so we are going to do that now, so let's go ahead and do that.

So let's say get status.

So now we are on Bandmaster Mostert.

So check out minus B, ok, hyphen B, hyphen B will give us to just check out and then other branch

name will check out to that branch.

OK.

But if you see say hyphen B, it is going to create a new branch for science here zero one.

And then I can say.

Ground zero, so it is nothing but ground zero base, I can see.

OK, so this is my branch in here.

OK, so now I switched to a new branch named Ground Zero.

If I see, I get status.

So you can see that we are on Branch zero one ground zero base.

So what we are going to do is here also for Ground Zero branch.

Also, we are going to set up the get Bush set up upstream origin master.

And we are not going to change any changes to this.

OK, but just as a standard, whenever we create a new branch, we'll try to setup's upstream to respect

to branch on the remote repository so that it becomes a habit for us.

OK, so I'll say get push.

Third upstream origin, and then I need to provide the.

Branch name.

Right.

So this is my branch name.

OK, and then I click on Enter.

So no disrespect to Branch Zero on Ground Zero base will be created in remote repository and also will

be in sync.

So brand zero on ground zero base set up to track remote brand zero on ground zero based from Origin.

So now we'll go back to our GitHub and then see the same.

So now we are here.

So let's go here to springboard building blocks.

And if you see here, we have the zero one ground zero base.

So we have the master and zero on ground zero base.

So this completes like whatever we want to create from the branches perspective and then set up our

GitHub account and then local GitHub repositories, all these things.

So we'll have completed our three three B, Part B set up steps, which is create a project on GitHub

and then create a master branch and then perform all the changes here and then also create a zero one

ground zero based branch.

OK, so we also created that respective base branch, OK.

So in the next lecture, we'll focus on adding that report to the outside.

OK, so that will be able to manage the same thing where I.

So I'll see you in the next letter and then bye bye.

Thank you.


### Step 9. Step04: Add GIT Repository to Spring Tool Suite IDE.md
Welcome back.

In this lecture, we are going to add this respectfulness repository, which we have created for this

project in our society so that we can view it from our perspective or we can manage it from our perspective.

And ideas are even we can check in the court files everything.

We're good staging view.

So let's go back to our personal history.

So we are in our era, you know, let me stop this come down.

And if you see here in the.

Window in the prospectus.

OK, so see other OK, and then we can see it here, the get perspective.

Right.

So now we are also opening the gate perspective.

Right.

So this is the get perspective so we can click on this option, which is nothing but add an existing

local git repository to this view.

OK, and then copy our directory here and then browse that, OK.

So my project directly is at this location.

I'll click on Browse.

So this is my project directly through Springwood building blocks.

OK, so I'll click on Open, right.

And then I'll select that thing.

OK, so now I'll click add.

Right.

So now my good repository is added here so you can see zero one ground zero base.

Right.

So if you go here.

So in the branches, if you see local you can see master and then ground zero.

Both has the same code here, nine E to SC.

So which means both has the same level of code currently.

And if you see here in the remote tracking also you can see two branches, OK.

So Origin Master and then Origin zero one ground zero base.

So we have two branches here also.

So which confirms that yeah, this everything is good from good repositories perspective and it's decided.

So now we can go here.

And then in addition to that, what we are going to do here is so one thing.

OK, so we'll also see the sure view and then we topin don't get staging.

OK.

So.

Let me see where it is.

OK, so it's not in the perspectives, so it should be in the short view.

OK, so let's say other and then I'll say good staging.

Right.

So this is like whenever that change happens in the staging of you, those changes will be displayed

and then we can take in the quote directly from here also.

So let me make it bigger.

So let me go to Springboard to shoot here.

And we are in the we are in the zero on ground zero base.

OK, right.

So if I say just if I see some command lines two and then see automatically, you can see it's unstaged

here so we can drag it here and then see the second comit.

Right.

And then we can say comit and push.

So that same changes will be pushed to both our local and then remote repositories.

OK, so I'll take it and then push.

OK, so far my stack simplify details for my idea.

Also it needs the credentials.

So I am saying stac simplify tax simplify and then I'll say password.

OK.

So is your surname, and I'll say Thida and pointis you are.

Squalene.

I'll see school one.

OK, so just.

OK, so now you can see how did I push you to Springwood building blocks, to our remote repository

to so I where this could get changed.

Let's see.

So now go to get and if you see here, the master has nine years to fight this year.

And here you can see so on YouTube seven to be able to see him in that remote also so we can even see

the come on our I respect all branches.

OK, here.

So let's go here.

And then we can see we have two branches.

OK, so master.

And then.

What we call a default brand is master, and it has updated 31 minutes ago, but our zero one ground

zero, this updated one minute ago.

So we can see that changes here, that we have a new 10 years to this respect to branch.

OK, so that's about the setting up of our new.

Project the.

Related intel, GitHub set up, so now we have all the GitHub things.

Set up for our project, now we can move on to our core project, which is nothing but a springboard

building blocks.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.


### Step 10. Step05: Create a Simple Hello World RESTful Service which returns a String.md
Welcome back.

In this lecture, we are going to work on Hollowell, the service, we are going to build a simple hello

press service.

So we have divided this into three parts.

One is for which is nothing but build a simple hello, well-dressed service.

So which will return it.

And the second is two, which will return Jason back means like we are going to return it being so that

it will be in decent format.

So that is like will return in simple, simplest and with first name, last name and then city.

So that one and the other one is like, OK, we are going to o come at these changes to the zero to

hello world respect to Branch and then we are going to push it to the remote repository.

So this time we are going to do our command line just to get an idea, just to get more experience with

the command line.

So let's do that now.

So let's start with the four year.

So first we are going to create a good branch, right?

And then we are going to create local controller.

So let's start with creating all these things step by step.

So in Hollowell controller, we are going to create a simple matter which returns a string Hallowell

and then we are going to mark the controller as the readdressed controller.

And then we are going to test with both mapping, a direct request mapping and then aderet get mapping.

So let's do that now.

So we are in our GitHub now.

We can see it here, latticed committees and I need to fight for the master and but for a zero on ground

zero base is something different.

So which means we have a second coming here.

But in the master, we don't have it, which means first we need to merge the zero one ground base to

the master and then push the code and then know from the master.

We are going to check out the zero one Hollowell branch.

OK, so let's do that now where our terminal look.

So I say get a branch.

OK, so I'll see that now we are in zero on ground zero.

So if we want to merge zero one, ground zero to M. So we need to go to Masterbrand.

OK, so get Ticketmaster before that.

You can even see the difference using short branch also.

OK, so you can see it both are Nazeem here.

OK, so master first come in.

This one happened after that happened in the second coming but in master we don't have those details.

OK, so what we will do is like we'll go to get out master will and will say it gets data so it will

show that we are on Branch Master and then we'll say good branch.

So that will get the list of branches and then we'll say good marked.

What is a branch way to merge to master is zero one hyphen ground zero base.

Right.

So now.

We have made it so now good status.

OK, so now, oh, we'll say good.

OK.

So say get push.

So now if you go ahead and then see that in our here, so let's see, OK?

So, Master, we have seven, eight, maybe seven to be OK, and here you can only eight, seven to

2B, which means like a both our master and then Zeron Brown is also in sync.

So now we can create a new branch named check out minus B, and then I'll said zero two.

Hello.

OK, so so this created and then we have checked out that.

OK, so let's go back to our idea and then see the same.

OK, so now we are in the idea with the 02 Hello world.

OK, so and in remote we still don't have this.

So if we want we can set this up with the first time.

Whenever we check out a new brand, our standard step is to get push hyphen set up stream like we do

a good get push hyphen set up stream origin and 02 Hello World.

OK, so now it pushed to the remote repository.

So now let's go back to our this one and then we'll click on we can see here file refresh.

We need to look.

OK, so we can see you're the remote also we have got the zero to Hello World, right?

So this confirms that we are good with the creating our new brand zero to Hollowell in both the local

and also in the remote repository.

And it is in the tech instead from local.

So we are going to do our next tune.

OK, so let's go ahead and then start building our Hollowell service now.

OK, so let's go ahead and create a new hello world class.

OK, so we can create another package, ok.

So I'll say hello package and in Hello package, I'm going to create a new controller named Hello World

Controller.

Right.

So now I'll click on Finnish.

Right.

So this is the controller.

So we are seeing it as controller.

Right.

And then now we are going to create a simple

method.

Right.

So we will say public and written by string.

So hello world.

And then let me return a string.

OK.

Hello world.

So now I am returning it.

Stringers Hello World.

So now we have created a simple matter which will return.

Hello World.

So let's now work on making this a rest controller so we'll see list controller.

So this will import the springform percolator, the rest controller package.

OK, so now we'll move on to making things like now we have the rest controller imported.

So there will be two things to handle here.

So one is how to access this in the rest.

Nothing, but it needs the euro.

Right.

So one it needs is the euro.

So we can see it as a slash hello world.

And the other thing which we need is like from our browser, from our last client, like Posman, with

which Matabele to access it.

Right.

So we are trying to get the data from this respective service.

So which means like it is going to be the get method.

Right.

So we need to implement that so we can do this in two ways from a rest perspective.

So they have two annotations to do that.

One is a direct request mapping and the other is a direct get mapping.

So what we are going to do here is we are going to first use the request mapping and we are going to

import that.

And then we are going to say method is equal to.

Request.

Metadata, you can see these all of the metadata supported from a spring framework perspective.

And we are going to use first thing as it get right.

And so we have completed this part.

So in the next year, you are nothing.

But it is also called the fourth.

Right.

So part physical to slash.

Hello, Lloyd.

Right.

So no.

It said, so we can see it here.

So what we have done is it is a controller.

We it as it list controller did it rest controller and we have written a simple hello world method,

which will return a string hello world.

And then for any other service, the important things are you worry politically to map to access it

and what metalic need to use either get put ok delete.

So it say it's going to return some content.

Hanawalt back to wherever we are accessing the respectfulness client.

So we are going to use the request metadata that get in the parties.

Hello world.

So let's start our springboard application and then go ahead and then tested in our browser.

So now our springboard application is started.

So let's go back to our growth.

So we are in our browser now, so we are going to see localhost

AT&T slash.

Hello, look.

So now we have got our Hollowell response here, we can see it here so I can make it bigger if required.

So, Hollowell, we got it.

Let me take it back.

Yeah.

So now this completes our Hollowell with a direct request mapping.

OK, so we can even do the same thing where get mapping.

So let's comment it out and then try to edit it, get mapping.

So far this we don't need to use.

Method is a call to request dot request metadata because we are treating it as a did it get mapping.

Right.

So now if that is the case, so then we can directly say.

Slash hello world right now.

I'll say hello, world one.

So just to see the difference, OK, if something cast in my browser or anything, OK, control shift

all from my windows.

OK, but your comment.

You've Yiftah OK in.

Mac, Yeah, so and then let me save it and then see the devil's behavior, OK, so it will auto to

load all the changes.

OK, so literally, you see, I just saved the file and then it started reloading all those things.

So that's the good thing about the bolts dependency, which we have added.

Right.

So now we'll say hello.

Well one way to get mapping and then is in our browser.

OK, so let's say hello old one.

So we got it.

So if you want, we can even see this as one and then save and relax this one more time.

OK.

Say hello.

Well, we've got to talk.

So this confirms that we are good with a simple hello world service, which requires a direct rest controller

as the controller annotation and trade.

Get mapping with the slash.

Leslie.

But OK, so this completes our string type of alola service.

So in the next lecture, we are going to work on creating it or we are going to return.

You will be.

It will be like on the on the browser, on the desk, like it is going to be the decent data.

So let's go ahead and do that now in our next lecture.

I'll see you in the next lecture.

Until then, bye bye.


### Step 11. Step-06: Create a Simple Hello World REST Service which returns a Bean (JSON).md
Welcome back.

Now we are going to create a method which militants have been in this lecture, so we are going to create

a simple matter with militants had been with some content like first name, last name, and then in

disinformed.

So to do so, we are going to create a class user details and then we are going to map it in our control

class.

Right.

So we choose in a very simple matter, which we are going to create in our controller class.

So let's do that now.

So.

So we are back in our ideas.

So let's do that from the first create a user details class here.

So the third new class and then see that as user details.

Right.

And in user details, let's define three attributes.

Provide string first name.

OK, and then.

Private string, last name and.

Private street city, right?

So we have defined three

attributes, sort of three variables we can see and then we will create.

Getters and setters for the same.

So let's go here and then generate, get Sensata, select all generate in the same way, will also create

the.

Source gendered constructor using Fields'.

OK, so we are creating the same now, and so we have created the Fields constructor and then we have

also generated the same set does OK.

So also generate the two string.

OK, so we'll see to string.

OK, so now let me also say bowstring, so this completes our user details, class creation.

So let's go back to our Hollowell controller and then go ahead and then.

Create a simple matter here, so public and what it is going to return for us is user details, right?

So I'll see user details, right.

And this says Hello world.

Then we can see it, OK?

So it is going to return the user details for us.

OK, so now we are going to return the user details.

So to do so, what we need to do is so we'll see a new user details and provide some data here.

OK.

So I'll see.

Uh, first name is color and comma.

Second name is really.

And first name and last name.

I have greater intensity.

I can see Hyderabad.

OK.

OK, so this is what we are going to return.

So I have completed creating a simple method now so let's go ahead and then create it, get mapping

for the SIM so I'll get mapping and redgate mapping and so.

Hello, world.

Hello, world been right, so let's say it.

So now we have completed creating a simple user, details being and then we are returning it back.

OK, so let's see what happens now.

So let's go back to our browser.

OK, and then say hello, world hyphen Bill.

OK, so if you see it here now.

The Hollowell bean is returning our first name, Ascalon last name is ready, and then sits Hyderabad,

Soini, Jason format.

So that's about returning it been so what we have done is we have we went over.

We have created a new class named User Details Class.

We have defined three variables, first name, last name and city.

And then we have created the first constructor.

We have created the getters and setters.

And we also created the two string.

And then we came back to our Hollowell controller.

And then we have created a simple method, Hollowell Bean, which returns user details for us.

OK, so and then we have created a written new user details with all three barratry parameters, whatever

it is required.

OK, and then we have added the get mapping so we can return the Hollowell being back to us and then

we are seeing the content in the different format.

OK, so here.

OK, so this completes the old bean section which we have discussed here.

So in the next section we are going to work on pushing this code and then merging this with M..

So this completes the complete Hollowell Razavi section for us.

OK, so for now, only for this respect to Hollowell Razavi section, we try to use the command line.

So it took a little bit of more time for you when we are doing the command line for git commands, but

it's a good idea to learn them.

So in the next lecture and also we'll try to use the idea so that it will be faster for us for creating

a branch, are committing the code or merging the branches.

Everything will try to Broadway it so that it will be pretty faster.

OK, but for for one last time in the step for how we have created the branch and then whatever we have

done here now in the next letter also will do the git push with all the commit code and all those things

directly will command line for one last time.

OK, and if required in middle for a few of the steps.

Again, I'll try to use the command line so that again it will be a refresher for you all.

.

Thank you.


### Step 12. Step-07: GIT Commit & Push Hello World RESTful service changes to Github.md

Welcome back.

In this lecture, we are going to commit the court, which we have developed in our previous lecture,

which is about Hollowell service being and then hello, World Service returning this string, all those

chord changes.

We are going to commit to our local good report, which is nothing but zero to a hollow world.

And then we are going to push it to the remote REPL at the same time, again, will take us back to

Master and then Master Zero.

Hello, World Local report to Master.

And then we will also push the master to the remote repo so that it completes that.

Our master is in sync with the latest to 02 Hollowell the branch.

OK, so let's do that now and then.

This completes our Hollowell service, the service section.

OK, so let me go back to the terminal.

OK, so clear and then I'll say good status.

So I am on Branch 02, Hollowell and Ontrack and file sohel one file in Hello four package, which is

nothing but our user detail service.

OK, so I'll say get and right and I'll say good status.

It became Greenall so user details service.

We have created Newlyn Hollowell controller.

We have made that in this case so I'll say it comit minus M and then I'll say uh

hello world this right.

And I have committed that changes.

So now I have committed this present in the local tripple.

So subject sure.

Branches.

OK, so now you can see it here in zero to whatever is the code.

It is not there in the master socket I will say clear and will come from the top.

OK, I'll push it to the remote branch first.

OK, so now I'm pushing it so that a zero to Hollowell locally and zero to Hollowell in the remote should

be at the same state now.

OK, super.

So it should be nine F for one eight three four.

Good.

So now what we'll do is we'll go back to our master.

Right.

Get Checkout Master.

So now we are in the master.

Right.

So now from in we need to merge the changes from.

Zero to Hollowell to master.

So I'll see you get.

Much 02.

Hello, world.

So now we have major changes.

So now they will do it, get pushed from the same master so that both master and master from local and

remote will be in sync.

So now master also will be at this stage.

So let's go back to our browser and then go back here.

And if you see here, Hollowell base came back to our master.

Whatever we have come to, just not right in the same way for zero to Hollowell, also Hollowell base

and it is nothing but nine have for one year committer.

I right it three four.

OK, it should be the same for our master to ride nine four one eight three four.

Right.

And now indictee also we should see that master is checked out.

OK, so let's see it here and then master should be not checked out.

Did see.

Yes.

So that is something.

So this completes the creation of forwarder.

Hello world.

This service OK with both a string and then beam and then also managing it via GitHub project.

OK, so in the next lecture, in the next complete section we are going to work on a bigger example.

OK, and then understand everything about get mapping, post mapping or kaputt mapping, delete mapping.

OK, everything in detail.

So I'll see you in the next lecture.

Until then, bye bye.

Thank you.

