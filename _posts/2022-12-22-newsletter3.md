---
layout: post
title:  "AICC Newsletter 3: Sustainability"
date:   2022-12-22 18:49:32 -0800
categories: newsletter permacomputing
---

Hi again!

Here we are in our third AI/ML newsletter for the term and the theme of this week is going to be *sustainability* and the resources used by machine learning.

I've been thinking about this ever since the ceo of OpenAI said that the cost of operating chatgpt is "eye-watering"
<https://twitter.com/sama/status/1599669571795185665>

The cost of training or using a machine learning model, of course, is essentially the cost of the energy used the run the computers. The cost of the energy is thus proportional to the environmental impact of the model.

So I don't know about you but I hear that costs are "eye-watering" and my immediate thought is "oh no, how much carbon emission **is** this exactly?".

Understanding the resource usage of modern big-scale machine learning is still very much in its infancy and at the moment relies on private organizations self-reporting on training and inference costs. We know that stable-diffusion cost $600k to train because Stability AI told us. Meanwhile we&#x2014;as far as I can tell unless it was in a poorly circulated press release&#x2014;only have estimates of OpenAI products like dall-e2 (estimated to be upwards of $1M) and gpt-3 (estimated to have cost at least $4.6M but possibly on the order of $10M).

That doesn't mean, though, that there aren't a lot of people in the ML community who care about this! Huggingface has been doing research on estimates and has started even including data on carbon costs along with hosted models in order to&#x2014;and this is absolutely wild to me---**let you search for models to use by estimated carbon emissions in grams**
<https://huggingface.co/blog/carbon-emissions-on-the-hub>

They even have a semi-automated way of keeping track of carbon emissions for your code if you're using their infrastructure for training and using models!

But this opens a lot of questions about the use of large models, especially in the rush to build both toys and tools on top of things like github's copilot or openai's chatgpt. To even run gpt-3 once it's trained would require ~$50k worth of GPUs shared between multiple computers. That's a lot of upfront cost and resources just to run a single&#x2014;albeit impressive&#x2014;service. Having to build and buy new computers is also, with the exception of very low-power architectures, always environmentally worse than 

There's two obvious directions for improving the sustainability of things: reduce the amount of resources used or find a better way to use the resources we have. We'll talk about the second, first, because I think it's the most well-explored. Distributed computing is the process of splitting big computational jobs between multiple machines and collating the results back together, in an automated way. Note I say "automated" not "automatically" in that you will probably have to do a little work to make your code work with a distributed computing framework but, once you have, then you can split the job into pieces and farm them out between different machines.

As a personal connection, my first research group back in the day used distributed computing for particle physics simulations over machines across the entirety of the UW Madison campus. It turns out, though, that this project&#x2014;Condor&#x2014;still exists and has actually pivoted to distributed computing for machine learning! <https://research.cs.wisc.edu/htcondor/>

In more immediate machine learning and distributed computing success Eleuther (<https://www.eleuther.ai/>)&#x2014;a big actually open source organization&#x2014;has had a lot of success using mesh-tensorflow (<https://github.com/tensorflow/mesh>) to train their own competitor to gpt-3: gpt-neox (<https://blog.eleuther.ai/announcing-20b/>, <https://github.com/EleutherAI/gpt-neox>)

And of course this makes me think of eons and eons ago, back I used to leave projects like Folding@Home (<https://foldingathome.org/?lng=en-US>, <https://en.wikipedia.org/wiki/Folding@home>) running on my ps3, and whether we might one day be able to having training large models be a collective work of humanity rather than something only a few organizations can afford to do. Unshockingly, there are other people who've been wondering about this too: <https://learning-at-home.github.io/>

If you check out the above site this is still very much a project in its infancy but wouldn't it be neat to use across a bunch of machines across a community college system that has multiple campuses? Just a random example.

But, okay, what about just making models *smaller*? I mean we already know that just making models bigger and bigger isn't necessarily making them better. Chinchilla is a recent model that is still **large**, don't get me wrong, but it's less than half the size of gpt-3 and performs better (<https://towardsdatascience.com/a-new-ai-trend-chinchilla-70b-greatly-outperforms-gpt-3-175b-and-gopher-280b-408b9b4510>). I cannot stress enough that we don't actually know what the "right" number of parameters should be for things like these large language models. It's entirely possible, maybe even likely, that they're so big not because they have to be but because we need that big of a hammer to force the circle through the triangular hole.

Which brings me to a paper an internet-friend once shared with me: Playing Atari with Six Neurons <https://arxiv.org/abs/1806.01363>. This paper is about how, by being more clever in the design of the system, they created a neural network that can play an old atari video game that is just absolutely **tiny**. They basically trade up-front engineering for the creation of very small final models. And while the specific technique they use probably won't apply to things like a future micro-gpt, maybe that core lesson will!

The last thing I wanted to share about sustainability, and perhaps better context for why all these things are on my mind, is that I come from the permacomputing scene (<https://permacomputing.net/>) where we're concerned with how to create a world where computers are long-term artifacts that last decades and not disposable quantities. The idea, to me, is that we want to not only reduce future electronic waste, make better use of the computers that already exist so they don't rot in landfills, but also make computing more financially accessible for everyone by reducing the hardware requirements for participation in this shared computational infrastructure. I have **a lot** of thoughts on this topic, if you can't tell!

So now with the heavy stuff out of the way here's some of the links shared by faculty members this week:

-   Emmanuel shared this announcement <https://blog.tensorflow.org/2022/12/introducing-simple-ml-for-sheets.htm>, which is a legitimately cool product that allows for machine learning models to be built from tabular data *inside* the google spreadsheet
-   Carol shared this explainer for diffusion models from WaPo <https://www.washingtonpost.com/technology/interactive/2022/ai-image-generator/>
-   Station shared riffusion, a cute little toy that uses stable-diffusion fine-tuned on captioned spectrograms of music to create new spectrograms as images that can then naturally be converted into sound! <https://www.riffusion.com/> Yes, that's right, it generates *images* that can then be interpreted as *sound*. That's just a really fun and creative use of stable-diffusion

Okay, and with that I'll leave y'all for the holidays!
