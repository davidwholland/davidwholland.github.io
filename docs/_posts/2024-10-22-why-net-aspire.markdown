---
layout: post
title:  "Why .NET Aspire?"
date:   2024-10-22 13:56:26 -0400
tags: dotnet programming
---
In 1980, Microsoft was awarded a contract to provide an operating system that would come to be known as MS-DOS for IBM personal computers. Over the next four decades, Microsoft came to dominate much of the IT industry, first with Windows and eventually with the Office suite of products.

As technology proceeded apace, the company worked hard to respond as the ground moved beneath them. The famous memo by Microsoft founder Bill Gates called [The Internet Tidal Wave][famous-memo] served to rally the troops by driving home the magnitude of the paradigm shift that was coming.

When Amazon launched what became [Amazon Web Services][aws] (AWS) in the mid-2000s, Microsoft quickly began moving to build their own competing platform called [Azure][azure]. Both companies had learned much from managing large enterprise data centers, and they were successful in convincing the IT industry that companies with far more modest infrastructure needs could still benefit from moving their operations to the cloud. AWS and Azure were able to capitalize on this idea, and the result was stupendously profitable.

As the tech industry as a whole latched on to this new way of working, software engineers had to reexamine the practices and tools they used to deliver software. The cloud's big selling point was that it made scaling an application easier than it had ever been. But someone still had to build the applications. And the cloud introduced systems and workflows that brought a flood of new technologies that had to be learned.

Well-architected cloud applications make use of a number of features that already existed but were perhaps not as commonly used in smaller, less mature engineering teams. To pick just one example: patterns like continuous integration and continuous development (CI/CD) became full-blown systems with their own tools, languages, file formats, security contexts, and monitoring needs.

As engineers tried to assimilate the vast number of new concepts and tools that seemed to appear weekly, some began to complain that the levels of complexity were rapidly exceeding what could reasonably be understood by an individual developer. 

That presented a problem. It was no exaggeration to say that Microsoft had become, for all intents and purposes, a cloud company. That is to say: most of its revenue and much of its hope for future growth were tied to the success of the cloud as a platform. If developers were to lose enthusiasm for cloud development due to an overly steep learning curve, that would sound a warning that would disturb even Satya Nadella's sleep.

This isn't an idle worry. In addition to the complexity inherent in developing for the cloud, cost is another major factor that can dampen the zeal of even very successful companies. 37signals, the company known for their project management software called Basecamp, has made it clear that the shine of cloud computing has truly worn off for them. One of the cofounders of the company, David Heinemeier Hansson, says that they expect to [save more than $10 million over the next five years][dhh] as a result of moving to on-premises servers that they manage themselves.

So what's a $3 trillion company to do? The answer of course is to make it as easy as possible for developers to get their applications into the cloud and then make sure they stay there. 

And that brings us to .NET Aspire.

[famous-memo]: https://lettersofnote.com/2011/07/22/the-internet-tidal-wave/
[aws]: https://aws.amazon.com
[azure]: https://azure.microsoft.com/en-us/
[dhh]: https://world.hey.com/dhh/our-cloud-exit-savings-will-now-top-ten-million-over-five-years-c7d9b5bd