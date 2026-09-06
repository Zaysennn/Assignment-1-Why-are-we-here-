# Assignment-1-Why-are-we-here-
ChiSang Cheng's Assignment 1 for SD5913.

## The Last 20%: Why I Still Learn Programming

I am a game developer and level designer. I use Unreal Engine Blueprints with an AI assistant connected through MCP to build gameplay prototypes, and GPT to analyse design documents and game breakdowns. AI already does work I previously had to do myself. My reason for learning programming is therefore practical: **I need to understand, evaluate, and improve the systems that AI generates.** The ability to produce a framework quickly does not guarantee that I can finish it, or even recognise what remains unfinished.

## Fast beginnings, difficult endings

My rough description of working in a familiar field is that AI can take me from 0% to 80% of the basic implementation in about 5% of the development time. I then spend the remaining 95% using professional knowledge to refine the final 20%. Taking that familiar workflow's total time as 100%, I suspect that entering an unfamiliar field with AI could consume 150% or even 200%, yet leave me at only 80–90% completion, struggling with the final 10%. These are personal estimates and a hypothetical comparison, not measured productivity statistics. They describe how quickly apparent progress can turn into prolonged uncertainty.

The difficulty is often knowing where to look. Across my prototyping work, incorrect node parameters, object configurations, materials, and collision settings have caused problems. Without some understanding of these areas, I might keep requesting changes without knowing whether the assistant is investigating the relevant part of the system.

## A trap that could not kill the player

While developing a 3D platforming demo, I asked AI to create a trap. Touching it should kill the player immediately and respawn them at the nearest checkpoint. The assistant generated most of the logic, but during testing I discovered that the player could not interact with the trap.

I asked AI to diagnose the fault. It repeatedly checked and modified the code without resolving the problem. Eventually, I inspected the setup myself and found that the trap's collision box and the necessary collision detection configuration for its model had been omitted. After I added them, the mechanic worked.

This experience changed what I considered a complete implementation. A convincing sequence of logic was insufficient when the conditions needed to trigger it were missing. The problem required looking beyond the code that the assistant kept revising. My contribution was to identify a missing connection between the gameplay logic and its configuration in the scene.

Simply noticing a broken mechanic did not require programming knowledge; any playtester could have reported it. The value of technical understanding was being able to narrow the investigation and intervene. Blueprint work combines logic with engine configuration, and [Epic Games (n.d.)](https://dev.epicgames.com/documentation/en-us/unreal-engine/blueprints-visual-scripting-in-unreal-engine) describes Blueprints as a complete gameplay scripting system using a node-based interface. Learning programming in this context includes understanding how events, objects, and conditions connect. It gives me ways to test an explanation instead of repeatedly asking for another attempt.

## Professional vocabulary as a key

After roughly a year of using AI, I think of professional terminology as a key to a treasure chest. Knowing the relevant concept often helps me obtain a more precise explanation or implementation. Recognising collision detection as a possible source of failure gives me a much more useful starting point than repeatedly reporting that the trap does not work.

I experience a similar pattern when using GPT to analyse design documents. In areas I understand, I can ask focused questions, challenge answers, and select useful ideas through successive conversations. However, knowing a term is only an entry point. I also need to understand its relationships to other concepts and determine whether an answer fits the actual problem. Otherwise, a more technical answer may merely sound more convincing.

This connects reading with specifying. Reading a generated system helps me identify what it does and where it might fail; that understanding then improves what I ask AI to change. The ability to ask better questions grows alongside the ability to evaluate the answers.

## What should survive automation?

In *The Art of Code*, [Beattie (2020, 22:11–24:43)](https://www.youtube.com/watch?v=6avJHaC3C2U&t=1331s) presents an artist discussing tool limitations, experimentation, and rapid feedback, followed by a photograph reconstructed through depth analysis and layered processing. I connect this example to my own use of AI: faster iteration expands what I can attempt, while understanding the medium helps me direct those attempts. The talk's account of programming as creative expression supports this connection, although it does not prove that every designer needs the same technical depth.

There is also a reasonable objection to my argument: a better AI system might identify and repair that collision problem immediately. My experience does not establish a permanent limit on AI, and AI can help beginners learn. I therefore do not argue that everyone must memorise syntax or manually build every component. For my practice, the priority is enough knowledge to trace behaviour, inspect configurations, test assumptions, and judge whether a proposed solution serves the intended gameplay.

I want AI to keep accelerating the first 80%. I am learning programming so that I can make informed decisions about the rest, including when to accept its work and when to intervene. Professional knowledge helps turn fast generation into a mechanic that actually works within my design.

## References

Beattie, D. (2020, January 31). [*The art of code*](https://www.youtube.com/watch?v=6avJHaC3C2U) [Conference presentation]. NDC London, London, United Kingdom.

Epic Games. (n.d.). [*Blueprints visual scripting*](https://dev.epicgames.com/documentation/en-us/unreal-engine/blueprints-visual-scripting-in-unreal-engine). Unreal Engine documentation.
