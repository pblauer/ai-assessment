Mar 20, 2026
Ai Accelerator: Full SDLC with Devin  - Transcript
00:00:00
 
Pablo Blauer: All right, there we are. All right. Um, so welcome back again everybody. Um, as happy Friday to everybody and this is another session of AI accelerator with how forte uses AI sub sessions as well. Um, but essentially today we we we we bring a very great example of usage uh in in all the SDLC.
 
 
00:00:31
 
Pablo Blauer: We we'll review that in a moment. However, to do a very brief again recap on on what's the goal here is for everybody, you all are actually welcome to to bring more ideas and to share your experience as is going to be sharing today. Um the the idea is to share how we use AI. This year I think we are focusing on how to use it as a team and how we can empower the whole team rather than individuals. But that's the the main goal of of these sessions and to share how we use it so that other ones can start using the same tips and and and and best practices like that that we share here. Again, it's not uh regarding a specific tool. It's it's only how how we use it and and then of course tools will vary depending on every client uh that we that we have. One small another additional uh comment that I have is um at Forte we are um launching I think you probably saw this um a a a paid AI certification.
 
 
00:01:38
 
Pablo Blauer: There are certain training courses that that you can do and we really encourage everybody to to to be going through them and get certified. And I guess the the latest and most uh probably uh hot topic is also that we are trying to to work on a partnership with Antropic. And for that uh we we are going to be uh specifically highlighting the need of certifying certain uh entropic courses that that that you can see here listed there here. Um you will of course uh you already got this information from HR the the below ones that are deep learning IBM and and Google cloud. we are now adding this entropic target so that everybody can can get whatever level you are. I mean you have levels for for for everybody there. Um so so yeah I encourage you if you if we have delivery managers here please encourage your teams as well to certify um uh on on one of these specifically anthropic because we are trying to build this partnership but at the same time uh with these other one that are paid and and we can work on on covering that from our side.
 
 
00:02:45
 
Pablo Blauer: Having said that, uh you will see here um a link with all of the training courses as well. But um but yeah, let's let's uh let's dive into the today's topic directly which is um Slava from from lender uh who will show how he uses Devon uh to handle uh all the SDLC essentially. You will see he has shared with me examples. he has given me an early demo of what this session will be and and it's really amazing how everything um is used with Devon. he he will share best practices on what to take care uh what what what is working what is not and and essentially it's it's is going to again as I was saying it's it's going to be through all the SDLC requirements documentation code analysis of course implementation as well uh and and even technical depth right that that that is sometimes hard to to find solutions to to to old legacy problem um so with at I want to here want to welcome again Slava uh our uh delivery manager there at lender. So, welcome SL.
 
 
00:04:00
 
Pablo Blauer: Take it on.
Slava Vlaskin: Yep. Yep. Thanks, Pablo. Uh hello everyone and thanks everyone uh for uh for joining today. Uh let me start uh like I actually have a lot uh to describe here but uh I want to start with the basics because uh we living in a world where there is a lot of new instruments uh new instruments appears uh like every week every day and there is a lot of uh it is very hard to uh take a look at everything. So basically uh what is or even who is Devon? Uh Devon it's actually a bit old tool from if I remember correctly 2023. Um they are um Cognition is the company behind that and they are actually position Devon not as a tool but as a uh engineer like real person real teammate. Uh I'll get into much details soon. Uh but really uh what is Devon? It's basically a set of virtual machines that can uh execute anything. Basically, I want to start with a very brief uh overview um starting from the architecture.
 
 
00:05:36
 
Slava Vlaskin: So, basically um Devon uses uh anthropic load models. uh there is a variety of them uh and they also use uh their own orchestration. Um basically we can say that uh Devon consists of two big parts. It's brain it's all related to the large language models uh and AI and that box it's all related to execution. Um really that's almost it. Uh one thing I want to mention here before we uh will go uh next is uh actually there is kind of tricky situation just because um there can be security uh concerns here just because uh Devbox is a set of Ubuntu virtual machines. They can run at own uh virtual uh private cloud but brain will always exist in their propri uh in their own uh cognition cloud service. Um I'll get into much details uh in the end but really that's all we need to know uh before we'll go to the uh actual overview uh about dev usually how it works uh we are just assigning some work to the dev via I don't know via chat via slack via discord even um and it starts planning.
 
 
00:07:25
 
Slava Vlaskin: It writes code. It plan requirements. It even propose requirements. And all you as a developer, as a tester or maybe uh product owner, all you need to do is carefully review what uh was produced and finally merge it, approve it and so on. So um I think uh Pabla I can share my screen now uh and give you Mhm.
Pablo Blauer: Yep.
Slava Vlaskin: and we'll give you some real world examples. So um as I said uh Devon it's kind of old technology it's old product. Um recently we had a lot of great tools like uh clo codes uh uh open AI codeex and there is a lot of them uh but really because Devon was uh it may be three years old it has a lot of very useful tools basically a lot of things that you need to uh that you need to configure uh with cloud code for example it's already built in into that so you like will not lose a time to configure it um let's start with a simple one with a simple example all you need to uh like start using dev in your project is uh just u connect it to github to gitlab to any um to any other uh version management system.
 
 
00:09:20
 
Slava Vlaskin: Um let me quickly uh share it with you. I have some uh example here. Uh basically Devon has all access to all of your repositories to all of you uh task tracking system to all of your documentation. Um I will not spend too much time on that it's kind of a lot of integrations available here but one thing I want to show you right now uh is we right after we are connected uh Devon to all of our repositories we actually have out of the box we have full technical documentation. It creates it by its own. Oh, I'm sorry. Let me reshare my screen. Um, sorry for confusion. Finding the right window.
Pablo Blauer: Yeah, all of those integrations are also something easily integrated with Devon as you were showing me. It's oral like uh comm in conversational you integrate tools conversationally. So that's really useful as well and and reduces the barrier.
Slava Vlaskin: Yes. Yes. I'll I have that part two to share with guys.
 
 
00:10:59
 
Pablo Blauer: Sorry. Sorry. I saw you.
Slava Vlaskin: Yeah. Yeah. That's fine. uh so basic okay thanks uh what I'm talking about so right after you are connecting uh your repository you right away will have full technical documentation like we all know that documentation all um often is obsolete we need to spend a lot of time to support it uh I can probably Do I zoom zoom in a bit and what we have here uh we have all the diagrams all the technical description based on a real state of the project it generates it uh via its own internal tools uh it uses I don't know a markdown format for that so it's easily sharable uh I will not again get into much details but here we can actually see the full description the full description of uh of that project from the technical standpoint like it automatically determines our runtime our frameworks uh other technology used and so on so on. It also analyzes uh analyzes dependencies. It also uh just for example it also um like understands our uh architecture our design.
 
 
00:12:35
 
Slava Vlaskin: Uh so as I said uh one thing I need to do to uh achieve that is connect a repository and it will be fully automatic. Um obviously yeah there is a there is some kind of uh limitations here. Um they are not um they are not scanning our repository after each commit. Uh basically as far as I got they um they update that documentation uh once a week but we can obviously force it. So that's just regarding the documentation. So that's uh this stuff is fully covered by that. Uh one interesting thing here is they have uh again builtin uh kind of knowledge base I can say uh based on all documentation based on all real code uh it can uh it can answer your questions regarding code regarding business logic regarding actually anything it also points you to exa uh to exact lines I don't know to exact use cases uh two exact test cases so basically what I can say if um if you will connect devon to any tool you use uh I'll uh talk about it uh in few minutes uh you automatically will share all that uh context with him and you can use it as you want.
 
 
00:14:29
 
Slava Vlaskin: Um very quickly I want to show you like available integrations. It's pretty basic actually GitHub, GitLab, some Atlassian uh integrations like for example Jira and Bitbucket. It seems like pretty limited uh pretty limited set of integrations but the great thing is that uh Devon supports MCP as any other tools. So new integration becames like pretty easy like just for example we maybe a few days ago enabled integration with our database and Devon automatically again understands that okay if user wants me to check some data obviously not in production but in some uh test environments it can automatically access it and you even don't need to like remind him about this ability. uh a bit maybe maybe the last thing I want to mention is again as as any other tool uh it supports knowledge um knowledge it's kind of set of it's kind of system prompt um our team currently is um improving those knowledges uh and uh we are adding them bas basically on demand. That's it regarding like overview. I provided you just a general information right uh about what you will see just uh just right after uh integration.
 
 
00:16:18
 
Slava Vlaskin: uh let's probably switch to the more interesting uh more interesting use cases and I want to share with you uh a session uh from our product owner um we are starting to talk about SDLC uh and the planning and requirements um so let's uh I will not again get into much details of our specifics. But let's say that we just have an uh a request from our customer that we need to uh improve our notification system. Uh currently like situation in our project uh following that we have uh notifications uh in many parts of our system but they are not structured. They are not generalized. U you can see um hit a sec. You already see like a lot of messages. Uh really a lot of messages. It's a long session. But what exactly happened here? Our P started to plan those changes uh those necessity of not of single place of notifications in our platform. um and also asked it to provide some architecture for that like uh business requirements and uh technical requirements.
 
 
00:17:57
 
Slava Vlaskin: Um again there is a lot of uh there is a lot of text but uh after few rounds of um detailing some requirements of questions uh and so on so on. We've got actually uh it's it's an obsolete version so uh it's okay to share it with you. We just got a lot uh we just got fully documented solution with the uh with everything we need from the business perspective to the technical perspective. Uh I can briefly like really briefly show you it's business standpoint. Um it automatically uh I mean Devon automatically analyzes our system. uh created a migration plan and most importantly created a new requirements. Um it provided let let me find it. It provided uh like life cycle of notifications like what will happen when notification will appear? What will happen if user marks it as read? Uh how persistent should be uh these notifications. It also provided a uh like again you see a lot of uh information here but it also provided wireframes for that like design solutions based on shared with it uh design system sorry one sec.
 
 
00:19:47
 
Slava Vlaskin: So again uh I don't want to spend too much time into specific uh decisions were made uh but we can say that our pure uh by himself with help of Devon created really big epic based on just uh messages in chat. Um again a lot of context here, a lot of wireframes, a lot of uh technical solutions. Uh here we have another document like really architecture. Uh it's a technical specification all within one session. Uh most importantly and this is like uh most interesting thing here as I said uh we have a lot of uh we have a lot of integrations uh with the Devon. So basically what Devon did as a next step it created we are using laneer as um uh um as a task tracking system but the next step was to create an epic to create a project with all that information with all the schemas with all the uh design and technical solutions. We will not stop on that. It also created all the issues. Team basically right after that just need to uh just need to take it into work.
 
 
00:21:29
 
Slava Vlaskin: Uh again like um a lot of information provided here. Obviously important thing uh and I will repeat it multiple time in my uh in my speech. Obviously all of this needs to be carefully reviewed by the app by the developers um and all and all parties I can say. So that was
Pablo Blauer: uh one question there because I that's an important note a highlight
Slava Vlaskin: yeah
Pablo Blauer: to everything must be reviewed and now that you are showing here for example the acceptance criteria I wonder probably you and product owner are are the ones that are reviewing this as well from the technical aspect as well uh how many I I see that it created a lot of tickets and so on but uh what is the level of accuracy in general with the acceptance criteria in of course I got I got filling right not asking for metrics but
Slava Vlaskin: Um yeah yeah yeah sure um I probably will not give you an exact number of level of confidence right but I can say it is acceptable uh really uh from my experience and from experience from our pure from our product owner.
 
 
00:22:51
 
Slava Vlaskin: Um, it got the most the majority of things right. It doesn't hallucinate if you uh if you for example ask it to verify its own work maybe in another session. uh we are still um let me rephrase it probably we are still uh in the middle of the process uh of integr of adoption of devon right uh basically what happened uh like I do it myself I know that uh every de not every but developers uh do it and uh our product owner do it too right after implementation It's really very helpful I mean implementation of functionality or implementation of requirements I mean creating a requirements uh it is a good practice for us to ask it to ask Devon to verify uh its own uh outcome. I can say that obviously there is uh as it's LLM based right it obviously can hallucinate but we are trying to create a pipeline for everyone uh with the important steps like okay you generated a requirement we start new session for the uh for the verification of that but again in general if uh you give it clear instructions it will follow it in majority of cases.
 
 
00:24:46
 
Slava Vlaskin: Yeah, obviously review is required uh is required and uh um not optional we can say. Uh yeah and of course as I said uh Pablo you noticed it right that really there is a lot there is a lot of issues and uh right now we are trying to adapt u to that new process just because like there is a really uh LLM likes to produce a lot of text we are trying to suppress
Pablo Blauer: Yeah, I I I imagine it's also hard you have a hard time reviewing all of this at the same time,
Slava Vlaskin: Yes.
Pablo Blauer: making sure that everything is is okay.
Slava Vlaskin: Mhm.
Pablo Blauer: But at least it gives you a full backlog that then you can start You
Slava Vlaskin: Yes. Exactly. Mhm. Again like if we will uh switch to the to that original session like we all see
Pablo Blauer: see?
Slava Vlaskin: that it is really uh it is really long. So a lot of text needs to be reviewed, needs to be verified. Human work will not be cancelled by that.
 
 
00:25:59
 
Slava Vlaskin: But again um if we are comparing it to the like uh classical uh requirements creation or uh uh documentation creation. uh it just has uh it it just happens a lot faster than uh then create I don't then set up I don't know few meetings uh collect all the requirements from uh all the knowledge most importantly all the knowledge from uh all the parties uh actually again Devon has an access to code and that's it he can answer any your question uh Ah, yep.
Pablo Blauer: Jav Javier, you had a question or was just mistake.
Javier Acevedo: Surely it was a mistake.
Pablo Blauer: No worries. No worries. Yeah. And and what I was what I was thinking Slav as well because it produces a lot and especially in the product definition uh an architect a person a human in the loop should be there to control that is not uh goldplating or overengineering things or you know maybe we as humans sometimes we try to do it the the MVP the most uh short version to to to try to see if this works or not and and that strategy also needs to be
 
 
00:27:19
 
Slava Vlaskin: Yes. Mhm.
Pablo Blauer: controlled Because if it gives you a thousand stories to build a login, maybe it's like probably too much.
Slava Vlaskin: Yes. Yes. Totally agree. Like really uh that's that's an important thing. we cannot get rid of it at least for now. Okay. So, uh again uh this was just uh like an example of how a single product owner can plan uh can plan uh the whole new feature here. Uh, I want uh you can ask questions. Uh, but I want to switch to the really um to the really helpful from at least my experience uh topic. Uh it's um it's actually how developers and how development team can use it. Uh before that um I want to show you uh how we can add new integration to the de um a brief information we are using as a devops for our CI/CD processes right and uh Azure DevOps just don't have its own MCP server so basically we can't connect it in easy way as I thought uh but as we And see here I'm asking Devon how I can teach him to use Azure DevOps action.
 
 
00:29:03
 
Slava Vlaskin: uh it provides me a plan and uh this is uh removed key so uh removed token so everything is fine but really what happened here he created a plan how he can act how it can access uh our CI/CD logs uh our pipelines logs I just provided uh I just provided him uh token for that it saved that token as a secret and uh basically that's it and it just created a knowledge for himself that now he can access our uh CI/CD pipelines. So that's how it simple in most cases. Um again this is just an uh just a um how to say uh just very simple and very quick example but uh again you can use it uh you can use it um in whatever area you need. Just for example uh we need to integrate Figma. Uh you can just ask Devon how we can integrate Figma. uh and give uh give it context uh it will say that actually I have uh support of uh MCP and it will configure everything automatically. Again a small uh small glimpse here.
 
 
00:30:40
 
Slava Vlaskin: The most uh fascinating thing I want to share with you uh is dealing with the really old technical depth. Again, a bit of um a bit of uh information about our project. We used uh we are using Azure and we have several microservices that still uses obsolete Azure functions. Uh really this is very migration from one technology to another technology is kind of pain always. Even if we have uh even if we have a great architecture uh great separation of layers uh and so on so on uh it just consumes a lot of time from the developer to go through for example uh 200s of methods of end points and um just rewrite it basically what I've did uh and we've did it actually multiple times in the in the previous week. Uh we had a bunch of u such obsolete uh projects we've just created with Devon. We've just created an issue in line task in line uh to do a migration. it automatically based on our uh discussion with him uh with it uh it automatically like determine scope uh I asked it to validate uh every requirement and that's it what happened next I've just asked him to uh implement that task in parallel mode uh it's kind of new functionality.
 
 
00:32:44
 
Slava Vlaskin: It it's appeared maybe a week ago. Uh we can say that this is uh that this is kind of agent swarms. Um I just provided it a link to the issue and asked it to plan uh implement and verify it. It created a bunch of um a bunch of sessions and we have here what we have here is advanced session. It's kind of orchestrated uh for that and then magic actually uh happened. It created um PR uh pull request in our GitHub. You see amount of lines. It automatically tested it with already existing uh API tests and basically again provided all the information all the cavits all the unclear questions within within that session. I gave it uh I gave it an answers. Uh and all I need to do right now uh is just test it locally and measure it. And from my experience because I uh I've did that without dev myself uh maybe a year ago or so. I've spent like really maybe several weeks for that. This is achieved just in hours and uh like with with that repetitive but well scoped work, Devon works really great.
 
 
00:34:48
 
Slava Vlaskin: like we really uh based on a tech depth we can see uh um we can see only positive things again obviously it will have a mistakes I always u um I always uh ask it to verify those things uh multiple times uh when I uh I actually want to uh work on that right after uh our demo uh I know that when I uh pull that branch locally and start all the development on the uh start uh on the development uh and testing. Uh I know and I expect that there will be an issues but all I need to do is not manually verify every point. I can just ask it to uh for example generate API tests to cover old solution and new solution and find any find any differences in uh um in logic. That's it. Um so yeah again we can see how many end points how many end points were covered by it. Uh yes.
Lee Barnes: the the example here is uh technical debt at the code level. Have you tried addressing any architectural level
 
 
00:36:20
 
Slava Vlaskin: Mhm.
Lee Barnes: technical debt? Uh you know maybe poorly decomposed services, tightly coupled components, other things that are uh you know would be more difficult for example for a you know a junior developer to uh to address.
Slava Vlaskin: Yes. Yes. we had that experience un unfortunately I didn't prepare the session uh but uh you actually uh raised a great topic because um how I can say it um just because uh developer or I don't know or technical lead or someone who start that session needs to fully understand what it tries to achieve. Usually how it happened with examples you asked for um when our experienced developer knows that this code smells uh it uh he um asks Devon that okay I have a problem here. I have very tightly coupled uh modules for example. Find me a ways how we can how we can decouple it. I cannot say that really it works incomparable level of simple repetitive work. uh but if you uh try to I don't know discuss proposed solution with him maybe add a bit more details maybe say that no it's not uh it's not a good solution uh this is achievable to unfortunately again I just don't have such example here uh and trying to um trying to provide like generic a very generic response.
 
 
00:38:35
 
Slava Vlaskin: Sorry, didn't prepare for
Lee Barnes: Oh, no, no, no, no. Thank you. I think my my thought process was that maybe it it couldn't address the architectural
Slava Vlaskin: that.
Lee Barnes: level that uh and was maybe more well suited for the you know more mechanical issues.
Slava Vlaskin: Mhm.
Lee Barnes: So I just just curious if you had tried it on any more architectural level changes.
Slava Vlaskin: Yeah. Yeah. uh in general what we definitely have an experience like and I can show it a bit later uh we've implemented a new functionality with with it uh with the desired architecture but really yeah uh I can remember that we've tried to work with Deavian on some uh architectural tech depth let's say uh maybe will do in next few weeks. Uh Lucas, please go
Lucas Hendrich: Yeah. So, so thank you for this. This is a great presentation and um I I guess this might you might not have this
Slava Vlaskin: ahead.
Lucas Hendrich: information so it'd be a good followup um after, but I'm really curious about the economics of it.
 
 
00:39:44
 
Lucas Hendrich: I'm curious about how you're tracking token spend and if you're finding that for more complex features, you know, is it how variable is it and how are people controlling Like let's say let's say I I you know I make a mistake in my requirement, right? And this is probably more common with like one shot prompting and I go down a path and I've grown a bunch of tokens but I get a bad result. So I'm curious how how is all of that managed with Devon?
Slava Vlaskin: Mhm.
Lucas Hendrich: And I know that's a lot.
Slava Vlaskin: Um yeah.
Lucas Hendrich: I'm curious.
Slava Vlaskin: Yeah. Um yes, if you want uh go
Lee Barnes: Yeah, Ju just to just to follow on to that and that I had a very similar question.
Slava Vlaskin: ahead.
Lee Barnes: I know they have some normalized unit they I can't remember what it's called. Uh okay,
Slava Vlaskin: I see you. Yeah. Mhm.
Lee Barnes: ACU that substitutes for for token. So, just to to add on to what Lucas asked, um are you finding, you know, how um I guess are you tracking how much you're spending on on non-usable output, which I think is, you know,
 
 
00:40:52
 
Slava Vlaskin: Uh specifically right now uh no. Uh but really we actually started to discuss it with our with our client. uh just because like you absolutely right it can spend a lot of tokens. It can burn a lot of tokens uh with uh not with not desirable output. um Devon itself it uh provides a statistics uh and starting I think from our next sprint we've agreed uh with our clients that we will collect that stat for now uh we are kind of experimenting and adopting so there were u like our client wasn't specifically addressed uh financial questions but obviously yes obviously we will face it. Um regarding that uh just a bit uh just a bit information thanks for already like providing uh that info they are using ACU it's kind of uh their own units based on token usage uh based on uh virtual machine usage uh basically how um how I uh for example monitor it when session size became Excel like very large obviously we need to close that session and continue in other uh if I see that ACU usage is high too but I don't see uh but I don't see any uh valid results in my opinion uh there is always a chance that I will close that session and continue in another maybe with more again detailed prompt with more detailed requirements.
 
 
00:43:02
 
Slava Vlaskin: Um yeah, unfortunately cannot answer uh like from any stand from all points
Lucas Hendrich: Can can you yeah can you give just an example and it can be very rough estimate of what
Slava Vlaskin: here.
Lucas Hendrich: the monthly spend is for everything related to Devon just so we can understand what percentage of let's say a developer's spend is so is it 10% of what a developer would cost is you know so or is it so variable that it's hard to
Slava Vlaskin: I think yeah that's a great question. I think I cannot provide such info for now because really like first of all uh um I don't I just don't have that information.
Lucas Hendrich: That that's fair. it it I think that's that's the burning question is um what I'm finding when I'm just experimenting with different tools that that reaches a point at which you could almost imagine you know half of a developer's salary spent on tokens and that's partly because I think there's a lot of experimentation but also um the the token economics are I think are variable depending on the model too so so that's I know That's hard to capture but that's that's what I'm really curious about particularly a year
 
 
00:44:19
 
Slava Vlaskin: Yes.
Lucas Hendrich: from now two years from now as people get locked in at some point you have to make a decision and stick with a tool set just you know for enterprise reasons then you know once we become captive to let's say claude or or you know name whatever foundation model then you know the price is going to be extremely sensitive that Makes sense.
Slava Vlaskin: Yes, totally totally agree. Um, yes.
Lee Barnes: Just just real quick to Lucas's point about, you know, spending tokens uh without any value. Are there things that you guys have realized, hey, Devon does a really good job at this and it's it's worth the token spend. These types of tasks and then there's other types of tasks you found out that yeah, the you know, typically the output just isn't very usable. Um and you're starting to avoid those things.
Slava Vlaskin: Mhm. Uh actually yes actually we have some uh outcome from like our discussions. uh what really uh we can say where uh Devon is really great at and uh people actually start to uh not do such things manually.
 
 
00:45:43
 
Slava Vlaskin: Uh I have like two real uh real examples. First example I already showed you. It's all related to the let's say um to the maintaining to the really uh long repetitive work. Devon not spends a lot talking tokens. Uh it again uh thinks about uh maybe maybe half of an hour and implements everything within each repository. That's really big win. And I want to mention uh another um I want to mention another uh like really well recommended usage. It's a box. It's finding uh finding uh causes for the bugs. Uh because it understands code perfectly uh for for it to analyze the code and to find the place where buck has happened. Uh it costs nothing. It just use uses a lot of searches. That's it. Uh and uh I will um I will need to speed up a bit because we have only 10 minutes. Uh I have um I really have a final slide uh when I can show you team's dynamic in terms of story points and velocity.
 
 
00:47:14
 
Slava Vlaskin: Um okay, let's try to quickly continue. Uh I'll I'll try to be short here. Uh just another example. Uh it's regarding the bug. I uh we found the bug for um uh we we found the bug in one of the our functionalities. Uh all we need to do uh is ask Devon why uh why it's happening and how we can fix it. like really it has uh only 10 minutes to think and to propose solution. I provided him some answers and it just implemented again new PR request here with the code. I mean u that's kind of uh right after PR creation uh obviously uh we need to do we still need to do manual things we need to review we need to merge it uh and so on so so and probably I think it will be um again just small example of uh how Deavian uh like how to use Deviian more efficiently I think is just for example testing I'm not talking uh right now about uh the full quality processes uh because we are still in the middle there is a lot of uh decisions needs to be made but it's again really great to increasing coverage for the development work I mean for the development uh for the testing uh that um depends on developers I'm talking about integration tests API tests unit test that's really great like just for example we had a flaky tests um it analyzes it and it provided uh
 
 
00:49:29
 
Slava Vlaskin: provided a solution and again PR and merge Um the last thing uh I think I want to show you it's again it's just um uh it's just um uh example of Devon itself of their product. Uh because like what I've showed uh today is more about you know this is the chat we can discuss some issues in that chat with uh with Deon. But really I um I'm I already provided an info that actually Devon uses a virtual machines and uh in some cases you can see uh result uh right through their um uh through their web interface. Uh give me one second. Uh it is just an example really small example. For some reason I've decided to change uh I've decided to change uh color of our heater. That's one of our application uh deaf environment. Uh we have a blue heater. What I as what I've asked him uh is sorry uh is just to make it red. and what I can do with it. And this is really helpful for some test for some use cases.
 
 
00:51:03
 
Slava Vlaskin: Just for example, for UI perspective, we can ask uh it to uh start test session and what it will do uh it will uh run our application in isolated mode. Uh maybe it's it um I think yeah it's go to sleep. Um, I can ask him to uh no ah okay uh yeah great timing uh because Daven is centralized platform right and we're not using our own uh VPC sometimes we are experiencing uh degraded performance because of high usage. So unfortunately I think I will not Yeah. Yeah. So uh it's a dead end. Um will not show you it but really you can ask Devon to for example u set up that environment uh and it will give you private link to test your application. That's I think it one important thing I wanted to I wanted to uh describe. Um Pabla I want I will stop sharing. Can you please uh share the presentation again?
Pablo Blauer: Yeah, give me one second. And you want to see the takeaways?
Slava Vlaskin: Yeah.
 
 
00:52:51
 
Pablo Blauer: Uh,
Slava Vlaskin: Uh yeah. Yeah.
Pablo Blauer: there you are. Oh, no, I'm not sharing. Hold on. Ah, there you are.
Slava Vlaskin: Okay, thanks. U so I want to wrap up our demo. Um yeah, uh I want to wrap up and uh uh provide you some takeaways from our usage. Um again as any other technology it's not a magic button if you are using uh if you are providing it clear requirements uh clear description and carefully review it uh you really can achieve uh like impressive things again with all the tech depth that I provided um already said about it uh that repetitive and well scoped work uh works the better. Uh one thing I didn't actually mentioned but I want to mention it right now uh that um Devon is kind of fully agentic and what we really can achieve here and what we already achieved uh in our team is work parallelism. So you know when you for example opening and testing your application uh let's imagine that you found some not very beautiful behavior or maybe some wrong uh maybe some bug instead of instead of just uh creating an issue in your task tracking system uh you and I see it uh by myself.
 
 
00:54:52
 
Slava Vlaskin: I see that other guys from our team started to use that approach. You are opening new session in parallel mode and ask Devon to analyze it maybe to create an issue uh to uh finally fix it. So really mindset needs to be changed a bit. Um again super uh super generic information that yeah it already like embedded uh and I showed you how easy uh DN can be embedded in workflow just connect everything you need and uh basically you have a great outcome in terms of documentation and uh all other things. again want to mention a security um just because uh again there is no ability to self-host it uh but it's uh SLC2 certified and for enterprise plan VPC is uh available um again major uh major disclaimer major u highlight here that uh LLM still under the hood. So, hallucinations happen. Uh, it actually I saw it myself multiple times. It actually forgots what you sayed like five minutes ago in the same session. That's why like maintaining and u checking session size, tokens usage uh and everything else is really important.
 
 
00:56:35
 
Slava Vlaskin: And again the main the main thought here is human review is not optional in any case of uh in any use case in terms of requirements in terms of architecture and in terms of code itself. Um that was it from my side. I think
Pablo Blauer: Yeah. Yeah. Uh that was great. Uh Slavas, thanks for this. And yeah, you you bring something that is really important. Usually the the context in the long sessions usually you exceed the available tok the available context and yeah some context management some compacting uh of the sessions needs to happen there. So but but yeah it's something to to take into account. Yeah, great uh insight presentation Sava. Thanks for for sharing uh this uh way of working with Devon which I think uh to my knowledge you are the only team working with this but it's it's great to see that it's happening
Slava Vlaskin: And thanks everyone.
Pablo Blauer: right
Slava Kreynin: Uh SLA great presentation. Uh I have a question to bigger team if anybody else wants to try Devon.
 
 
00:57:47
 
Slava Kreynin: uh maybe we can explore it on internal projects or on there with obviously with client permission uh introduce it so we can share the experience and also I know Slava specifically I'll will talk with you separately testing that's a very painful issue right now because on the other side of all the hallucination and all security risks then testing so if you can mitigate that and perhaps maybe somebody on our bigger team can help you deal with issues you currently deal with in testing but I'll speak to you about it separately.
Slava Vlaskin: That's
Slava Kreynin: So again if anybody wants to uh interested in using it and I know there are questions about the cost reach out and
Slava Vlaskin: great.
Slava Kreynin: we'll discuss it. It's cost is substantial not to be ignored. Um for my experience and I talked to uh lender management a little bit it's probably about just to give you an understanding probably about you should on the safe side assume it's 20% of what development cost it might be a little bit less but 20%. So whatever the cost of developer is time right assume 20%.
 
 
00:58:55
 
Slava Kreynin: of that will be in token somewhere you know uh it's usually less but again hallucination over overuse reuse etc so budget about 20% that's what I've heard I know it's very early to truly summarize it
Pablo Blauer: that's becoming a kind of a standard from the community metric or something like that. Cool. Good to know. Yeah.
Slava Kreynin: okay thank you this was this was this was very very good and yeah uh let's you and I let's side of
Slava Vlaskin: Thanks.
Slava Kreynin: this thank you thank
Slava Vlaskin: Sure.
Pablo Blauer: All right, that's a wrap. Thank you everybody. Have a good Friday, good weekend, and we'll connect next time. Thank you.
Ihor Leonets (Igor): Thank you.
Javier Acevedo: Kiss the most.
Ihor Leonets (Igor): Thank you.
Pablo Blauer: Bye.
Slava Vlaskin: And I think has a question.
Pablo Blauer: Oh, sorry.
Lee Barnes: Yeah,
Pablo Blauer: Did not
Lee Barnes: just just real just real quick um uh to kind of uh pile on to Slava's point about uh using it elsewhere. I guess I have two two-part question.
 
 
00:59:49
 
Lee Barnes: First one I easy one. Have you noticed any changes into your in the quality trends uh uh of the application either positive or negative?
Slava Vlaskin: Um yes I can answer right
Lee Barnes: Um
Slava Vlaskin: away. Yes we've noticed uh yes we noticed negative trend actually uh but uh really uh like as Slava mentioned uh we have some struggle right now with testing and quality uh perspective. I really uh I cannot give you a clear answer what uh because of what it happened um because of AI or because of hidden changes
Lee Barnes: Okay.
Slava Vlaskin: that happened in our project too. So yeah need to need to understand
Lee Barnes: Right. Yeah,
Slava Vlaskin: that
Lee Barnes: we Yeah, I'd be happy to to talk to you about that. And then on a related topic about other teams using it, um, Alex Lucvich and myself are looking at essentially playbooks for implementing, uh, AI within the SDLC, not specific to any tool, uh, but general. So let I'd be interested to you know understand your learnings um uh and certainly specific to Devon as other uh groups uh hopefully get to try it but just general uh to see what alignment we have with you know some of our uh thoughts and
 
 
01:01:19
 
Slava Vlaskin: Sure.
Lee Barnes: findings uh to see if it it aligns at least at a conceptual level uh with what you're doing at Devon. So uh Alex and I will reach out on that as well. But thank you. This is awesome.
Slava Vlaskin: Yeah. Thanks everyone again. Uh also I actually forgot about the final slide. It's not uh yeah it's just a um like real uh real velocity increase. uh it's not made up like it's available in our lineer uh because of uh different uh processes uh but we can say that really we are seeing increase of our velocity thanks to AI thanks to Don specific and I think that's it from my side for sure All
Pablo Blauer: So this is comparing before Devon and and with David. This last final four sprit or 24 29%. Okay, cool.
Slava Vlaskin: right.
Pablo Blauer: Any other questions before I close it accidentally? Sorry. Yeah, John.
Jhon Calderón: Yeah. Hello everyone. Well, I have one question by by curious those uh functions that you mentioned you migrated from an old version to the new one.
Slava Vlaskin: Mhm.
Jhon Calderón: Uh those functions are in production now in the in the production
Slava Vlaskin: Uh yes yes yes some of them already in
Jhon Calderón: working. Okay.
Slava Vlaskin: production
Jhon Calderón: Have you had any uh production issues with those functions or not?
Slava Vlaskin: actually no like really uh just because we've tested uh we've tested
Jhon Calderón: Okay.
Slava Vlaskin: them a lot uh before uh before provide uh providing them before delivering them to production. But uh want to highlight that again um really uh because it is very destructive change uh we are paid close attention to verify that everything is work actually. Yeah. Uh almost as I said almost no problems uh were
Jhon Calderón: Got it. Thank you.
Slava Vlaskin: found.
Cristian Taborda: Thank you.
Jhon Calderón: May.
 
 
Transcription ended after 01:04:15


This editable transcript was computer generated and might contain errors. People can also change the text after it was created.