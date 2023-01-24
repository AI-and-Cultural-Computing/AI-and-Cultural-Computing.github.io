---
layout: post
title:  "AICC Newsletter 2"
date:   2022-12-15 18:49:32 -0800
categories: newsletter
---
Hello again!

Now is the time of our second newsletter full of developments happening in the world of AI and ML.

There were, shockingly, no gigantic earth-shattering developments dropped in the past week. You may think I'm joking but honestly the pace of AI research really does make you get used to weekly big news.

That being said, I think there's still a lot of really cool things to share and talk about!

First, related to chatGPT (which I shared a lot about last week) as well as Google's copilot I have some interesting links about people using large language models for coding.

The programmer mnmlmnl has a very compelling and actually very positive report on using chatGPT in his work here: https://write.as/mnmlmnl/working-with-chatgpt

And another programmer talking about trying to use chatGPT to help him learn the language Rust while solving Advent of Code (https://adventofcode.com/) problems:
https://simonwillison.net/2022/Dec/5/rust-chatgpt-copilot/

For programmer in the audience who know what AoC is and whince at the idea of someone using LLMs to solve problems faster, the author of said post explicitly says he doesn't submit his solutions in a timely manner to avoid competing on the leaderboard.

Oh, and speaking of programmers and their friends the mathematicians I found a really cool, really accessible tutorial on the mathematical framework that makes modern machine learning tractable: automatic differentiation! https://thenumb.at/Autodiff/

Automatic differentiation is basically about getting the computer to do calculus for us, by which I mean we get to write down equations in terms of adding, multiplying, dividing, things like that and then the AD framework will just figure out the "rate of change" of those functions, well, automatically and more importantly very efficiently. Why do you need to know how fast or slow functions grow and shrink? Well that's the basic of how we train neural networks: gradient descent.

If you remember how we compared training a neural network to letting a ball roll down hill until it settles in a flat spot? This is about calculating the slope of the hill so we can figure out where the ball will end up. Which is really important when you're "rolling" down a >100000 dimensional space beyond human comprehension and not, y'know,

a hill.

In less cool and more frustrating news some folks are having bad experiences with the new Lensa app that's gone viral, which lets people transform their pictures and turn them into a variety of different styles and vibes. If you guessed that it's going to have something to do with racism and sexism, you'd be right
https://arstechnica.com/information-technology/2022/12/lensa-ai-app-causes-a-stir-with-sexy-magic-avatar-images-no-one-wanted
https://www.technologyreview.com/2022/12/12/1064751/the-viral-ai-avatar-app-lensa-undressed-me-without-my-consent/

Finally, I'd like to plug this little self-directed course I've been having fun with on the weekends: https://github.com/johnowhitaker/aiaiart

It does require a bit harder of coding than what you may have done so far but it also has a discord where you can ask questions about any lesson

That's all from me this week
