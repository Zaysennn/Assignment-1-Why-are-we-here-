# Assignment-1-Why-are-we-here-
ChiSang Cheng's Assignment 1 for SD5913.

## Direction: Reading versus writing. If a machine writes the code, someone still has to know whether it is any good. What does it take to be that someone?

If AI builds a system, what must I understand to judge its quality? I will also explore “The gap between describing and specifying”, because technical understanding shapes the questions I can ask.

As a game developer with level designer. I use Unreal Engine Blueprints with an AI assistant connected through MCP to prototype gameplay, and GPT to analyse game design documents and game breakdowns. AI already handles much of the work I previously did myself. My reason for learning programming is practical: I need to understand, evaluate, and improve AI-generated systems. Quickly generating a framework does not mean I can finish it, or even recognise what remains unfinished.

### Fast beginnings, difficult endings

When I first started using AI-assisted development, I was excited by how quickly it could implement gameplay mechanics. A standard mechanic that previously took me an hour or even a full day to work out could appear almost immediately.

However, adding more features exposed conflicts during playtesting. Separately generated mechanics did not always integrate properly. This taught me the importance of planning the overall architecture and interactions between systems, rather than adding features whenever a new idea came to mind.

In fields I know well, AI seems able to take basic implementation process from 0% to 80% in about 5% of the development time. I then spend the remaining 95% time applying professional knowledge to debug, integrate, and refine the final process of 20%.

Taking that familiar workflow’s total time as 100%, I felt that working in an unfamiliar field with AI could consume time of 150% or even 200% more, and yet leave me at only 80–90% completion process with stuck on the final 10%. These are personal estimates and a hypothetical comparison, not measurements. Fast initial progress can turn into prolonged trial and error.

The difficulty is often knowing where to look. I have encountered problems with node parameters, object configurations, materials, and collision settings. Without understanding these areas, I could keep requesting changes without knowing whether AI is investigating the actual cause.

### A little personal experience - Unreal MCP+AI

While developing a 3D platforming demo, I asked AI to create a trap: on contact, the player should die immediately and respawn at the nearest checkpoint. AI implemented most of the logic, but testing revealed that the player could not interact with the trap.

I asked AI to troubleshoot it. It repeatedly inspected and modified the code without resolving the issue. Eventually, I checked the configuration myself and discovered that the trap's collision box and the necessary collision detection settings for its mesh were missing. After I added them, the mechanic worked.

This experience changed my understanding of “complete”. Without the conditions needed to trigger the logic, a seemingly complete implementation could not function. Resolving the issue required examining more than the code AI kept revising. My contribution was identifying a missing connection between gameplay logic and scene configuration.

Any playtester could notice that the mechanic was broken; that alone required no programming knowledge. Technical understanding helped me narrow the investigation and make an effective fix. Blueprints combine programming logic with engine configuration, and [Epic Games](https://dev.epicgames.com/documentation/unreal-engine/blueprints-visual-scripting-in-unreal-engine?lang=en-US) defines them as a complete gameplay scripting system using a node-based interface. For me, learning programming includes understanding how events, objects, and conditions connect. This helps me test a diagnosis instead of repeatedly asking AI to try again.

### The 'Terms' as a key

After using AI for some time, I see 'terms' as a key to a “treasure chest”. Understanding relevant concepts often helps me obtain more precise explanations or implementations. Identifying a particular logic flow or subsystem as a possible source of failure is more useful than repeatedly saying, “This does not work.”

I have similar experiences using GPT to analyse design documents. In familiar areas, I can ask specific questions, challenge answers, and select useful ideas through multiple rounds of discussion. However, knowing terminology is only a starting point. I also need to understand how concepts relate and whether an answer fits the actual problem. Otherwise, a more technical answer may simply sound more convincing.

This connects reading code with specifying requirements. Understanding an AI-generated system helps me identify its behaviour and possible failure points, then request more precise changes. Asking better questions and evaluating answers are abilities that develop together.

Better questions can also improve human–AI collaboration and, with usage-based billing, reduce costs by avoiding unnecessary exchanges. I cannot place all my hopes in increasingly powerful AI models. Without effective communication, it could be like hiring a team of aerospace engineers to diagnose and fix “Hello world” code: substantial expertise is available, but it is poorly directed. Professional knowledge helps me use that capability more purposefully.

### What should survive after AI-automation?

In [The Art of Code, Beattie (2020, 22:11–24:43)](https://www.youtube.com/watch?v=yDB3wbkfEeI&t=1331s) introduces an artist discussing tool limitations, experimentation, and rapid feedback, followed by a photograph reconstructed through depth analysis and layered processing.

I connect this example to my AI workflow: faster iteration expands what I can attempt, while understanding the medium helps me guide those attempts. The talk shows how programming can become a form of creative expression, but does not establish that every designer needs the same depth of technical knowledge.

My argument also faces a reasonable objection: a more capable AI model might immediately identify and fix deeper issues that currently require human review. My experience does not prove that AI has permanent limitations.

I think everyone do not need to memorise every aspect of syntax or build every component manually. In my practice, what matters more is having enough knowledge to trace gameplay behaviour, inspect configurations, test assumptions, and judge whether a solution supports the intended gameplay.

I want AI to keep accelerating the first 80% of the work. I learn programming to make informed decisions about the rest, including when to accept AI’s output and when to step in myself. Professional knowledge helps me turn quickly generated content into something that actually serves my design.

### References

Beattie, D. (2020, January 31). The art of code [Conference presentation]. NDC London, London, United Kingdom.

Epic Games. (n.d.). Blueprints visual scripting. Unreal Engine documentation.
