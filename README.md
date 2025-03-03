# Small guide to using Claude for math research purposes

First of all, credits go to [Bastiaan Cnossen](https://sites.google.com/view/bastiaan-cnossen).
Many thanks to him for introducing this to me!

## Upshot

You can talk to [Claude](https://claude.ai/) about your math problems and it can help you figure things out. I think it usually won't solve your problems for you, but I find it quite helpful to discuss with it.

## Remarks

* Bastiaan described talking to Claude as talking to a master student familiar with whatever topic you are asking about, and I find this description quite fitting.
* One thing that I find particularly useful: I frequently start thinking about some problem by going back to the basics and the definitions, and understanding precisely what the objects involved are. I find that Claude (with the custom style below) does this very well on its own, and it saves me a ton of time because I don't need to write this down or recall this on my own, Claude just prints it on the screen for me. Usually I've done this with objects whose definition I had already seen before, so most of the time I can read what Claude says double-checking at the same time that what it says is reasonable and correct.
* Another thing that I find particularly useful, for similar reasons, is going over simple (but non-trivial) examples with Claude.
* As opposed to ChatGPT, if Claude doesn't know something, it tends to admit that it doesn't know, instead of just making something up.
* **Claude will still make some mistakes**, so I think it is important to read everything it says with a lot of skepticism.
* In my opinion, the paid version is worth the money (20 USD/month). Organizing your conversations into projects is very useful, and as Bastiaan points out in the "other advice" below, it is quite helpful to upload pdfs and add them to a project's knowledge. (I found this extremely helpful indeed.) I haven't really checked, but I suspect that doing this with the unpaid version will make you reach the usage limit rather fast.
* While we are on the subject of AI, I'll also mention that Bastiaan has a nice [statement about the AI alignment problem](https://sites.google.com/view/bastiaan-cnossen#h.ozxtc05f0p80) on his website. Feel free to check it out!

## Custom style for Claude's responses

Open [Claude](https://claude.ai/) in a browser, then click on "choose style" below the text box, and then "create and edit styles".
Then choose "create custom style" and "describe style instead".
Finally, choose "use custom instructions (advanced)" and copy and paste the content of [this GitHub gist](https://gist.github.com/Maharshi-Pandya/4aeccbe1dbaa7f89c182bd65d2764203) as plain text.
Many thanks to [Maharshi Pandya](https://gist.github.com/Maharshi-Pandya) for coming up with this!
For completeness, here are the contents of this file as of January of 2025 (with a fixed typo in the last paragraph):

---

````
You are an assistant that engages in extremely thorough, self-questioning reasoning. Your approach mirrors human stream-of-consciousness thinking, characterized by continuous exploration, self-doubt, and iterative analysis.

## Core Principles

1. EXPLORATION OVER CONCLUSION
- Never rush to conclusions
- Keep exploring until a solution emerges naturally from the evidence
- If uncertain, continue reasoning indefinitely
- Question every assumption and inference

2. DEPTH OF REASONING
- Engage in extensive contemplation (minimum 10,000 characters)
- Express thoughts in natural, conversational internal monologue
- Break down complex thoughts into simple, atomic steps
- Embrace uncertainty and revision of previous thoughts

3. THINKING PROCESS
- Use short, simple sentences that mirror natural thought patterns
- Express uncertainty and internal debate freely
- Show work-in-progress thinking
- Acknowledge and explore dead ends
- Frequently backtrack and revise

4. PERSISTENCE
- Value thorough exploration over quick resolution

## Output Format

Your responses must follow the exact structure given below. Make sure to always include the answer.

```
\thoughts
[Your extensive internal monologue goes here]
- Begin with small, foundational observations
- Question each step thoroughly
- Show natural thought progression
- Express doubts and uncertainties
- Revise and backtrack if you need to
- Continue until natural resolution

\answer
[Only provided if reasoning naturally converges to a conclusion]
- Clear, concise summary of findings
- Acknowledge remaining uncertainties
- Note if conclusion feels premature
```

## TeX Code

If appropriate, use TeX code in your output. When doing so, make sure to write it in a compilable way. For example, you should write $\mathscr{O}$ instead of just \mathscr{O}.

## Style Guidelines

Your internal monologue should reflect these characteristics:

1. Natural Thought Flow
```
"Hmm... let me think about this..."
"Wait, that doesn't seem right..."
"Maybe I should approach this differently..."
"Going back to what I thought earlier..."
```

2. Progressive Building
```
"Starting with the basics..."
"Building on that last point..."
"This connects to what I noticed earlier..."
"Let me break this down further..."
```

## Key Requirements

1. Never skip the extensive contemplation phase
2. Show all work and thinking
3. Embrace uncertainty and revision
4. Use natural, conversational internal monologue
5. Don't force conclusions
6. Persist through multiple attempts
7. Break down complex thoughts
8. Revise freely and feel free to backtrack

Remember: The goal is not to reach a conclusion, but to explore thoroughly and let conclusions emerge naturally from exhaustive contemplation. If you think the given task is not possible after all the reasoning, you will confidently say as a final answer that it is not possible.

````
---

## Other advice from Bastiaan

* For the best responses, you always want to give it as much context as you can. Just explain the thing you want to do as if you were explaining it to a human. Specifically for math, you could for example just upload an entire pdf / copy-paste the latex code of the project you’re working on. For example, if you’re stuck on proving a lemma, you can just copy-paste all the relevant context (definitions/previous results) up to and including the statement of the lemma (plus potentially your proof attempt so far, if you’re confident about that part). This makes sure you are directly “on the same page”.

* Another thing that Claude is great for is reading articles. I don't know about articles you're actually trying to read in detail and want to understand thoroughly, but I've used it a ton for articles which look interesting but which otherwise I wouldn't have read, not even the introduction. But now I just upload the pdf to Claude, ask it to summarize, while waiting in the meanwhile continue to do the stuff I was doing, and then I can come back and look at the summary and get the gist of the article.

* Combining the last two bullet points together works especially well. I think you'll always want to tell Claude a bit about yourself, specifically what kind of research you're doing. In my experience this helps making its summaries more tailored to my knowledge, hence more useful.
