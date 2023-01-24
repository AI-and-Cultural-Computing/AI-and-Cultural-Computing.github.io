---
layout: post
title:  "AICC Newsletter 4: LLMs and Higher ed"
date:   2023-01-05 18:49:32 -0800
categories: newsletter llms
---

Hey everyone!

Hope y'all had a good break. I got thrown off this week by us having monday off so you're getting one of my brain-and-link-dump newsletters on a thursday instead of a wednesday.

So what I wanted to talk even more about chatGPT, the big system that dropped just about a month ago now that was&#x2014;and currently is&#x2014;freaking a lot of people out. I want to share a few different perspectives about chatGPT, some I agree with and some that I think are a little goofy, and talk about what I personally think are its real implications for us as educators.

First, let's talk about this piece that Melissa linked to this morning: <https://www.cnn.com/2023/01/05/tech/chatgpt-nyc-school-ban/index.html>
(which itself is mostly a re-reporting of the content of this linked article <https://ny.chalkbeat.org/2023/1/3/23537987/nyc-schools-ban-chatgpt-writing-artificial-intelligence>)

The tl;dr is that NYC's education department has blocked access to chatGPT from devices administered by NYC schools or from NYC public schools' networks. Why? Because they're concerned about chatGPT not just being used to cheat but, in a sense, to **cheat badly** as chatGPT frequently returns incorrect information.

This decision out of NYC definitely feels in line with stories like this one about a professor who, almost immediately after the release of chatGPT, caught a student using it to fake an essay:
<https://nypost.com/2022/12/26/students-using-chatgpt-to-cheat-professor-warns/amp/>

> Earlier this month, Hick had instructed his class to write a 500-word essay on the 18th-century philosopher David Hume and the paradox of horror, which examines how people can get enjoyment from something they fear, for a take-home test.
> 
> But one submission, he said, featured a few hallmarks that “flagged” AI usage in the student’s “rudimentary” answer.
> 
> “It’s a clean style. But it’s recognizable. I would say it writes like a very smart 12th-grader,” Hick said of ChatGPT’s written responses to questions.
> 
> “There’s particular odd wording used that was not wrong, just peculiar … if you were teaching somebody how to write an essay, this is how you tell them to write it before they figure out their own style.”

What's interesting about this case, of course, is that he felt confident that it was in fact a machine generated essay because of the discovery that the old gpt-2 text-detector works remarkably well even on this far more fluent and cogent system: <https://openai-openai-detector.hf.space/>

The fact that you can still really easily algorithmically detect chatGPT text sorta validates this professor's gut instinct that something feels "off" about the text, and I find that just incredibly fascinating. 

What's funny, to me, is that you can contrast this ban with this toot (did Mastodon 4 change the default to "post"? yes. will I say toot when it amuses me? also, yes) by the mathematician Terence Tao shortly after the release of chatGPT 
<https://mathstodon.xyz/@tao/109543141003492779>

> AI tools like #ChatGPT will soon be capable of answering a large fraction of traditional university homework type questions with reasonable accuracy.  In the long term, it seems futile to fight against this; perhaps what we as lecturers need to do is to move to an "open books, open AI" mode of examination where we give the students full access to AI tools but ask them more challenging questions, both to teach the material and also to teach the students how best to use the AI tools of the future.

It's an interesting question, right? What's the right approach here? Do we push the tools away or do we embrace them and change our assignments and what we ask of students? I mean we have people speculating that gpt-4 will be able to do far better than even chatGPT (<https://the-decoder.com/gpt-4-could-pass-bar-exam-ai-researchers-say/>) and from there 

Personally, I probably lean more towards Terence's view than the NYC public school system **if these systems worked more as advertised**. Here's where things get a little thorny, I think, because the question becomes "can something like chatGPT actually replace search engines?"

Linguistics professor Emily Bender has a lot to say on this topic. First, here's her short news interview where she's giving her explanation and complaints about chatGPT
<https://www.youtube.com/watch?v=NIqgr3AF3VE>

here's a pull-quote from it

> I really hope it's not the next Google because it is designed to come up with plausible sounding strings and that doesn't mean it's right and that doesn't mean you can go and find out where that information came from, so if people start using it as a source of information we're going to be worse off than we are now

and another good bit about whether she's worried about chatGPT being used to cheat

> so I'm not scared because I don't see the point of writing essays as producing the form of an essay and if students are turning to this out of desperation then the problem has happened earlier. we need to be supporting students so that they have the time to get their work done, so that they can feel comfortable asking questions. and if students are turning to some fallback to get an essay done&#x2014;gpt or another human&#x2014;the problem was upstream

really you should just watch the whole thing.

(Also I'd be remiss to not point out that the "stochastic parrots" paper she co-authored last year is open-access:  <https://dl.acm.org/doi/10.1145/3442188.3445922>

abstract:
\#+begin<sub>quote</sub>
The past 3 years of work in NLP have been characterized by the development and deployment of ever larger language models, especially for English. BERT, its variants, GPT-2/3, and others, most recently Switch-C, have pushed the boundaries of the possible both through architectural innovations and through sheer size. Using these pretrained models and the methodology of fine-tuning them for specific tasks, researchers have extended the state of the art on a wide array of tasks as measured by leaderboards on specific benchmarks for English. In this paper, we take a step back and ask: How big is too big? What are the possible risks associated with this technology and what paths are available for mitigating those risks? We provide recommendations including weighing the environmental and financial costs first, investing resources into curating and carefully documenting datasets rather than ingesting everything on the web, carrying out pre-development exercises evaluating how the planned approach fits into research and development goals and supports stakeholder values, and encouraging research directions beyond ever larger language models.
\#+end<sub>quote</sub>)

Okay, so Emily brings up her concern that people will attempt to treat things like chatGPT like the next google search and that's not a hypothetical fear.

Microsoft is partnering with OpenAI to add chatGPT to their bing engine: <https://www.bloomberg.com/news/articles/2023-01-04/microsoft-hopes-openai-s-chatbot-will-make-bing-smarter>

There's also a company called you.com (<https://you.com/>) that's attempting to build a chatGPT-like interface to their search engine. Much like chatGPT, though, their interface doesn't include any kind of attribution or way of exploring the actual space of the answers. Another company in this space is <https://www.perplexity.ai/> and I'm sure there are a number of others that have cropped up in just the past few weeks. 

Here's Gary Marcus, the writer with maybe the most intense love-hate relationship with AI ever, giving his thoughts about whether these models can be useful as search replacement: <https://garymarcus.substack.com/p/is-chatgpt-really-a-code-red-for>

Caveat lector: I think Gary has some interesting points here but is also a little "okay, boomer". You'll see what I mean.

But, okay, having shared all of this material maybe it's time for a little synthesis and for my own thoughts.

First, I think that trying to ban these tools in educational contexts is just an inherently bad idea. I both agree with Tao that we should be looking at this as an opportunity to ask more difficult and interesting questions. I also agree with Bender that I think if students see the need to use a large language model (LLM) in order to finish their assigments, something has gone terribly wrong already that should be addressed at a deeper level.

Where I personally differ from both a little bit is that I just largely don't think people are ready to use tools like chatGPT nor do I think the user interface is where it needs to be to actually be useful for information management. I think there isn't enough education yet around LLMs and what they really are&#x2014;as Bender put it so well, chatGPT is a text synthesis engine&#x2014;for the average person to understand what why sometimes it produces the right answer and why sometimes the text it generates is ridiculously wrong nor how to tell the difference easily. At the very minimum, I think you would need to

-   have the ability to assess confidence levels of generated text
-   generate (and validate as existing) citations on the topic that can be used to double check the information

in order to make such a tool useful beyond something that can help you remember things you already knew at some point or have enough expertise to check

Even if we did that, though, there's still some other problems that are a little more philosophical in nature. How much objectivity is even possible? If a chatGPT system provides an answer is that really "the" answer? There are obviously a lot of questions where "the" answer is very subjective, depending on assumptions and axioms that can dramatically change interpretation of facts.  

This gets to the question of "the view from nowhere", whether there can be a point of view that is inherently objective. And even further whether or not you believe such a thing can exist it's somewhat obvious that the idea of objectivity has been weaponized to marginalize others.

And this isn't an idle question either: it affects the very nature of what we do in this space. I think the two extremes are either that that we try to eliminate bias so that a future gpt6 is a completely objective source of accurate information or that we completely abandon the project of LLMs for information management.

I think my views in between the two and this is where I tie it back into educational contexts. I think these tools can be useful but only with enough literacy to understand their limitations, to adapt them to our needs, and to be fully capable of being independent of them when they fail.

So those are my thoughts.

What are yours?
