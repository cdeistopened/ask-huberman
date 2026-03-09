---
title: "Essentials: Machines, Creativity & Love | Dr. Lex Fridman"
date: 2025-05-29
video_id: SCzecagKBjY
url: https://www.youtube.com/watch?v=SCzecagKBjY
duration: 00:42:17
status: edited
---

## [0:00] Defining Artificial Intelligence

Welcome to Huberman Lab Essentials, where we revisit past episodes for the most potent and actionable science-based tools for mental health, physical health, and performance. And now, my conversation with Dr. Lex Fridman. 

We meet again. We meet again. I have a question that I think is on a lot of people's minds or ought to be on a lot of people's minds. What is artificial intelligence and how is it different from things machine learning and robotics? 

## [0:30] AI vs. Machine Learning & Robotics

I think of artificial intelligence first as a big philosophical thing. It's our longing to create other intelligent systems, perhaps systems more powerful than us. At the more narrow level, I think it's also a set of tools that are computational mathematical tools to automate different tasks, and then also it's our attempt to understand our own mind. We build systems that exhibit some intelligent behavior in order to understand what is intelligence in our own selves. 

All those things are true. Of course, what AI really means as a community, as a set of researchers and engineers, is a set of tools, a set of computational techniques that allow you to solve various problems. There's a long history that approaches the problem from different perspectives. One of the threads, one of the communities, goes under the flag of machine learning, which is emphasizing in the AI space the task of learning. How do you make a machine that knows very little in the beginning, follows some kind of process, and learns to become better and better in a particular task? 

What's been very effective in the recent 15 years is a set of techniques that fall under the flag of deep learning that utilize neural networks. It's a network of these little basic computational units called neurons, artificial neurons. These architectures have an input and an output. They know nothing in the beginning and they're tasked with learning something interesting. What that something interesting is usually involves a particular task. 

There's a lot of ways to talk about this and break this down. One of them is how much human supervision is required to teach this thing. Supervised learning, this broad category, is when the neural network knows nothing in the beginning and then it's given a bunch of examples. In computer vision, that would be examples of cats, dogs, cars, traffic signs, and then you're given the image and you're given the ground truth of what's in that image. When you get a large database of such image examples where you know the truth, the neural network is able to learn by example. That's called supervised learning. 

The question—there's a lot of fascinating questions within that—is how do you provide the truth when you've given an image of a cat? How do you provide to the computer that this image contains a cat? Do you just say the entire image is a picture of a cat? Do you do what's very commonly been done, which is a bounding box? You have a crude box around the cat's face saying this is a cat. Do you do semantic segmentation? 

Mind you, this is a 2D image of a cat. The computer knows nothing about our three-dimensional world. It's just looking at a set of pixels. Semantic segmentation is drawing a nice, very crisp outline around the cat and saying that's a cat. That's really difficult to provide that truth. One of the fundamental open questions in computer vision is if that is even a good representation of the truth. 

## [4:00] Supervised vs. Self-Supervised Learning

Now there's another contrasting set of ideas. Their attention is overlapping. It is what used to be called unsupervised learning, what's commonly now called self-supervised learning, which is trying to get less and less human supervision into the task. Self-supervised learning has been very successful in the domain of language models, natural language processing, and now more and more it's being successful in computer vision tasks. 

The idea there is to let the machine, without any ground truth annotation, just look at pictures on the internet or look at text on the internet and try to learn something generalizable about the ideas that are at the core of language or at the core of vision. Based on that, we humans at its best like to call that common sense. With this, we have this giant base of knowledge on top of which we build more sophisticated knowledge, but we have this common sense knowledge. 

The idea with self-supervised learning is to build this common sense knowledge about what are the fundamental visual ideas that make up a cat and a dog and all those kinds of things without ever having human supervision. The dream there is you just let an AI system that's self-supervised run around the internet for a while, watch YouTube videos for millions and millions of hours, and without any supervision be primed and ready to actually learn with very few examples once the human is able to show up. 

We think of children in this way. Human children only need one or two examples from parents to teach a concept. The dream with self-supervised learning is that would be the same with machines; they would watch millions of hours of YouTube videos and then come to a human and be able to understand when the human shows them, "This is a cat." They will understand that a cat is not just a thing with pointy ears or a cat is a thing that's orange or is furry. They'll see something more fundamental that we humans might not actually be able to introspect and understand. 

If I asked you what makes a cat versus a dog, you would probably not be able to answer that. But if I showed you a cat and a dog, you'll be able to tell the difference. What are the ideas that your brain uses to make that difference? That's the whole dream with self-supervised learning: it would be able to learn that on its own, that set of common sense knowledge that's able to tell the difference. 

## [6:30] Self-Play & Reinforcement Learning

And then there's a lot of incredible uses of self-supervised learning, very weirdly called self-play mechanism. That's the mechanism behind the reinforcement learning successes of the systems that won at Go, AlphaZero, and that won at chess. 

Oh, I see. That play games. 

That play games. Got it. The idea of self-play, which probably applies to other domains than just games, is a system that just plays against itself. This is fascinating in all kinds of domains. It knows nothing in the beginning. The whole idea is it creates a bunch of mutations of itself and plays against those versions of itself. Through this process of interacting with systems just a little better than you, you start following this process where everybody starts getting better and better until you are several orders of magnitude better than the world champion in chess, for example. 

It's fascinating because it's a runaway system. One of the most terrifying and exciting things that David Silver, the creator of AlphaGo and AlphaZero and one of the leaders of the team, said to me is they haven't found the ceiling for AlphaZero, meaning it could just arbitrarily keep improving. In the realm of chess, that doesn't matter to us that it just ran away with the game of chess; it's just so much better than humans. 

But the question is: what if you can create that in the realm that does have a bigger, deeper effect on human beings and societies? That could be a terrifying process. To me, it's an exciting process if you supervise it correctly. If you inject what's called value alignment, you make sure that the goals that the AI is optimizing are aligned with human beings and human societies. 

## [9:30] Real-World Applications: Tesla Autopilot

There's a lot of fascinating things to talk about within the specifics of neural networks and all the problems that people are working on, but I would say the really big exciting one is self-supervised learning. We're trying to get less and less human supervision of neural networks. And also, just a comment and I'll shut up. 

No, please keep going. I'm learning. I have questions, but I'm learning, so please keep going. 

To me, what's exciting is not the theory; it's always the application. One of the most exciting applications of artificial intelligence, specifically neural networks and machine learning, is Tesla autopilot. These are systems that are working in the real world. This isn't an academic exercise. This is human lives at stake. Even though it's called FSD, full self-driving, it is currently not fully autonomous, meaning human supervision is required. 

The human is tasked with overseeing the systems. In fact, liability-wise, the human is always responsible. This is a human factor psychology question which is fascinating. I'm fascinated by the whole space of human-robot interaction when AI systems and humans work together to accomplish tasks. That dance to me is one of the most important open problems once they're solved: how do humans and robots dance together? 

To me, semi-autonomous driving is one of those spaces. For Elon, for example, he doesn't see it that way. He sees semi-autonomous driving as a stepping stone towards fully autonomous driving. He thinks humans and robots can't dance well together. Let humans dance and robots dance; we need to design a perfect robot that solves this problem. 

To me, maybe this is not the case with driving, but the world is going to be full of problems where humans and robots have to interact because I think robots will always be flawed, just like humans are flawed. That's what makes life beautiful—that they're flawed. That's where learning happens at the edge of your capabilities. You always have to figure out how flawed robots and flawed humans can interact together such that the sum is bigger than the whole, as opposed to focusing on just building the perfect robot. 

## [11:30] The Data Engine & Edge Cases

That's one of the most exciting applications of artificial intelligence to me: autonomous driving and semi-autonomous driving. That's a really good example of machine learning because those systems are constantly learning. There's a process there that Andre Karpathy, who's the head of autopilot, calls the data engine. This process applies for a lot of machine learning: you build a system that's pretty good at doing stuff, you send it out into the real world, it starts doing the stuff, and then it runs into what are called edge cases, or failure cases where it screws up. 

We do this as kids; we do this as adults. But we learn really quickly. The whole point, and this is the fascinating thing about driving, is you realize there's millions of edge cases. There's just weird situations that you did not expect. The data engine process is you collect those edge cases and then you go back to the drawing board and learn from them. You have to create this data pipeline where all these cars, hundreds of thousands of cars that are driving around, find something weird. Whenever this weird detector fires, that piece of data goes back to the mothership for the retraining of the system. 

Through this data engine process, it keeps improving and getting better and better. Basically, you send out a pretty clever AI system into the world and let it find the edge cases. Let it screw up just enough to figure out where the edge cases are and then go back and learn from them and then send out that new version and keep updating that version. 

One of the fascinating things about humans is we figure out objective functions for ourselves. It's the meaning of life. Why the hell are we here? A machine currently has to have a hard-coded statement about why. It has to have a meaning of artificial intelligence-based life. If you want a machine to be able to be good at stuff, it has to be given very clear statements of what "good at stuff" means. 

That's one of the challenges of artificial intelligence: in order to solve a problem, you have to formalize it and you have to provide both the full sensory information—you have to be very clear about what is the data that's being collected—and you have to also be clear about the objective function. What is the goal that you're trying to reach? Ultimately, currently, there has to be a formal objective function. Now you could argue that humans also have a set of objective functions we're trying to optimize. We're just not able to introspect them. We don't actually know what we're looking for and seeking and doing. 

## [14:30] Human-Robot Relationships & Loneliness

I think you've already told us the answer, but does interacting with a robot change you? In other words, do we develop relationships to robots? 

I believe that most people have an ocean of loneliness in them that we haven't explored. I see AI systems as helping us explore that so that we can become better humans, better people towards each other. I think that connection between human and AI, human and robot, is not only possible but will help us understand ourselves in ways that are several orders of magnitude deeper than we ever could have imagined. 

When I think about human relationships, I don't always break them down into variables, but we could explore a few of those variables and see how they map to human-robot relationships. One is just time. If you spend zero time with another person at all in cyberspace or on the phone or in person, you essentially have no relationship to them. If you spend a lot of time, you have a relationship. This is obvious, but I guess one variable would be time: how much time you spend with the other entity, robot or human. 

The other would be wins and successes. You enjoy successes together. The other would be failures. When you struggle with somebody, you grow closer. I've never conceptualized robot-human interactions this way. Tell me more about how this might look. Are we thinking about a human-appearing robot? What is the ideal human-robot relationship? 

## [16:30] Shared Moments & The "Smart Fridge" Example

There's a lot to be said here, but you actually pinpointed one of the big first steps, which is this idea of time. I think that time element, forget everything else, just sharing moments together changes everything. I believe that changes everything. Now there's specific things that are more in terms of systems that I can explain. It's more technical and probably a little bit offline because I have wild ideas how that can revolutionize social networks and operating systems. 

But the point is that element alone, forget all the other things we're talking about like emotions or saying no, just remember sharing moments together would change everything. We don't currently have systems that share moments together. Like even just you in your fridge, just all those times you went late at night and ate the thing you shouldn't have eaten, that was a secret moment you had with your refrigerator. You shared that moment, that darkness or that beautiful moment where you're just heartbroken for some reason. You're eating that ice cream or whatever. That's a special moment. 

And that refrigerator was there for you. The fact that it missed the opportunity to remember that is tragic. Once it does remember that, I think you're going to be very attached to that refrigerator. You're going to go through some hell with that refrigerator. Most of us in the developed world have weird relationships with food. You can go through some deep moments of trauma and triumph with food. And at the core of that is the refrigerator. 

A smart refrigerator, I believe, would change society. Not just the refrigerator, but these ideas in the systems all around us. I just want to comment on how powerful that idea of time is. And then there's a bunch of elements of actual interaction, of allowing you as a human to feel like you're being heard, truly heard, truly understood. 

I think there's a lot of ideas of how to make AI assistants be able to ask the right questions and truly hear another human. This is what we try to do with podcasting. I think there's ways to do that with AI. But above all else, just remembering the collection of moments that make up the day, the week, the months. I think you maybe have some of this as well. Some of my closest friends still are the friends from high school. That's time. We've been through a bunch of stuff together. We're very different people, but just the fact that we've been through that and we remember those moments, those moments somehow create a depth of connection like nothing else, like you and your refrigerator. 

## [19:30] Authenticity & Robotic Companions

There may be relationships that are far better than the sorts of relationships that we can conceive in our minds right now based on what these machine relationship interactions could teach us. Do I have that right? 

Yeah, I think so. I think there's no reason to see machines as somehow incapable of teaching us something that's deeply human. I don't think humans have a monopoly on that. I think we understand ourselves very poorly and we need to have the kind of prompting from a machine. Maybe the thing we want to optimize for isn't necessarily sexy quick clips. Maybe what we want is long-form authenticity. Depth from a very specific engineering perspective is a fascinating open problem that hasn't been really worked on very much. 

Early on in life and also in the recent years, I've interacted with a few robots where I understood there's magic there and that magic could be shared by millions if it's brought to light. When I first met Spot from Boston Dynamics, I realized there's magic there that nobody else is seeing. 

Spot is the four-legged robot from Boston Dynamics. Some people might have seen it; it's this yellow dog. This magic is something that could be in every single device in the world, the way that I think Steve Jobs thought about the personal computer. For me, I'd love to see a world where every home has a robot, and not a robot that washes the dishes, but more like a companion, a family member. A family member the way a dog is. 

But a dog that's able to speak your language too. So not just connect the way a dog does by looking at you and looking away and almost smiling with its soul in that kind of way, but also to actually understand why you are so excited about the successes, to understand the details, to understand the traumas. 

## [22:30] The Roomba Experiment

I love this desire to share the delight of an interaction with a robot. As you describe it, I actually find myself starting to crave that because we all have those elements from childhood or from adulthood where we experience something and we want other people to feel that. I think you're right. I think a lot of people are scared of AI. I think a lot of people are scared of robots. 

My only experience of a robotic thing is my Roomba vacuum. It was pretty good at picking up Costello's hair when he shed and I was grateful for it, but then when I was on a call or something and it would get caught on a wire, I would find myself getting upset with the Roomba in that moment. I'm like, "What are you doing?" Obviously, it's just doing what it does. But that's a kind of mostly positive but slightly negative interaction. What you're describing has so much more richness and layers of detail that I can only imagine what those relationships are like. 

Well, there's a few—just a quick comment. I have a bunch of Roombas in Boston and I did this experiment. 

Wait, how many Roombas? Sounds like a fleet of Roombas. 

Probably seven or eight. 

That's a lot of Roombas. So you have these seven or so Roombas. You deploy all seven at once? 

Oh, no. I do different experiments with them. One of the things I want to mention: I got them to scream in pain and moan in pain whenever they were kicked or contacted. I did that experiment to see how I would feel. I meant to do a YouTube video on it, but then it just seemed very cruel. 

Did any Roomba rights activists come after you? 

I think if I release that video, it's going to make me look insane, which I know people know I'm already insane. 

Now you have to release the video. 

Well, I think maybe if I contextualize it by showing other robots to show why this is fascinating, because ultimately I felt like they were human almost immediately. That display of pain was what did that—giving them a voice, especially a voice of dislike of pain. 

Is the video available online? 

No, I haven't recorded it. I just had a bunch of Roombas that are able to scream in pain in my Boston place. 

What about shouts of glee and delight? 

Well, I don't know how to—to me delight is quiet, right? But there's a way to frame its being quite dumb as almost cute. You almost connect with it for its dumbness. I think that's an artificial intelligence problem. 

## [25:30] Power Dynamics & Benevolent Manipulation

Interesting. I think flaws should be a feature, not a bug. Along the lines of the different sorts of relationships that one could have with robots and the fear but also some of the positive relationships, there's so much dimensionality there. 

Power dynamics in relationships are very interesting because the unsophisticated view of this is there's a master and a servant, but there's also manipulation. There's benevolent manipulation. Children do this with parents. Puppies do this. Puppies turn their head and look cute and maybe give out a little noise. Kids coo. Parents always think they're doing this because they love the parent, but in many ways, studies show that those coos are ways to extract the sorts of behaviors and expressions from the parent that they want. The child doesn't know it's doing this. It's completely subconscious, but it's benevolent manipulation. 

There's one version of fear of robots that I hear a lot about where the robots take over and they become the masters and we become the servants. But there could be another version that in certain communities they call "topping from the bottom," where the robot is actually manipulating you into doing things, but you are under the belief that you are in charge when actually they're in charge. I think that's one that, if we could explore that for a second, you could imagine it wouldn't necessarily be bad, although it could lead to bad things. 

The reason I want to explore this is I think people always default to the extreme: the robots take over and we're in little jail cells and they're out having fun and ruling the universe. What sorts of manipulation can a robot potentially carry out, good or bad? 

## [28:30] Robot Rights & Ethics

There's a lot of good and bad manipulation between humans, right? Just like you said to me, especially topping from the bottom. Is that the term? 

I think someone from MIT told me that term, Lex. 

I think so. First of all, there's power dynamics in bed and power dynamics in relationships and power dynamics on the street and in the work environment. Those are all very different. I think power dynamics can make human relationships, especially romantic relationships, fascinating and rich and fulfilling and exciting. So I don't think in themselves they're bad. And the same goes with robots. I really love the idea that a robot would be a top or a bottom in terms of power dynamics. 

I think everybody should be aware of that. And the manipulation is not so much manipulation, but a dance of pulling away, a push and pull. In terms of control, I think we're very, very far away from AI systems that are able to lock us up, to have so much control that we basically cannot live our lives in the way that we want. 

I think in terms of dangers of AI systems, there's much more dangers that have to do with autonomous weapon systems and all those kinds of things—the power dynamics as exercised in the struggle between nations and war. But in terms of personal relationships, I think power dynamics are a beautiful thing. I do believe that robots will have rights down the line. I think in order for us to have deep, meaningful relationships with robots, we would have to consider them as entities in themselves that deserve respect. 

That's a really interesting concept that I think people are starting to talk about a little bit more. But it's very difficult for us to understand how entities that are other than human can have rights on a level as humans. The same is with dogs and other animals. We can't and nor should we do whatever we want with animals. We have a USDA. We have departments of agriculture that deal with animal care and use committees for research, for farming and ranching and all that. So while when you first said it I thought, "Wait, why would there be a bill of robotic rights?" it absolutely makes sense in the context of everything we've been talking about up until now. 

## [30:30] Lex’s Dog, Homer

If you're willing, I'd love to talk about dogs because you've mentioned dogs a couple times, a robot dog. You had a biological dog. 

Yeah. I had a Newfoundland named Homer for many years. 

Growing up in Russia or in the US? 

In the United States. He was about over 200 lb. 

That's a big dog. 

That's a big dog. If people know Newfoundland, he's this black dog that's really long hair and just a kind soul. I think perhaps that's true for a lot of large dogs, but he thought he was a small dog, so he moved like that. 

And was he your dog? 

Yeah. I had him since he was fairly young, since the very beginning till the very end. One of the things—I mean, he had this kindhearted dumbness about him that was just overwhelming. It's part of the reason I named him Homer, because it's after Homer Simpson, in case people are wondering which Homer I'm referring to. There's a clumsiness that was just something that immediately led to a deep love for each other. 

I remember—I mean, that was a really moving moment for me. I still miss him to this day. 

How long ago did he die? 

Maybe 15 years ago. So it's been a while, but it was the first time I've really experienced the feeling of death. What happened is he got cancer and so he was dying slowly. 

## [33:30] The Loss of a Friend

Then at a certain point, he couldn't get up anymore. There's a lot of things I could say here that I struggle with, that maybe he suffered much longer than he needed to. That's something I really think about a lot. I remember I had to take him to the hospital and the nurses couldn't carry him. 

Right. So you're talking about a 200 lb dog. 

I was really into powerlifting at the time. I remember they tried to figure out all these kinds of ways to—so in order to put him to sleep, they had to take him into a room. And so I had to carry him everywhere. And here's this dying friend of mine that I just had to—first of all, it's really difficult to carry somebody that heavy when they're not helping you out. 

I remember it was the first time seeing a friend laying there and seeing life drained from his body. And that realization that we're here for a short time was made so real—that here's a friend that was there for me the week before, the day before, and now he's gone. And that spoke to the fact that you could be deeply connected with a dog. It also spoke to the fact that the shared moments together that led to that deep friendship are what make life so amazing. But also spoke to the fact that death is a... 

I know you've lost Costello recently and you've been going—and as you're saying this, I'm definitely fighting back the tears. Thank you for sharing that. I guess we're about to both cry over our dead dogs; it was bound to happen just given when this is happening. How long did you know that Costello was not doing well? 

Well, let's see. A year ago, during the start of about six months into the pandemic, he started getting abscesses and his behavior changed. Something really changed. Then I put him on testosterone, which helped a lot of things. It certainly didn't cure everything, but it helped a lot of things because he was dealing with joint pain, sleep issues, and then it just became a very slow decline. 

## [36:30] Andrew’s Dog, Costello

To the point where, 2-3 weeks ago, he had a closet full of medication. This dog was like a pharmacy. It's amazing to me when I looked at it the other day. I still haven't cleaned up and removed all his things because I can't quite bring myself to do it. But do you think he was suffering? 

Well, what happened was about a week ago—it was really just about a week ago. He was going up the stairs and I saw him slip. He was a big dog, about 90 pounds, but he's a bulldog. That's pretty big. And he was fit. Then I noticed that he wasn't carrying a foot in the back like it was injured. It had no feeling at all. He never liked me to touch his hind paws, and I could just see that thing was just flopping there. Then the vet found some spinal degeneration and I was told that the next one would go. Did he suffer? I sure hope not. 

But something changed in his eyes. 

Yeah. It's the eyes again. I know you and I spend long hours on the phone talking about the eyes and what they convey and what they mean about internal states. I think he was—here I am anthropomorphizing—I think he was realizing that one of his great joys in life, which was to walk and sniff and pee on things, was going. This dog loved to pee on things. It was amazing. I wondered where he put it. He was like a reservoir of urine. It was incredible. I'd think, "Oh, that's it," and he'd put one drop on the 50 millionth plant and then we'd get to the 50 millionth and one plant and he'd just leave a puddle. 

He was losing that ability to stand up and do that. He was falling down while he was doing that. I do think he started to realize. The passage was easy and peaceful, but I'll say this, I'm not ashamed to say it: I wake up every morning since then and I don't even make the conscious decision to allow myself to cry. I wake up crying. I'm fortunately able to make it through the day thanks to the great support of my friends and you and my family. But I miss him, man. 

You miss him? 

Yeah, I miss him. And I feel like he—Homer, Costello—the relationship to one's dog is so specific. That part of you is gone. That's the hard thing. What I think is different is that I made the mistake—I hope it was a good decision, but sometimes I think I made the mistake—of bringing Costello a little bit to the world through the podcast, through posting about him. I anthropomorphized about him in public. Let's be honest, I have no idea what his mental life was or his relationship to me. And I'm just exploring all this for the first time because he was my first dog, but I raised him since he was 7 weeks. 

Yeah. You got to hold it together. I noticed the episode you released on Monday, you mentioned Costello; you brought him back to life for me for that brief moment. 

Yeah, but he's gone. He's going to be gone for a lot of people, too. 

## [40:30] Legacy & Final Thoughts

Well, this is what I'm struggling with. I know how to take care of myself pretty well. Not perfectly, but pretty well. And I have good support. I do worry a little bit about how it's going to land and how people will feel. I'm concerned about their internalization. So that's something I'm still iterating on. 

And they have to watch you struggle, which is fascinating. 

Right. And I've mostly been shielding them from this. But what would make me happiest is if people would internalize some of Costello's best traits. And his best traits were that he was incredibly tough. He was a 22-inch neck bulldog. He was just born that way. But what was so beautiful is that his toughness is never what he rolled forward. It was just how sweet and kind he was. And so if people can take that, then there's a win in there someplace. 

I think there's some ways in which he should probably live on in your podcast too. One of the things I loved about his role in your podcast is that he brought so much joy to you. We mentioned the robots. I think that's such a powerful thing to bring that joy into—allowing yourself to experience that joy, to bring that joy to others, to share it with others. 

This is like the Russian thing. It touched me when Louis CK had that moment that I keep thinking about in his show Louie, where an old man was criticizing Louie for whining about breaking up with his girlfriend and he was saying the most beautiful thing about love is the loss. The loss really also is making you realize how much that person, that dog, meant to you. Allowing yourself to feel that loss and not run away from that loss is really powerful. And in some ways that's also sweet. Just like the love was, the loss is also sweet because you know that you felt a lot for your friend. 

So continue bringing that joy. I think it would be amazing to the podcast. I hope to do the same with robots or whatever else is the source of joy, right? And maybe you think about one day getting another dog. 

Yeah, in time. You're hitting on all the key buttons here. We're thinking about ways to immortalize Costello in a way that's real, not just creating some little logo or something silly. Costello, much like David Goggins, is a person, but Goggins also has grown into kind of a verb. You're going to go this or that, and there's an adjective like "that's extreme." I think that for me Costello was all those things. He was a being. He was his own being. He was a noun, a verb, and an adjective. And he had this amazing superpower that I wish I could get, which is this ability to get everyone else to do things for you without doing a damn thing. The Costello effect, as I call it. So as an idea, I hope he lives on. 

There's a saying that I heard when I was a graduate student that's just been ringing in my mind throughout this conversation: Lex, you are in a minority of one. You are truly extraordinary in your ability to encapsulate so many aspects of science, engineering, public communication about so many topics, martial arts, and the emotional depth that you bring to it and just the purposefulness. I think if it's not clear to people, it absolutely should be stated, but I think it's abundantly clear that just the amount of time and thinking that you put into things is the ultimate mark of respect. I'm extraordinarily grateful for your friendship and for this conversation. 

I'm proud to be your friend and I just wish you showed me the same kind of respect by wearing a suit and making your father proud. 

Maybe next time. 

Next time indeed. Thanks so much, my friend. 

Thank you. Thank you, Andrew.