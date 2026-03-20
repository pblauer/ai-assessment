# Slava / Pablo - Lender/Devin 

**Meeting Date:** 24th Feb, 2026 - 11:02 AM

---

**Slava Vlaskin** *[00:00]*: Pablo. 
**Pablo Blauer** *[00:01]*: Hey. How's it going, Slava? All good? 
**Slava Vlaskin** *[00:04]*: Oh, yeah. Hope you're doing. 
**Pablo Blauer** *[00:06]*: How's how's Forty Life treating you? 
**Slava Vlaskin** *[00:12]*: Huh. So I think, for Pablo, I have very limited plans for today because, like, I think it will better for us to discuss our plan. Right? I can give you a brief overview what we've done in our team Mhmm. And how we can actually use them right now. Huge disclaimer, we are still in the middle of that process. Like, things constantly changes every day. Like, right now, when I'm talking about it, I have a few messages from our customer about all this process. Mhmm. Okay. So let me share probably my screen. Okay. I if you want, I can provide you I can share with you how we are using Devin in auto test in and in development. 
**Pablo Blauer** *[01:20]*: Yeah. I'm I'm interested in, let's say, in all of the SDLC. So whatever part you think is more viable to share, it's a good idea. And and, also, I'm I'm interested in hear your opinion maybe before you share if you think this is working or not because we spoke about, I don't know, twenty years twenty days ago, and this is something that you are starting. And Yeah. What what are your hesitances there? 
**Slava Vlaskin** *[01:47]*: Exactly. So let me give you, first of all, like, my brief overview of where Devin is good and what things needs to be improved. So first of all, I know that there is a lot of tools right now, like Codex, CloudCourt, any other agentic startup, and so on. What is the main difference with the Debian is actually almost everything works out of the box. Like, you don't need you really don't need to spend a lot of time to set up processes. Just for example no. Let me start from a bit different angles. So Debian is actively integrates with the different services. Just for example, it currently I'm sharing it with you right now. It currently has an access to all our GitHub repos. 
**Pablo Blauer** *[02:53]*: Got it. 
**Slava Vlaskin** *[02:54]*: So, basically, you don't need to do anything. You just you just set up integration, and that's it. Great. From this point, you can work with any repository. Just, for example, I'm showing it to you What Devin supports? First of all, it's it is great in the documentation. So when you are adding repository to it can I'm showing it to you. It can generate pretty good Vicka, pretty good technical documentation. Like, really good. I'm impressed. Just, for example, to show you so here is fully auto generated architectural diagrams. I don't know. Main concept, domain. 
**Pablo Blauer** *[03:55]*: And this is sorry to interrupt. This is automatically generated only by adding the repository. Sorry. Or what? Yes. The repository. 
**Slava Vlaskin** *[04:03]*: Yes. Yes. Exactly. Exactly. So, actually, main focus for the Debium, they are advertising it as a developer. So here. 
**Pablo Blauer** *[04:18]*: Mhmm. 
**Slava Vlaskin** *[04:18]*: Okay. This is just, like, a brief glimpse. So he automatically, without any, like, configuration, just click one button, and he generates really good documentation. More importantly, it is regenerates it. Basically, as far as I remember, after each commit. So documentation. 
**Pablo Blauer** *[04:43]*: Is up. 
**Slava Vlaskin** *[04:45]*: To date. Yes. Yes. Exactly. Next thing, I'm not even, like yeah. 
**Pablo Blauer** *[04:53]*: One question. This is from scratch. So you gave the repository, and it generated from scratch. Do you. 
**Slava Vlaskin** *[04:59]*: Know Exactly. 
**Pablo Blauer** *[05:00]*: What happens if you already have a documentation? Can it take it and kind of re. 
**Slava Vlaskin** *[05:09]*: That's a good question. That's a good question just because, you know, previously, we had previously, we had documentation placed in Azure DevOps in a Vicki. 
**Pablo Blauer** *[05:23]*: Yeah. 
**Slava Vlaskin** *[05:23]*: So, actually, Devin, as I say it works better with, like, repositories and Git, like, storages. I'll, I want to write your question, Pablo, a bit later because I have a great example regarding. 
**Pablo Blauer** *[05:49]*: Got it. 
**Slava Vlaskin** *[05:49]*: Regarding that documentation. Mhmm. What works out of the box? When our repositories are indexed, when documentation is created, you actually can talk to your with your code base. Ask questions so on. My opinion here is it works not really good. I mean, sometimes it answers perfectly, sometimes not so perfectly. LLM or LLM has similar issues with that. You can't be 100 sure. This is, like, only what I've showed you. This is just, you know, like, fancy stuff. The main thing here the main thing with Devin, and I personally like it, after using codex, you know, that, actually, Devin supports a lot of other integrations. Just for example, let me where it pays. What we have currently? It has official integrations with Slack, with Linear. Linear is our task writing system instead of Azure DevOps, and bunch of others. Right? 
**Slava Vlaskin** *[07:19]*: The main thing here is that Devon actually supports anything that supports API. Mhmm. I will show you how I integrated it to the Azure DevOps yesterday. So, basically, what I did, I just I just asked it that, look, I have a CI on my Azure DevOps. I have test cases in Azure DevOps. I have a Viki with the documentation. How I can build integration with you? It analyzes everything. It gave me an instruction. It asked me to provide personal access to terms. And more most importantly, it updates its internal knowledge for our organization. And with any request, with any session, with any new request to the dev end, it will know that we currently have an integration with Azure DevOps, and it can look for it can, for example, track, I don't know, status Mhmm. Or something like that. 
**Slava Vlaskin** *[08:39]*: So story for a bit maybe not organized presentation. 
**Pablo Blauer** *[08:44]*: But No. No. But I like it. I mean, it's sharing the real usage, And it automatically with natural language, you can configure the integration. That work that's what you're saying. 
**Slava Vlaskin** *[08:54]*: It's Yes. 
**Pablo Blauer** *[08:54]*: Yes. Almost you had to almost do nothing. Yeah. 
**Slava Vlaskin** *[08:57]*: And it works really with everything. We've tried actually crazy things. Not me personally, but our customer. He gave it an access talking to our production. We are not in live currently, so we don't have live clients. But if our customer gave it credentials to our APIs. Mhmm. Ask it, for example, to analyze our document types. Mhmm. For example, remove duplicate, create some add some important fields, and so on. It handled it perfectly. 
**Pablo Blauer** *[09:43]*: Yeah. 
**Slava Vlaskin** *[09:44]*: So anything that has an API or even better an MCP server works, like, without any configuration. 
**Pablo Blauer** *[09:57]*: Nice. 
**Slava Vlaskin** *[09:59]*: Okay. 
**Pablo Blauer** *[09:59]*: What is the you have licenses for all of the team, for everybody, or only for you or for management? 
**Slava Vlaskin** *[10:11]*: We have as far as I remember, we have a team plan. It costs about fifth $500 per month, and it has prepaid ACU. ACU is kinda kind of prepaid tokens. They have their own metrics. Actually, I'm, unfortunately, I'm not aware of all the pricing stuff, you know, because it's handled directly by our client. 
**Pablo Blauer** *[10:49]*: Good. Good. Good. 
**Slava Vlaskin** *[10:50]*: So, yeah, everyone really have an access to it. And let me show you where I think the most impact is applied to our team. It's actually with the writing code. So you see I have a lot of sessions. Devin actually operates with the session. Session is kind of, like, ChatGPT chat. 
**Pablo Blauer** *[11:24]*: Yeah. Yeah. Yeah. 
**Slava Vlaskin** *[11:25]*: Just for an example just for an example, today, a few hours ago, I needed some endpoint in our platform. I just described it that, hi. I want to export some entity from one endpoint to another endpoint. Sorry. From one environment to another environment. I know that we can do it. Please analyze the code and provide me a solution. What's actually happening what's actually happening here? He did all the research because he have all access to our repositories. Right? He proposed me a solution. Eight a sec. So it created automatically PR. I'm sure I will show you PR in one sec. No. Sorry. He create it created an issue within the our task tracking system with detailed plan, with detailed, I don't know, requirements and all other stuff. I reviewed it. And what happened, Max? I just asked it. Now let's implement it. 
**Pablo Blauer** *[12:49]*: So first, he give you the plan, and then it doesn't start implementing process. Good. Good. Good. 
**Slava Vlaskin** *[12:54]*: Yes. Yes. So you can fully control, actually. You can fully control it. So what happened next? It created just a regular PR. It's kinda configurable. We have data and AI integration as an active view. So it's committed all the code. I've asked it to make a review or each actually, it made review by himself. So, yeah, and I just merged it. 
**Pablo Blauer** *[13:30]*: Wow. 
**Slava Vlaskin** *[13:31]*: So from the development perspective, really, I can say, Pablo, that while we've started to use I mean, massively use Debian maybe two weeks ago, we see a lot of great results. We've dealt with, you know, with the technical depth that was untouched by the years. Right now, I I see that we are starting to shift our, like, not even as DLC, but our mindset that we can actually not create some PBI for future to resolve some technical debt. If you see something, if developers see something wrong in cold or ugly or maybe not with our common approach. I already see that entire team started to feed it to Devon directly if and fix it right now, not to postpone it for the years Mhmm. As it usually happened with the technical debt. That's from the that's from the development perspective. 
**Slava Vlaskin** *[14:51]*: Also, just, like, want to show you that you see it's, like, it's an agent. It constantly monitoring the situation. After he create after he created PR, it automatically started to monitor CI. It already, like, have an access to it. So it can I don't remember exactly where I have those sessions, but I saw that multiple time that it creates PR? PR is not often is not so good. Like, it's LLM. Right? But it's key that, for example, CI is failing. It starts analyze code again and finally resolves the issue. One important thing I forgot to mention is that, actually, Devin is not only the chat. Devin, actually, for each session, it creates, let's say, virtual machine. 
**Pablo Blauer** *[16:02]*: It. 
**Slava Vlaskin** *[16:04]*: Executes scope. It executes test in that local environment. I just, like, don't have right now something. 
**Pablo Blauer** *[16:17]*: And it creates unit test and so on. Right? So if we see if you go and see the PR, like, what has changed? Yeah. 
**Slava Vlaskin** *[16:25]*: Yes. Yes. Basically, like, as I say, Devin has organizational setup where you can manage where you can manage entire knowledge regarding, your workflow. More importantly, I forgot to show you it. It has, like, different section knowledge. Just for example, let's, let me show you. So knowledge is basically its manner. Right? 
**Pablo Blauer** *[17:01]*: Mhmm. 
**Slava Vlaskin** *[17:03]*: Basically, what we have here is that, for example, we have for the back end development, we have this knowledge of that direct Devin to use specific approach when working with your packages. So not always it follows those rules, but in most cases, That's from the development. Mhmm. Mhmm. 
**Pablo Blauer** *[17:35]*: No. No. This is very interesting, really. And what is the so I see that you generally use it for maybe tech debt or or small things. What about features or more or things that are more complex or, you know. 
**Slava Vlaskin** *[17:54]*: Exactly. Here is my here is my example from today because what a coincidence. I'm working on a huge feature right now. It's actually it's actually a tech debt tool, but we are transferring one of our apps. 
**Pablo Blauer** *[18:15]*: Mhmm. 
**Slava Vlaskin** *[18:15]*: From one technology to another, from Azure Functions to the AskMap. Let me show you just briefly. You see how much code it is. So it's not something quick. Yesterday just yesterday, we've got an access to the new feature. It's called batch sessions, but, actually, it's like agent swarms. What we can do what we can do let me probably show you. We can ask Devin to start batch sessions. Basically, what what it does, it creates one orchestrator session, and that orchestrate orchestrator session plan all needed work, start independent sub agents, and control them. So I've spent maybe one hour or so to guide it, to provide it answer because it's actually always asking some questions, some important questions. And then it prepares, like, it asks if I want to start that work. Right? 
**Slava Vlaskin** *[19:41]*: It started work, and just scrolling to show you, he it planned seven independent workers to work on those issues, and it's actually resolved right now. So I may. 
**Pablo Blauer** *[20:05]*: No. No. And and each worker, you need to go ahead and answer things? Or the main here, the main. 
**Slava Vlaskin** *[20:12]*: Main is our. 
**Pablo Blauer** *[20:12]*: Station is the one that asks you questions. Like, oh, I found, like, for example, I don't know, in dev eleven seventy, I found something that needs to be answered. So and it okay. 
**Slava Vlaskin** *[20:23]*: Artistrator session, main session is actually, like, the perfect way to. 
**Pablo Blauer** *[20:30]*: Right. 
**Slava Vlaskin** *[20:31]*: To interact with it. But, yeah, again, if there's any other. 
**Pablo Blauer** *[20:36]*: Yeah. How how does the team I'm seeing you as delivery manager doing everything from here. Like, how does the team work with this in terms of development? Are they doing PR reviews, or or how at what point they put in work? 
**Slava Vlaskin** *[20:54]*: Actually, as I said, Pablo, we are start like, we're experiencing serious mindset shift right now. Two weeks ago, it was really almost impossible to ask anyone to work with the veteran because, you know, it's new technology. Right? 
**Pablo Blauer** *[21:18]*: Yeah. 
**Slava Vlaskin** *[21:18]*: People not familiar with it. As I said, currently, I can stay following that our development processes in FDLC, like, from the getting from getting requirements to the, I don't know, to the CICD base. Almost everyone developer in our team uses Devin more or less. Someone still prefer to manually control it. Someone like me, I'm just looking through the code, maybe execute that code once. I'm in local machine. 
**Pablo Blauer** *[21:59]*: Mhmm. 
**Slava Vlaskin** *[22:00]*: And merge it. So I can say that development is covered by the 70% right now. In different, maybe, use cases, maybe from end to end, maybe only just for code review, but everyone uses it. Yeah. Currently, maybe just half of an hour ago, we've create we've made a session with our QAs. Just a bit of background. Our project doesn't have automated QA engineers. So it was really a pain for us for many years. What we are trying to achieve? We're trying to we're trying to force Devin to write autotest for us. So we are actually trying to cover testing. We are in very beginning in very beginning of that process because there is a lot of questions. Guys don't have an expertise in any coding. So they're just pure manual QAs. 
**Slava Vlaskin** *[23:25]*: But I think, maybe at the end of this week, we will already further results. I can actually try to, find an example for you just quickly. Sorry. 
**Pablo Blauer** *[23:41]*: No. That's fine. Maybe you can share in the next session or whatever. But my and my other question, I understand that you are trying to implement in automation. My other question is how do you decide what you do versus what you give to the team, the developer team too? You you see my point here? You showed me how Yes. Yes. How you did a simple that, export import checklist JSON. That's something you did yourself and seems to be something simple enough and so on. Like, what do you give your team to implement? 
**Slava Vlaskin** *[24:19]*: I have actually no one right now because it's too painful for us right now. You see, our project is a start up. 
**Pablo Blauer** *[24:29]*: Mhmm. 
**Slava Vlaskin** *[24:29]*: So we have our CEO slash CTO from the client side. He is generates ideas constantly. 
**Pablo Blauer** *[24:42]*: Mhmm. 
**Slava Vlaskin** *[24:43]*: Basically, how and we, for the big period of time, maybe a year or so, we had serious bottleneck with the requirements. Like, you know how it's happened. He comes to me. He comes to our other leadership leaders. And just personally ask them or me that I have an idea. Let's implement this, and that, and that's it. We currently definitely have a serious issues with the requirements. Because me, personally, I can make a decisions in our projects. You know? Other other leaders of our teams can do decisions too. But this is a big question for me. How developer without clear requirements or even QA without a clear requirements, how they can use it same way as I do or our leaders do. Ask answering to your question, what hap what's happening now? 
**Slava Vlaskin** *[26:03]*: I got a requi for example, I got a request from the from our client, and I really like, I'm starting to think, will I have time to do it or no? And that's it. Based on that, I've I'm implementing it by myself or I'm passing it to the team. Actually, one important thing here, team, obviously, has its own backlog. Like, we've had lot of planned issues. We started to get feedback from customers. So for better understanding for you, team is not, like, speaking and do nothing. Obviously, they have a huge backlog. 
**Pablo Blauer** *[26:58]*: Yeah. 
**Slava Vlaskin** *[26:58]*: On their No. 
**Pablo Blauer** *[26:59]*: Because the way I'm imagining myself doing this is, you know, having a product owner or product manager, you know, doing the first part, you know, describing the requirement or at least, you know, inputting from a conversation with the client, creating the ticket, and then developers take over what you do, which is essentially seen. And as you see, as you said, some people will like to do it more manually. Some people will do it more automatically. But I think it all can go in a same workflow. But you say, okay. I created this sticker. The developer will take it and implement it and make sure that it's well with quality in certain environment and so on. You will then come back the product owner and and recheck and so on. All is there, but it's handled by each person individually. 
**Pablo Blauer** *[27:44]*: So you or the product owner have more time to create more requirements and large the backlog as well. 
**Slava Vlaskin** *[27:49]*: Yeah. Yeah. I guess. 
**Pablo Blauer** *[27:51]*: And, also, the dev team can simply say to Devin, oh, I found this technical dev. Can you add it as a ticket? And that's it. It's not hidden anymore. Or I found this bug. Boom. That's it. Cool. I it's very interesting, really. I need to drop now, but I I have one question. Do you think we are probably in a good position to share this? Just with sharing what you've shared to me is is amazing to me. It's it's very valuable. But do you think we can do kind of a session with more people to share, like, what you are doing, you know, the status and so on, saying, like, we are starting. Maybe you can share the first, you know, automation case that it created by then and so on. But, essentially, it Yes. 
**Pablo Blauer** *[28:37]*: Covers requirement gathering and ticket creation, documentation, coding, deploying, quality. I I already said it. Automation, and so it covers everything. And and it's amazing. So it's a little bit. 
**Slava Vlaskin** *[28:59]*: I think, Pablo, yeah, I definitely want to share it. I even want to share it. Yeah. 
**Pablo Blauer** *[29:06]*: Cool. 
**Slava Vlaskin** *[29:06]*: But one thing, I just know I'm just not sure about the timing of it. This week is completely, like, unavailable for me. We'll do Maybe we can. 
**Pablo Blauer** *[29:21]*: We'll do it with time. Whenever it's work it's good for you. Maybe, I don't know, Thursday or Friday, thirteen, like, two weeks from now or three weeks from now, I think, something like that. Oh, that's even if it's the '20. I mean, I don't mind about the date. You tell me what's better date for you, what works. 
**Slava Vlaskin** *[29:43]*: And I can submit in two weeks, and we can agree Two weeks. We can agree over to yeah. 
**Pablo Blauer** *[29:51]*: Yeah. Let's say the thirteenth or the twentieth, whatever works. 
**Slava Vlaskin** *[29:57]*: Give me a sec. 
**Pablo Blauer** *[29:59]*: Or maybe a Thursday, the twelfth or the nineteenth. 
**Slava Vlaskin** *[30:03]*: Let's do nineteenth. Let's agree on nineteenth then. We'll have a bit more time to test. 
**Pablo Blauer** *[30:10]*: There there is another accelerator. Do you mind if we do it on the twentieth? 
**Slava Vlaskin** *[30:15]*: Okay. I'm I'm totally fine. 
**Pablo Blauer** *[30:17]*: Okay. Friday, the twentieth. That's I'll put a place Huddl for you and I. Only for, 
**Slava Vlaskin** *[30:22]*: The tools. Okay. Okay. 
**Pablo Blauer** *[30:24]*: And and we can regroup later. 
**Slava Vlaskin** *[30:29]*: This. 
**Pablo Blauer** *[30:31]*: Is very interesting, to be honest. 
**Slava Vlaskin** *[30:35]*: Yeah. Yeah. I, like, I seriously impressed too. There is a lot of pressure, you know, from our from our clients, but, yeah, it's really and amazing in some cases. Yeah. 
**Pablo Blauer** *[30:54]*: Yeah. And you seem to have a meeting at 9AM CT. 
**Slava Vlaskin** *[31:01]*: Is. 
**Pablo Blauer** *[31:07]*: Is ten CT too late for you? 
**Slava Vlaskin** *[31:13]*: Ten CT. No. I think it's okay. It's okay. Okay. 
**Pablo Blauer** *[31:25]*: I'll put that on a Friday, okay, or on a Thursday. You you can tell me what works. 
**Slava Vlaskin** *[31:32]*: That won't matter. And a day is at work for you. 
**Pablo Blauer** *[31:39]*: I will try to keep it very short and try to focus on your sharing. But it's really interesting. Okay. 
**Slava Vlaskin** *[31:49]*: I'll I'll prepare I'll be more prepared than. 
**Pablo Blauer** *[31:54]*: No. I I To be honest, I don't think it needs to be more prepared than this. Probably if you have a diagram or, like, saying, like, what is behind this? Like, what what is the LLM behind Devin? Is that a sonnet? Like, how. 
**Slava Vlaskin** *[32:09]*: It's, like, Claude. Claude. That's Claude. As part of my name. 
**Pablo Blauer** *[32:13]*: For everything. For coding, for documentation, for everything. Yeah. Maybe a brief description of what Devin is. Right? Maybe we're Sure. Sure. 
**Slava Vlaskin** *[32:22]*: Yeah. Like, this was very, like, preliminary meeting. I just shared, like, all my thoughts. But yeah. 
**Pablo Blauer** *[32:29]*: But to be honest, you can share these examples as you can like, it's amazing. You can see, like, you know, I simply chatted and say, I want this and it created all that. Cool. Alright. Thank you, Slava. I really appreciate it, and we'll connect later. Okay? 
**Slava Vlaskin** *[32:47]*: Yep. Thank you. 
**Pablo Blauer** *[32:48]*: And and I guess I I didn't get what's not what doesn't work. Or. 
**Slava Vlaskin** *[32:56]*: I don't know. Really? I don't know. We've tried, like, a lot of different cases. With the firm adjustments, everything seems to be achievable. Not saying perfect, but really achievable. 
**Pablo Blauer** *[33:11]*: Awesome. What yeah. Security? What about security? 
**Slava Vlaskin** *[33:17]*: No. Actually, we didn't try it. We didn't try it that. Also, yeah, also, if you have one minute, just one thing that I think will not fit every project need is just because they are self hosted. So there is no ability, you know, to, like, self host Devin as as far as I know. And for some teams, for some projects, this will be a huge compliance gap. 
**Pablo Blauer** *[33:53]*: So everything is going to Devin? 
**Slava Vlaskin** *[33:55]*: Yes. Yes. Exactly. 
**Pablo Blauer** *[33:58]*: And, also, there are a thing that Igor told me as well is that these are mainly microservices that are very small in scope, and as well because of that. If you will would have a kind of a monorepo more larger, it will be more complex too. 
**Slava Vlaskin** *[34:18]*: I have actually doubts about it because we right now, we're in the middle of transferring from the monorees or maybe so on. Yeah. To the to the microservices. I'd say it's does pretty good job with Monorepo too. 
**Pablo Blauer** *[34:39]*: So, yeah, maybe we. 
**Slava Vlaskin** *[34:40]*: Would obviously. 
**Pablo Blauer** *[34:42]*: Can do a few intro slides of what Devin is first, like, Sonnet or, you know, Claude is behind the scenes. And what is your project like in terms of we have a microservices. We have, you know, we are not in production. We are blah. You know, everything that is important as well to realize. 
**Slava Vlaskin** *[35:01]*: Yeah. Production description definitely might help. Mhmm. 
**Pablo Blauer** *[35:03]*: Cool. Alright. Thank you, Slava. I'll connect later. Bye bye. Bye. 
