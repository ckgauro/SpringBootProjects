### Step 40. Step-00: Introduction to Spring Boot - Validations & Global Exception Handling.md
Welcome back.

In the U.S., we are going to understand and implement springboard validations and global exceptional

handling.

So if you see valuations are the key thing for any of these modern Web applications today, even further,

the steps validating user input is a very common and key requirement in today's world.

SoSpringboot nable provides strong support out of the box for validations, suspended support, seamless integration

with custom validators, but de facto for performing validation hibernate validator.

So there certainly is a specification of Java.

You prefer being validations, which ensures that properties have been meet specific criteria using

annotations such as not Nadelman and then Max.

So if I see that wallet annotation, then Springbroot finds an argument annotated with valid, it automatically

bootstraps the GSA implementation, nothing that happened that validated and validates that argument

when the argument fails to pass the validation springwater method argument, not valid exception, exception.

So this one, we're going to anyway test it in our upcoming use cases.

OK, so that's the reason I have put it very specifically here.

So if I seem to be validation to specification, is that primary thing which we can look into that is

that you are going to have provided where we can we have the means to have a net validator and validation.

Everything okay.

So we can reference there.

OK, so let's not too commonly used the validation annotations.

So from validation annotations perspective, very commonly used from our entity are from our moral perspective.

Right.

So those are natnael, OK, so that the annotated property values natnael in the same way.

Other annotation is size, which we very frequently use to talk about the little property value has

this size between so inside tribute Min and Max and continuing to that we can have Minin Max annotations

which validate that the property has a value not smaller than that molad in the not the spec to attribute.

So another one is email ballbuster.

The annotated property is accepting the valid email address or not.

So other thing is not blank.

Validate that the property is not white whitespace.

So it was not empty.

Validated that the properties not nahlah empty.

So like this means like if you keep saying there might be many, many, many, many occupations from

both hibernate validator and Angelique's validation perspective, but on a high level, then coming

to Springboro services and then at the moral level, at the entity level very frequently used, I have

listed here for our convenience.

There is a certain relative stability, the property values true.

So movement to global exception handling.

OK, so this is the key thing, which is the organization focuses when they implement their applications.

So it applies to any of the web application or services.

Right.

So in our case here we are building Bisping Springbroot RESTful Services so far that also earlier in

our previous section we have implemented the exception handling using respon status exception, one

of the class which had recently provided for in Spring Fiacre.

So which will be more like a dynamic hasn't been everywhere.

Wherever we want, we'll be able to define that respect to the exception and then use it.

OK, but Trouillot exception and then use it.

But here so we have a general look, OK, our entire application exception handling so we can implement

global exception handling.

So why we have put this in combination with validation is primarily so whenever I'm doing any validation

anyway, it is going to throw the exception.

Right.

So and we need to handle that exception.

So for that purpose, in our previous section we focused on custom exceptions like username, not phone.

That user exists, all those things which we handle using response, status, exception, message.

OK, so but now we're going to focus on global exception, handling for the exceptions which are going

to be triggered using validations, OK, so that we have it in picture from exception, handling perspective

in the entire spring.

OK, so from again we're going to look at from Springbroot three, that one looks like we're a threat

controller best has been one of the key annotation.

OK, introduced in Spring 3.0.

OK, so and from that time still people are still using it primarily for the web and spelling it with

NBC.

But even for the controllers, we can use it and then it's frequently used.

So if you see controller advice allows us to write code that can be applied to a wide range of controllers.

It's not only for the exception handling, but for any of the global code, which we want to define

across controllers.

We can use the controller advice, right.

So this controller must play a key role when we are using the global exception handling so we can create

a simple global exception handling class so that it will be annotated with controller advice.

And the same thing will be used for us for defining the types of.

Exceptions which can be handled from Disrespectable Plus.

So that's what we are going to do.

So the other thing is by default, countermelodies annotation will be applicable to all plus that use

controller annotations, OK, which also applies for this controller because that is also one of the

controller.

Right.

So, no, the exception handler.

Right.

So this is one more exception.

Handler plus annotation for handling exceptions in specific handler classes or handler methods.

If you use it with controllers directly, we have the need to define it for controller.

But when we use it in combination with controller advice, it will be only used in the global exception

hand in class, but applicable to all controllers data controller advice capabilities.

OK, so primarily we are going to use this exception handler in our controller advice, so we are going

to see how it is going to be.

So the next user, the controller advice.

So this is again, I'd run sort of model out for controller advice.

OK, so we'll see.

What is that?

OK, service controller advice and the combination of the both controller advice and the response body.

So in controller that most we are supposed to manually define our response body, but from less controller

based perspective, it's a combination of both controller, less and less body.

So we can use the controller at sanitation for handling exceptions in the restful service, but we need

to address one's body separately.

That's about the rest controller and the controller differences.

OK, so but all in all, whatever we are seeing here, OK, are used for defining a global exception,

handling the scenarios so that you use this combination.

How we have arrived in implementing, which we are going to implement in the next few seconds, is listed

here.

OK, so the Fustiness controller advice and the response and to the exception handler class.

OK, so this is one more class for handling the exceptions which are there are predefined set of exceptions

defined in this class from rest services perspective.

So mainly from his duty perspective, we can say, right, so all those exceptions will be handled using

the spontaneity exception handler class.

So I bet we can use the default, which only gives the history to be status quo or we can override.

The methods are defined in this response and with the exception handler class and then also give our

custom message board whatever we want.

So we will implement our custom message body by automating the methods, presenting this response and

to the exception handler and see how it is going to be OK.

So that's going to be.

The important thing which you are going to implement so unabating is not that argument, not valid exception.

So this one by default, it is defined in the response and the exception handler.

And whenever this method argument, not valid exception is resolved, automatically we get a 400 bad

request tested in response code, but we don't get any message.

So what we're going to do is we are going to override this OK, right.

This default method and then implement it so that it will be in line with our customer response, what

we have defined so that we get both to be status quo and the request and also the custom at a response

message board.

OK, Jason, so we will do that.

And once we do this again, so it's a practice, right?

So when we are doing this, we might discuss multiple things.

OK, so and then to have additional practice for us, we'll also do one more time the simulator run,

the test method not supported exception, which we are going to be disrespectful to request method not

supported exception in response and to the exception handler class so that we have a good amount of

practice when implementing these two things, so that you can take it as an assignment for implementing

other exception classes present in this response and to the exception handler class to implement.

So in this combination, controller advice and in response and the exception handler class, we are

going to implement the two scenarios here.

OK, in the same way when we go to the controller advice and exception handler.

OK, so this exception handler is the thing where we hand, we define our exception classes right behind

this exception handler.

So rather than it is for the predefined exceptions like constraint, violation, exception, we are

going to implement one scenario.

And so as we implemented a predefined exceptions like system provider constraint, violation exception,

so we will have a feeling of also implementing the same for our user defined custom error exceptions

made custom exceptions.

So what we do is for custom exceptions.

Also like we have one method which we have created for something like a get user by user name.

OK, so this is one method we have which we didn't implement any exception handling or the response

status exception message which we have implemented earlier.

Right in the previous section.

So we left it one partly because we want to implement it here with the custom exception user name,

not for an exception.

So we will implement this user name, not one exception.

Forget user by user name method, and then we are going to define it as a method of placing an exception

handler so that whatever that response message we are triggering for exception for the user name, not

from the exception, it will be triggered from this hospital exception handler.

OK, so we're going to see that in the demo.

OK, so the next is the best controller advice and the exception handler.

So this is one more thing.

OK, so we are going to implement that with custom exceptions like the name, not one exception.

So whatever we have implemented here in the controller advice, the four custom exceptions like this.

OK, so I will go in there and then you're coming back that advice class, which means let me if you

come in this country annotation, then this global exception handler class will become involved, which

means it will not be in use for any of the controllers.

Right.

Because this will be whenever we enable it, then it will be in the context to say that it will be applicable

to all controllers whenever we come in this, it will become a general class of models for us.

OK, so I will go and then comment this out and then we'll create a new class custom.

OK, custom controller exception handler class.

OK, which is nothing but another global handler class will create with the rest controller advice and

then we will implement that in the name not one exception in this and whenever we test that.

So instead of this, we should be able to say this from this because this is commented out at the controller

at this level.

OK, so we'll see that in particularly just to understand how the best controller adviser, how we're

going to implement and what will be the pattern for that for that purpose.

We are also implementing this.

So that's about it, even if you want for when we are implementing.

Right.

For predefined exceptions, OK, for the entire or whatever it may be.

My exception.

OK, I'd like to put an exception handler dispute exception, that class, which means for all exceptions,

it is applicable.

Right.

So you can be trained for the exceptions and then in the exception handler and then it will be applicable

for all the exceptions, whatever the customer said you want to trigger so that the customer, whatever

stupid response could.

One important thing here is that British controller.

Later, we are going to say an annotation response status, which is another indication we are going

to use it.

OK, so that's a very bad advice.

So no one, no implementation steps, right.

So as a first step and step.

Everywhere, wherever we do this right in all of our sections, we're going to create a good punch for

validation and this global exception handler.

Right.

So we'll keep up and then from then we'll start our implementation.

So we'll clean our massive plant and then create a new Blanchot validation and global exception.

Handler And then we'll move on to implementing validation.

So this section is about validations and also global exception handling.

So it is a combination of whenever a validation happens and it fails, then it exception will be fired

and how to handle that exception.

That's about the overall situation.

Right.

So implementing validation will implement validation and will follow it step by step approach when we

are doing the validation.

So which means like first we will implement reporting validation.

When the error occurs, what will happen right.

Means like you will get a little exception because it's a project that.

So then we'll go and then implement with a trade value to the validation for the request body right

at the time.

We'll get that method argument, the exception not from handler.

Right.

So that that one will be fired.

OK, so and then now we're going to handle it.

Right.

So then you'll want to implement custom of global exception, handler using controller advice and response

and to the exception handler.

At that point, you will handle that retrospective method of the exception here.

OK, so and then are not really the exception.

You are going to handle it in this Tirpak by implementing a custom global exception handler.

So the next Wimborne implementing exception handler for this method not supported exception.

So that's the thing.

OK, by picking, by writing the method defined in response and to the exception handler class.

Right.

So I will move on to the next step, which is nothing but implement exception handler for custom exceptions

like username not for an exception using exception.

Handler annotation.

Right.

So that is the thing.

So one more step.

So here's what we'll do is like we will implement the part where validation software, which means like

in the path variable like that user by user ready.

Right.

For that part, validation so exemplary should not be zero at any point.

So you can say that.

Did it mean zero?

OK, I mean, one woman means at least only one.

It should start from one.

OK, you should not such but zero.

Right.

So like that if you implement it will that constraint violation exception.

Right now we are going to implement it using exception handler in customer level exception handler with

controller advice.

So we are going to see that and then we'll move on to step six, implement global exception handling

using the rest controller advice.

OK, so that's about all the things which you are going to implement in this country that we are going

to implement the further one of the user name, not from exception, and then we're going to toss that

thing.

OK, so I'll see you in the next election.

Bye bye.

Thank you.


### Step 41. Step-00: Create git branch for Validations & Global Exception Handling.md
Welcome back.

It looks like we're going to create a good punch for validation and global exception handler.

OK, so now we have completed close to four sections and in all the sections we are starting, step

is to create a good brand, either with idea or either with the command line.

So we'll see the step once and then as already, we have done it multiple times.

This time we'll just go through the step what we are going to do and then we'll move on.

OK, so first we verify that we are in good status to ensure that we are in the master masterbrand and

then you can to get your code hyphen to create a new blood zero violations, global exceptional handler.

And then we'll create.

GitHub branch, using the get get push hyphenation, set up a origin and then in origin at this point

of origin is nothing but the remote.

And then what if I ever see a man ever get up?

That's all.

OK, so we're going we already implemented these steps, so we'll go to right.

And then verify the same.

We can see here through for validation.

We will exceptionalities created OK.

And same is also created in the remote branch too.

So this completes the creation of GitHub step.



Until then, bye bye.

Just to save time or instead of having that as a repetitive step.

So I just ensure that I have explained the steps here and then already exhibiter those things and then

put that ready.

So I'll see you in the next lecture and bye bye.

Thank you.


### Step 42. Step-01: Implement Bean Validation - @Valid.md
Welcome back.

In this lecture, we are going to implement the bean validation, so if you see our steps here for bean

validation, so what we are going to do is in the end here, we are going to implement validations on

identity objects, OK, which is nothing but user entity variables.

OK, whatever is there there.

So we have user name and also first name so far.

I mean we are going to apply it did it not empty.

OK, and we're going to also add the message saying that username is Mendeleev.

Please provide username in the same way for the first Memphian.

We're going to add annotation sites with the minimum as two character.

OK, so if you want it is going to fill in the same way here.

If you don't send any user name value, it is going to fail.

If it's an empty user name value, it is going to fail.

So our important thing is when it is going to fail and then what is the exception we are going to get?

That is the thing we need to focus on when we are implementing the validations.

And once the exception comes home, we are going to handle it.

So which is nothing.

But whenever we are implementing validations, no one is OK.

So it watkins's it is going to fail and in that case, without exception, it is going to throw that

number to and hopefully handle that.

Exception is rule number three.

So we need to be aware of these these three things when we are implementing the validations.

So what we do is we apply these two things to our respective entity objects there, and then we'll go

to our postman.

And then in the request of the creators of servicing the body for the first name, we will dispute one

character so that this will feel right.

So because it said minimum to the same user name will just send the empty string so that this will fail

and then we'll see what will we get it.

OK, so we have not implemented anything special here.

So it will be like an exception from the dippie level right away because then it will communicate to

the back in his database.

So you'll get a deeper level exception and will verify that.

OK, we got it.

So now after that we move on to the controller and in the controller, layer four will enable the validation

using a direct value for the request.

But what we are sending will add elements like a valid annotation to that.

OK, and then we'll go to the postman and test for a booklet with the service and we'll send the same

data.

What we have said, cefazolin with one character in the user name with the MVP's.

So what happens is like we get different, another bad request, OK, and then we verify the log.

It says that method are not valid.

Exception will be solved from the logs.

So which means this respect, the exception got resolved.

OK, so we'll see more in detail later about this exception in the next step.

But this exception got resolved and by default we got the four hundred bad requestor history to be status

quo.

But we don't get any more responsible.

We will not get any of this.

So let's see these things in step zero one so that we know that we got the X, we got better and then

how to handle the exception.

Will more on 022 handle this by creating a global exception and handling the class and all those things?

OK, so let's move on to just implement these things for now.

OK, so first thing is to implement validation.

So I'm.

So let's go back to that idea.

So this is a variety, so we are in the zero five validations, global exceptional high level bank checked

out.

So I'll go to that lady and now I'll go to our user entities.

Right.

So this is the user entity.

And if you see here, we have this.

OK, so let me apply also one more annotation here.

Did it not empty?

So and then we can say, come on, shift auto import so we can say that deregulation, OK, the same

way or even the highway network later.

It's up to us.

OK, so then your deregulation.

Furneaux so and for first name also with the car payments like a great size and then MRD suggested the

message is bigger one here, whatever I have written.

So just to ensure that save time I'm just copying those things.

So what I'm doing.

OK, in addition size with minimum two characters.

OK, my first name should have at least two characters.

OK, so I'll import those.

OK, so Giwa actualisation constraints.

I also got imported so now I will save this.

OK.

So currently this might not have been running.

So let's start over Davian.

So let's start the JVM now so I'll see if I click on this HealthSpring boot up.

OK, so my Davian got started, OK, so we'll go to the postman, no.

OK, and we'll go to the creative side, right?

So we should be able to use it now.

And the first thing is we are sending one character for the first name and use them.

We can send it as empty deck.

OK, so let me send it.

So now if you see here, we got the 500 internal server.

I still think it is a bad thing, which we should not see OK, from this client perspective.

And that is not a good thing.

And then we should definitely handle that.

OK, so no, we will go to our error message so this year could not come a transaction.

Mr. Exception, is Dalek's persistance.

Rebecca Benwell committing the transaction.

Right.

So we got the end of an exception, OK.

So now instead of going to JP and then getting the an exception, OK, so we can handle this, we can

validate this at the response by itself because by level itself, whatever it is, it that level.

OK, so it will go to our controller user controller and then we'll go to work with user.

Right.

So this is a user matter and what we do is before request by the annotation will add the.

Valid annotation and then.

We will put it OK and then we'll save it.

So what this does is likely to invalidate the Red Cross border, whatever is sent here itself.

OK, so no, go ahead.

And then again, that's the same thing.

OK, so let's send the same thing.

So if you see, you know, they got the 400 page request, right.

And we got the default message, which.

Spring is constructing for this, OK, so we have got a different message saying that I will go down

and then see it in detail, see, so like I said, we have got here, OK, so size, user name, first

name.

And if you see here, first name should have at least two characters.

This is coming from our message field.

Look in the same way for username.

Also username is mandatory for all.

Please provide username.

So whatever is being provided by default.

OK, but.

Responds by a request by the validations.

It's like being validation looks good, OK, but it looks very big, OK?

But when when we plan to do these things, OK, and at every level, if you want to define a standard

exception handling procedures, then all these things doesn't look good.

Right?

So it's like if you have four or five frames which are which you have standardize for the entire global

exception handling, then we need to handle this exception also into that framework.

Right.

So those things we can do our next step by implementing the global exceptional.

So let's go back to the console log and see what has been thrown.

OK, so if you see here in the console log, it said that method argument, not valid exception.

So it is no disrespect to exception with the two errors, validation failed first time.

So argument.

That's why I'm so OK.

So which means like whatever the exception now thrown his integrity to resolve this matter argument,

not valid exception.

OK, so in our next step, we need to handle this exception and then send a custom message, OK, customer

response body and should have this big information, whatever it is giving.

OK, so customer responds with timestamp details and then some message.

OK, so that that should be good for us.

OK, which is like blah blah of handling model.

OK, so it might be even more but even more famous and all those things in real world.

But I will try to implement and understand how we are going to implement the global exception handling

with the controller in the next section.

So I'll see you in the next lecture and building by.


### Step 43. Step-02: Implement custom Global Exception Handler - @ControllerAdvice.md
Welcome back.

In this lecture, we're going to implement custom global exception and let the U.S. come to another

place.

And also we are going to be looking to respond to the exception handler class.

And we are going to also override the methods defined in response and to the exception handler class.

So and then implement those methods.

OK, so let's go ahead and then see what all our detailed steps you are going to implement as part of

this step zero two.

So if you go here, so we are going to implement a custom global exception handler saying that exception.

Well, going back to classes.

OK, so first one is customary for custom and we can tell you in detail customer details.

OK, so we going to create a new class named Customer Details and we are going to define variables like

that message and then our retails and we are going to add things constructor and then get us inside

that nothing.

But we are going to create a customer that details being OK, which will be helpful for giving the responsibility

for all our exceptions with a big message and then other details.

So in the exception matrix elements like the exception package itself, we're going to create one more

class named customer global exception handler.

OK, so what this going to do is this is the core handler class.

It will handle all the exceptions, whatever we want to handle in our application so we can keep adding

all the methods inside this class for what are the exceptions we need to handle globally.

So we're going to create this class and extend it to respond to an exceptional handler.

OK, response to the exception handler is the core class, which will have the details about all these.

It will have the methods for handling the fuel.

Are the important exceptions OK?

Mainly related to the services.

OK, so if you see here, you're also going to annotate disrespect to class with the controller advice.

OK, so that can be applied to a wide range of controllers could continue that.

This will apply means like we can define the Global Code of Global Error Handling's custom handler.

Right.

Whatever we are defining that can be applied to a wide range of controllers using controller advice.

So that's the reason we're going to annotate our custom global exceptional handler class with the controller

controller advice.

And next, we'll move on to implementing a handbell method argument not valid.

So there steps to zero one.

We know that method are not really the exception we have seen.

OK, so it's a common method will be there in the response, the exception handler.

So we're going to implement this method.

And then what about the existing method?

OK, from Lesperance into the exception handler and then we're going to test the quality of the service

with the same things.

What we have done in step one, which is first name one character, and then use a name with them the

string and then modify their response.

So we should get our custom response, whatever we have defined with the date message and then other

details.

And also we should get the story before another bad request.

So we are going to perform all these things in this customer.

One exception handler step now.

So let's go ahead and then implement that now.

So we'll go for it and then implement the same thing.

We'll start with creating a lot of customer details.

Plus they come back.

So we are know now.

So it'll go for exceptions package, so know exceptions.

Currently we have used this exception and use a not from exception, these details which we have implemented

as part of response dataset, an exception, which means like if I remember in our response status exception,

you can see it here.

Right.

So during this implementation, during this section implementation, we have defined these error messages.

OK, so now whatever.

We are defining the global exceptional handlers.

Right.

So we should ensure that both like we are not colliding with the response status exception, the letter,

the exception handling and our global exceptional handler.

OK, in this project particularly, it's a good practice that, as I said in response, status, exception,

conclusion section also that we can use both things, which means that global exceptional handlers using

controller advice and also response status exception, which has been included as part of spring fire.

Both things we can use it.

But one thing we need to ensure is that whatever response status exception is handling those exceptions,

we should not be finding other notable exception handler.

And whatever global exception Handler is handling the exceptions, we should ensure that those were

not handled by this one status exception.

So which means like there should not be any confusion state for the system to decide which one it should

use.

So we should have.

Carefully, so we are doing that now, and that's a good thing, right, which means that we are going

to learn a lot of stuff here.

So now go to new and then create a class.

And are exceptions seeing custom error details?

Right.

So this is our custom details class and.

We can just give the message messages quiet.

Simple cost.

Custom.

Her details being OK, so just we are defining this and then we'll define our three variables.

So one is a private bit and then we'll define it as our timestamp.

Right.

So the second is private string and then message whatever we want to provide, OK?

And the next one is private string and then other details.

Whatever we want to report are we can even see a message, too.

So this is a generic message and this is error message.

So I'll say the details.

OK, that looks good.

OK, so now we have defined our variables, right?

So now we'll create our field constructor.

OK, so let me create the concept of using fuels and then generate the constructor.

OK, so next is so this one.

Let's import this data in Java util date.

OK, so that's good.

And then also generate the constructors so to get us right.

So select get us and then generated.

So now we'll see these as getters and.

This is

thrill's constructor and then let's see if this OK.

So now we have our custom error details class created.

So now we'll move on to creating our custom exception, custom global exception.

Handler.

OK, so.

So let's create that now, so I'm in the exceptions package and we are seeing classers.

Custom.

Global.

Exception handler.

OK, so we are creating a new class custom global exception handler and this class, what we are going

to do is let me make it bigger.

Yeah, so it should.

Extends right response and the exception handler, slow response entity, exception handler.

OK, so and then import this one.

We should we could know, so now if this custom global exception handler should be applicable to all

the controllers.

So what we need to do so we need to add the.

Controller advice.

Right, so let's import that package, too.

So now this was discussed and global exception handler will be applicable to all the controllers, whatever

will define the code.

Yet either it is exception, handling include or whatever the code.

OK, whenever we are annotated with controller advice, then it's globally applicable to all the controllers.

OK, so now we will go ahead and then override one method.

OK, so first we like the method name here.

My third argument.

Third argument, not valid exception like this one we are going to handle here, so let's go response

and the exception handler ones and then see what is present inside that.

OK, so.

So what we'll do is we will say.

Response.

Entity exception handler.

Right.

So let me open this, OK, so a convenient win this class, OK, this one.

So if you see here.

In this class, we need to go to the if you see in detail, OK, so that it's the exception handler

for all of these exceptions has to be a request method, not supported his GTP media type not supported.

OK, not acceptable media type, missing part, variable exception, missing cymotrichous, parameter

exception.

So like this we can see lots of exceptions which can be handled using response and the exception handler

class.

So in this our thing is method argument, not valid exception.

So if you see here, it's equal in method will be defined in this response and to the exception handler.

So let's go there.

OK.

So if you see here, so this is for the Questors GDP hand initiative request method not supported in

the same way we can search for a method argument not valid.

OK, so see here it is.

OK, so custommade the response fair method argument not valid exception.

So we are going to take this method and then implement it the way it is required for us.

OK, so we'll copy this method, OK.

And then use it in our custom global exception handler thing.

OK, so what I'll say is like control v OK.

And then I'll remove these things for whatever the written moonlighted.

The weight is required for us.

OK, so.

If you see here, handle method argument, not valid, right?

So what we're going to do is we are going to override this existing one.

So I'll.

All right.

Right.

So now what I will do is I we have something called the customer details.

Right.

Using this will set the details, whatever we need for this list.

But the exception, method, argument, not valid exception.

Whatever the message we want to send.

We will send by our being, OK.

So I will define our being here.

OK, a customer, other retail sales customer I love details is a call to new customer.

Other details.

Right.

And.

So inside this, we have three parameters, OK?

So one is a bit messy and then other details.

So the first one is dead, right?

So I'll see.

You bet.

In the same way, the second message, so I will say this as a name, whatever we want to argue, OK,

so far, no, I'll just give that it is coming from Matara argument, not valid exception.

This is just for our testing.

Right.

So I say.

From my third argument is not valid exception, OK, in global exception, handler, OK, detail Zilkha

shortcut for us, OK.

So now and the other one is the third one that also is trending.

Right.

So what we'll do is we'll bring this down here, OK.

So and here audiences will get something from our exception.

Right.

We have metadata argument, not valid exception.

So from here, we'll try to get some better details.

Why?

Because our third parameter here is error detail, some additional information about our error rate.

So I'll see you next, Dot.

OK, so whatever we want, we can get it, OK?

So I can say get localized message, whatever the string type me how we can get those things so I get

localized message or get message so we can get.

So I'll try to get some message here.

OK.

So initially we'll change it and then implement something else later.

OK.

So now we have a word.

Customer details to define.

OK.

So now we need to return the response entity to this.

OK, so let's return the.

Response entity, right, and.

What are we going to return this customer details, right, so customer header details and also our

history status.

OK, so I'll see EDP status that bad request.

OK, so I'll send that bad request.

So.

I can see the object here, so this should.

Konsta response entity, right?

So I need to say, New York, we should be good, OK?

I can even put to death that.

OK, this should be good.

So now let me save it, OK?

So if you see what we have done is we want to have a response to the exception handler class.

So why are you destroying error.

So Jabor, you still get little input, OK?

OK, let me say it, OK?

No errors, we should be good.

Yeah, so what we have done is we went to the response and to the exception handler class and then we

tried to find our Matara argument, not valid exception, related method here, and then copied that

method to our custom global exception handler, our class, whatever we are defining here.

And then we have already the existing method handle that argument not valid.

OK, we annotated it with.

All right.

So now we ready for that matter, whatever we want, we can write inside this.

So what we have written is we have brought our customer details being here and then said the messages

inside that.

And when we are retaining that customer details information back to our whenever this exception happens,

then return these things.

We are saying, OK, so and then you're also sending the status should be status, that request.

OK, so this completes the implementation of method argument, not valid exception, handling using

custom global exception handler, which extends the response into the exception handler.

So now we'll go to the postman and then test it.

OK, so this is the thing.

And if you see your username is empty and first name is.

So let me send it, OK?

Calm down.

So if you see statuses 400 bad reckless timestamped, we have got a message.

So I have a message from metadata and not valid, exceptional global exception handler.

I have defined it without it and other details you can see validation failed for I have said the exception

that get message right.

So using the exception.

But let me say it.

You have got the validation feel for argument in public and then you have got all the details.

OK, it said was rejected in the first name rejected.

You have got some information which is good.

OK, so this way, whatever we want, we can define another custom global exception handler and then

handle the methods, whatever we want to handle, which means like whatever the exceptions we want to

handle, we can handle.

So this is what we have done in this section.

So in this lecture, in the next lecture, we are going to also work on another method in the same pattern

so that we get a little more experience on implementing, using less brons and with the exception handler.

So if you reiterate what we have done just one more time, that we have created a customer details class

and then implemented messager, other details inside that and with the exception layer itself, same

exception layer itself, we have also implemented custom global exception handler and then we have extended

it with the response and with the exception handler.

We have annotated it with controller advice and then we have implemented a handler method admin, not

valuable, copying it from response to the exception handler.

And then we have overloaded the existing method and then implemented it with the message whatever we

feel is good for our organization.

And then we have to start with the postmen and which confirmed that.

Our customers are just coming out expecting the global exception handler when we implement the global

exception handler.



Until then, bye bye.

Thank you.


### Step 44. Step-03: Implement HttpRequestMethodNotSupportedException in GEH.md
Welcome back.

In this lecture, we're going to implement exception handler for his teacher, Pinecrest method not

supported exception.

OK, so this is also one of the exception which is already defined in the response and to the exception

handler.

OK, so we are going to override this using our global exception handler rule class.

OK, so let's do that now.

So let's see the steps ones.

OK, so first we are going to test using Posman that when we provided batch method, this is the method,

not supported exception.

Right.

So whenever we operate a batch method for create user, what is the response we are getting.

Right.

So and then we'll go back to the exception here and for our custom global exception.

Handler So and then we'll implement this Handal method argument.

Not valid from the spontaneity exception.

OK.

OK, this is a copy paste issue.

It should be handled, has to be a request method, not supported.

OK, so we are going to override this matter from response and to the exception.

And then again, we are going to provide batch method for creating and modify the response.

So first, let's go back to Obama Posman and then test it, OK?

So I will do some usernames.

Kirrily one one and I'll say this is Carillion, right.

And this is a that it should be a valid user.

Right.

So if I a post it should work ideally.

Correct.

OK, so it got created.

So in the same way I'll add one more for this unique constraint in here, not a large one.

So that no unaccept batch method.

OK, so this, this particular post method.

But I'm sending the patch method.

Let's see what happens.

OK, so batch method it said.

But for your file method not a allowed but we didn't get any bloody response.

OK, so which means this is not good.

OK, ideally we should also get some method saying some information.

OK, so let's go ahead and implement that now.

So let's go to our idea.

Right.

So if in the response entity, the exception handler, we can see it here handling GDP request method

not supported.

OK, so let me copy this method and then come back to our custom global exception handler.

Right.

So and what is the for which method we are doing this.

So let me add in this little bit.

Good.

Yeah.

So now.

Let's go up.

Right.

So far, which matter we're implementing is her to request method, not supported exception.

OK, so here's GTP request method not supported exception we are going to handle here.

So let me copy what we have copied from there.

OK, so all these things, whatever it is, they're here.

OK, so and then we are going to implement our customer details.

Right.

So let me copy these customer details from here.

It is going to be same.

Right.

So.

And also written and then edited whatever is required.

Right, so I'll say.

Customer details from, say, from.

SDP status from here, I am sending this message like this, OK?

And yet just I'm saying this one deadly.

Whatever we want, we can say example like a method, not a law.

I can just give an idiot and I can even say, additionally, I turn out the law, OK?

It should be more reasonable when we are implementing and production are for real cases.

But I just want to ensure that this is coming from G.H., which is nothing a global exception handler.

So I just gave like this.

OK, so in response entity and then customer details and then it is method not phoned.

Right.

So dark matter not allowed.

Yeah.

That is the one.

So I'd say method not outlawed.

OK, so this completes the response has to request method not supported exception.

Implementations of what we need to do is we need to also override the method.

Right.

And, and control Chief Def so our command should have to.

Formatted and then save it.

OK, so now we have implemented to method, good method, not supported also.

So let's go back to our.

Posman, OK, and then for creative users using the patch method and then send it.

OK, so now if you see here, I got the timestamp and I got the message from the person I did not support.

Immediate exception in G.H. and Method not allowed.

OK, whatever we have defined and other details we have given, but get a message which is the method

Bache not supported.

OK.

So like this.

So we have got the information, whatever we need, and also to be sure to score we can see for free

method.

Not a lot.

OK, so this completes the implementation of his request method not supported exception.



Until then, bye bye.

Thank you.


### Step 45. Step-04: Implement UserNameNotFoundException in GEH - @ExceptionHandler.md
Welcome back.

In this lecture, we're going to implement exception handler for custom exceptions like yours and not

from exception.

So let's go ahead and see the steps involved for this, OK?

So before even going, further steps will go toward idea and we'll see a few things.

OK, so you know what?

I seem to use a controller for a project we didn't implement any exception handling forbidden user by

user name method.

OK, so which means for all other methods use in response, status exception.

In our previous section itself, we implemented it OK, but we left this alone because we want to handle

that in our global exception.

Handler Kissack.

So that's the reason they didn't implement it earlier.

So now they're going to implement it.

So what we are going to now define is we are going to define a customer exception, use a name not from

exception, and then we are going to handle that exception user name, not from exception where custom

global exception handler.

So let's see how we are going to do that and what other steps involved for that.

OK, so let me go to the steps here.

So the exception.

First, we're going to create a new class user name, not one exception, which extends the exception.

And we are going to create a message constructor, superclass, constructor with the message as one

of the string there.

OK, and then one more under control earlier.

And then for that great user, the user name will throw the user name not for an exception and then

will implement that.

OK, so that one again, it's like whenever there is an error, it will throw the user name not for

an exception.

OK, so whenever that user is not present in the repository, it is going to say that user name not

found the exception.

It is going to throw that exception.

So we're going to test that where postmen and then see right there, it will throw that interesting

exception.

We test you to define the letter.

So and then remember a custom global exception handler and then create a handle user name, not for

an exception method.

Right.

It is called Method and then annotate.

Annotate it with.

A, the exception handler, and then provide this username not from exception class and said this exception

handler and then tested again with the postman so that whatever our customer said we have defined here

should be shown.

OK, so let's go ahead and implement this now.

So first is to create a user name, not one exception.

Right, so let's go back to our I.T. and we are in the exceptions clause, OK, package, new class.

I mean.

It was a name not for exception.

Right, and then finish, OK, and then which extends the.

Exception.

Now, this year before the Civil War tonight and then also the final constructor, right, super superclass

constructor.

So then that constructor from our super class, this Alectown and then select only with exception string,

OK, generate and then we can call it a super class constructor.

OK.

OK, so let's say it so now we have completed the user name, not one exception, a custom exception,

creation.

So now let's go to our user controller, whatever, whatever the user name, let's make it bigger.

So let's make it to center so that we can see it in detail.

So now what we will do here is a.

We'll get the username and then save it, right, so I can see.

That I copied this return, will write it later, so I'll say user.

User is equal to users, I will start getting user by user name, right?

So now what I will say is if.

User is equal to null then through no user name, not phone.

Exception light, so new username, not form the exception and then just.

This way, OK?

So and then import this, OK, imported, so now next year is going to be.

I have the details right, so I'll see.

Username.

Plus user name and again, plus and I will say.

Not in user.

Repository.

OK, so this should be good now, OK?

So if you were equal to throw this exception, OK, if not.

Then do one thing, OK, so what I need to do is return users.

OK, that's good.

So one more thing is a trust declaration for this matter.

OK, so trust you that not one exception.

OK, that's good.

OK, this looks good.

So now we have completed the.

Get get user by user name exception handling here, OK, so whatever we have said is like if user is

equal to now, we have brought the user and then if user user name not from the exception and say that

user name, not one in this user repository.

And if we get the user then immediately return the user.

That's what we have implemented.

OK.

So let me save it.

And then once it is sold, we'll go back to the postman.

Right.

So we are in that postman so no.

We need to get user by user name, right, so that was a user name, so and we should have the user

by default, which is a divisor.

OK, so let me see.

OK, so we have the divisor user.

OK, so this is one zero two.

So now what else is like I don't have a user name obesity so I send so it this timestamp and then status

500 and other detainees impanelled say whatever and message we got see which is username ebiquity not

for name, user repository, whatever we have defined thing is happening it effectively but it is trying

to find that error and then it is sending it in in the spring standard for times translator's error

message and then Patoka so we can.

Convert this into a global exception handler now using annotation, exception handler.

So let's do that now.

So we have verified it by implementing a simple user name, not from exception, custom, exception

for other good by username method.

And then we have tested it.

So now we need to convert this into our global exception handler case.

OK, so let's go ahead and then do that now.

So to do that, we need to go to our global exception handler, OK.

Made the comment username, not phone exception.

We are going to handle now so and say, OK, public final.

OK, so one thing is we need to return the response entity.

Right?

So the response and the object and I'll say handle.

User name, not the exception.

And then I will write my exact username, not from the exception here, OK, so let me make this because.

Yeah, it should be visible now, clearly.

OK, so I'll say use a name, not for an exception.

And inside, this will be the parameters, OK?

When his user name.

Not for.

Exception.

And I'll say he cuma.

That request.

Request.

Right, and.

Let me go down.

We get this here and capital.

OK, so this should be good.

Now we should be waiting for the written statement, OK?

So before making the written statement, our standard thing is to get our customer details right.

So copy from here.

Our customer details and also our response entity.

Right.

So both things from our previous thing.

OK, so first thing in customer details, we are going to define the stuff, right?

So the second is I'll say you start that message.

OK, let's not get messager the second parameter.

And as we're also sending the request, the requesting, I can say, a request to that get a description.

Right.

Good description.

And if you want, we can even include the client info.

OK, are we can say false.

OK, so whatever we want.

OK, so and the other thing is what is the thing is whenever there's a name not for it is like not font.

Right.

So is it not font.

OK, so now we have implemented this one.

OK, so now we also need to implement the exception handler.

Right.

So we have implemented a base method.

No handle.

I mean not from the exception.

We have two things.

He was a name, not one exception in the request and in our customer details for three parameters.

The first one is date and second one is not get myself and use a not for an exception.

And third one is from requesting that we call that good description, OK, and that and then from a

retail perspective, we are sending the customer details in a CTP status that Nachshon, which is for

the Florida building where we are clear.

So now the important thing is how to handle this, right?

So we have to find a method, but the revenues are not for the exception is filed or whenever that occurred.

Right.

So then this message should be triggered.

OK, so to do that, we need to use the annotation or annotate this matter with exception.

Handler, right.

And then come on.

Or imported.

And then so we need to define the actual user name, not from the exception, that class exception,

not class.

OK, and then we should be good.

So that's all.

OK, so we have done three things here.

One is.

We have created a great user by user name.

We have implemented the user name, not from the exception handling, customer exception, handling.

We have implemented and secondees in our global exception handler.

We have implemented the handle user name, not from the exception.

Well, and then we have also added the exception handler to catch this user name, not one exception,

and then try it whenever it occurs.

OK, so now let's go back to whether I have saved this.

So let's go back to our postman and then test it, OK?

So did you ever use an emergency for ABC?

Watch what happens.

So I have got instant messages, username ABC, not only the repository.

This is coming from our user name, not from custom exception.

Whatever we define further from the text messages coming in, from error details, whatever we said

is get that description right for a phone without the message correct and get that description for all

to be said so that we have got to talk.

So it should have a better description, whatever we want to put from request perspective.

Also, you can even see through, OK, how to include client info, is that right?

So I can see through.

Let's see what happens with Drew.

Right.

OK.

So we have got the climate in for here, some Tripura, some information.

OK, so we are optimistic for whatever.

OK, so but you got something here.

South Africa was that good description.

If you have an interesting type format, we can even get context, but we can get her that.

We can do whatever.

OK, so our get parameter, whatever, but we might lose her if you get S.A.T. or whatever we want.

We can send it back here.

OK, but we should be sensitive in sending these details.

But as far as like just whatever, one percent has better organization standards.

We will define and do it right with proper reviews.

So just this is like only what we call OK for testing purposes.

OK, so this is what happens.

So, yes, I mean, not one exception.

Related steps completed.

OK, so we'll save this and then we'll go back to what steps and what we have done.

So we then brought exception to the user name, not for an exception, OK, and then within to country

for better user by user name.

OK, let me see.

OK, I get user by.

He was an amateur, so we have implemented this, he was an important exception and we have tested it.

We got the to be 500, OK, and when we brought exception to the hand user name, not one exception

method and read with the exception handler and then added the username not from class here.

And then we have posted it and then we have got the customer response and there should be status quo

as a four or four.

OK, so this completes our username, not one custom error message handling using global exception handler.

So now in the next section run more like we have implemented using the exception handler.

We have handled the custom exception, right.

Custom defined exception.

In the same way, we can also use systems exception, which is nothing but example.

You can consider like a constraint violation exception so that when we can implement.

So in the next step what we'll do is we'll do the part validation and implement part validation and

it triggers the constraint, violation, exception.

And then we will handle that exception using a global exception handler.

.

Thank you.


### Step 46. Step-05: Path Variable Validation & ConstraintViolationException in GEH.md
Welcome back.

In this lecture, we're going to implement of this validation and empowerment exception handler for

constraint violation exception, which occurs as part of this part, variable evaluation.

OK, in the global exception handler, which we have built.

So let's go ahead and do that now.

So we're going to review the steps involved in performing this, OK?

So if he see here in the control earlier, OK, so we're going to add a direct mean one for part variable.

So for.

Which one get yuzu by?

I met her, so we are going to implement this, so I had a great run for pat variables, which means

my ideas should be one, OK, so it should not be zero.

So this validation we're going to implement for our part variable and profile that we are going to say

it, but it means like a validated annotation will be applied at the controller level.

So when do these two things at the controller layer and then we'll test it via postman and then as usual,

standard will get the 500 exception.

OK, spring exception.

And now again, we need to handle that.

Right.

So using the global exception handler, we are going to handle this 500 error, OK, in our desert.

OK, global exception handler.

And then we are also going to use exception handler to catch that exception and then throw it whenever

it occurs.

OK, and then we are going to test it using Posman again.

OK, so these are these steps we are going to implement now.

So let's go back to our idea.

OK, so we are in the idea, you know.

So let's go for the user controller.

Let's go up.

So we have over kidnapping saying get you by right and here we are going to implement travel validation,

part rebel validation, I will say minimum value should be one OK, and then can come on shift how to

import that validation.

OK, so now this is completer.

So we'll go to other countries at level and then at the um, at the rate.

Validated annotation.

Right, so import that now.

OK, so now part of is validated.

OK, so let's go back to our postman and then get you there by Idy, right.

So I will say just test a positive test, one zero one.

It should be working.

Right.

So and then one user not there.

Right.

So it should for for a because the response status.

Exceptional response status exception message.

Right.

So that when we have defined earlier.

Where is that.

Where is that response.

Status exception.

OK, so these things we have defined right to through whenever use are not fun.

So it has thrown correctly.

So now it is four zero seven so zero.

What should happen.

OK, send it back 500.

Whatever case we want to test, we are testing now, which is with zero, as we have said, the part

where the variable should be minimum one.

So now we have said with zero and then it said internal server error.

OK, get usability must be greater than or equal to one.

OK, so this is the thing and we are getting the response responses 500 internal server error.

So we need to go to the global exception handler now and then fix this, OK.

So let's go back to about, uh, idee.

Right.

And.

So and if you go to a Web logs right here.

We should have seen that where he said constrained violation exception occurred, OK?

So whenever whatever we have done now we have girdler constraint, violation, exception, one more

time will test it for our convenience, OK.

So, yeah, zero and then 500.

We have got it here and we got that constraint violation exception.

So what we are going to handle it now.

So we are going to handle constrained violation exception which is throwing find that are currently

using the global exception handler.

Right.

Custom global exception handler.

So let's go there now and then define our exception.

Right.

So which means like our first thing, what we do in general is.

A lot of.

Exceptionally constrained violation exception, so.

What we're going to do is we are going to define the method now.

Right.

So I'll see public financing and I will return by going to the response entity.

Object, right and handle it is going to be handled.

Constrained.

Constraint, violation, exception.

Right.

OK, so in constrained, why make an exception, so we are going to do two things here and handbill,

constraint, violation, exception.

So it's a constraint, violation, exception.

Yes.

And one modis.

Verb request, the request request.

Right, so now we are going to copy our standard two steps, which is nothing but our customer details

and the return to flight control C and control V, right.

And you did request that your description and my asked you to be straight, as I can say.

Is that right?

That request.

OK, so now what we are doing is in this constrained violation exception, we are going to set the date,

we are going to get the message, we are going to say request that the description falls OK, or whatever

we want.

OK, so if you want to give some message here, we can give that message directly, like saying that

in public works like a constant violation, exception, whatever you want.

OK, and then we're going to return those things.

What I appreciate is that request.

OK.

And then another important thing here is a direct exception handler.

And we need to define our constrained.

Violation.

Exception, not class, OK, and then it.

OK, so let me also say a control comment, you have to format everything.

So now we have completed a by mission exception related to a method creation and then handling it via

custom global exception handler.

Let me go to the postman and then post for the same thing and you can see it here.

OK, time stamp.

And then I got the message that Isabelita must be greater than or equal to one.

And then we also got the and that request OK.

So whatever we have before we have got it here, what we said yesterday, that message from that dismisses

details came for us.

OK, and the request that the description gave us this error details.

So this completes our implementation of constant violation exception with the global exception handler.

So just to reiterate, what we have done is we went to the control earlier and further.

That was a very idea matter.

We added for variable, a direct one, OK, and then at the user controller level, we added the annotation

validated and then we have tested it and we have got there has to be 500.

Then we went back to an exceptional year and then for custom, custom, global exception, handler plus

we have created a new method, handle, constraint, violation, exception, and annotated it with the

exception handler and the constraint violation exception class under this and then tested it.

And then we have got the response body, whatever we have defined and the status quo as 400.

So this completes the constraint, violation, exception, implementation.

So the next lecture, we're going to focus on a list controller and things like this O controller advice.



Until then, bye bye.


### Step 47. Step-06: Implement Global Exception Handling using @RestControllerAdvice.md
Welcome back in this letter.

We're going to implement a global exception handling using this controller advice.

So in previous actions we have implemented using the controller advice and now we're going to implement

it.

It's a superset wrest control of advice, which is a combination of controller advice and the response

body.

Let let's see the steps which we are going to perform for this respectless zero.

OK, so in the exception here, we're going to go to the custom global exception handler and then come

in this country.

Sanitation and best to ensure.

Controller advises not in action, forget user by user name because so we have to find good usable user

name with the user name, not one exception from controller advice.

If this is commented, then you'll get from standard spring with five hundred.

Right.

So let it come.

Okay, so once that comes, then we're going to handle that using the best controller advice.

So what we're going to do is we're going to create a new class customised controller advice exception

handler.

Again, this is also one more global Lochley.

So I can even see custom global little bigger class name, but that's fine.

Okay.

So I can even say a little more custom.

OK, so I'll set global to controller radwaste exception handler OK.

And I'll annotated with rest controller advice and I will handle user name not from exception inside

this, a method not from annotated with the exception handler and then also add the response status

for forever and then tested where Posman.

OK, so let's do that now.

OK, so here when we are doing this, when we come in, this will test you at once.

OK, so let me go back to the postman and get a usable username.

Right.

So if I send it.

So this is coming from our controller address currently.

You see that the message is that obesity and then the set of details, timestamp and the message, this

format and four coming from our controller advice, let's go back to our controller advice and then.

Come into doubt.

OK.

And then.

Sue.

OK, and then I get tested, get user by user name.

OK, now find it in panel, set back our format now.

OK, but the other message coming from our was a name, not from custom exception.

Right.

So this looks good to hear.

Now what we need to do is we need to define our best controller advice, OK?

So let's go back to our.

This one called this new globalised controller advice exception handler and then.

Go to our exhibitions package and say, create a new class and then use this name and then finish.

If you see here, there is no extensions.

Everything OK, so I'll see a rest controller advice and then come on shift.

Oh, important, good.

So now what we need to do is we need to define our.

Method, OK, for user name, not for exception clause to handle.

OK, so what I'll do is like.

Oh.

Public, so our response has been for customer messages is customer details, right?

This is the response been OK, so I'll say customer.

However, details and my method name is.

Username, not phone, I'll say like this, OK?

And inside this will have only one thing, OK, user name, not from exception.

Right.

And then Eakes.

And open the metal.

OK, so let's put another written statement, no issue, OK, so we'll see.

Little new customer details, we need to send three parameters, right, so one is.

You did.

And the second one is, I can say something like from it, did it just to ensure that this is coming

from West controller advice, OK?

And not only is my message in general, I just I'm writing something here.

And so you start.

Good message.

OK, so.

And if you see here.

OK.

Also improved the.

Java, you did good.

So now let me save it.

So here we are.

Good.

What we are saying is we have defined a user name, not from class, OK, method, and we are returning

some details for that exception.

So another thing important is to know we didn't perform two things.

One is the user name, not one exception occurs then this need to be filed.

To do that, we need to set an exception and let.

User name, not from exception, that class, right?

So come on.

You've got to import exception handler thing, OK?

Now, another thing is so far it is good.

But another thing is we also need to say send our response status.

Right, so we can send it using response status.

OK.

And come on.

You've got to import that.

And another is actually DP status dot not form.

OK, so now this completes our risk adverse implementation.

OK, so whenever a user name, not the exception is drawn immediately, the message will be triggered

from this controller advice.

OK, so let's go back to our postman and then send it.

OK, if you see here now from this controller, it's not fun.

We're getting it from the rest controller.

OK, so this completes our list controller implementation for user name, not for an exception.

So let's go back to the steps and then reiterate what we have done.

OK, so what we have done is in the exception we're forecasting custom global exception handler.

We have commented that the controller advice and then.

We went back to the exceptional layer and created a new class global risk exception Handler annotated

that class with the rest controller advice and then implemented a new metaphor username, not for an

exception, OK, and then annotated it with the exception handler and provided a username not for an

exception, Kluster, and also annotated with response status and then said that is not phone and then

posted via Postman.

And then we got the expected results.

So this completes the list controller advice implementation tool.

OK, so we have successfully completed a lot of things from exception handling perspective.



Until then, bye bye.

Thank you.


### Step 48. Step-07: Switching between @ControllerAdvice and @RestControllerAdvice.md
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

