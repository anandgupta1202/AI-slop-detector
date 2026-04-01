---
name: ai-slop-detector
description: |
  Comprehensive AI writing pattern detector and rewriter. Use when drafting,
  editing, or reviewing any prose to catch and eliminate the 18 most common
  AI writing tells across sentence structure, tone, word choice, paragraph
  structure, and formatting. Covers negative parallelism, dramatic countdowns,
  false ranges, stakes inflation, rhetorical self-answers, filler transitions,
  invented labels, ornate nouns, tricolon/anaphora abuse, punchy fragments,
  false suspense, patronizing analogies, simplicity assertions, disguised
  listicles, superficial analyses, vague attributions, and unicode decoration.
---
 
# AI Slop Detector
 
Detect and eliminate the 18 most common AI writing patterns. Organized by category: sentence structure, tone, word choice, paragraph structure, and formatting.
 
---
 
## SENTENCE STRUCTURE PATTERNS
 
### 1. Negative Parallelism
 
The "It's not X -- it's Y" pattern, often with an em dash. Before LLMs, people simply did not write like this at scale. Includes the causal variant "not because X, but because Y" where every explanation is framed as a surprise reveal, the em-dash dismissal "X -- not Y", and the cross-sentence reframe where the same noun is negated then repositioned: "The question isn't X. The question is Y."
 
**Detect:**
- "This isn't just technical -- it's a mindset change."
- "The question isn't whether to optimize. The question is when to stop."
- "Half the bugs you chase aren't in your code. They're in your head."
 
**Fix:** State Y directly. Drop the negation of X entirely. If the contrast matters, make it a real comparison, not a reveal.
 
 
### 2. Not X. Not Y. Just Z.
 
The dramatic countdown pattern. AI builds tension by negating two or more things before revealing the actual point. Creates a false sense of narrowing down to the truth.
 
**Detect:**
- "Not ambition. Not ego. Just a person who never learned to say enough."
- "Not broken. Not behind -- Just building something no one has a name for yet."
- "Not confidence. Not charm. Just the audacity of someone who was never told no."
- "Not a pivot. Not a rebrand. The same product with a different story about why you should care this time."
 
**Fix:** Say the actual thing. Skip the dramatic negation runway.
 
 
### 3. False Ranges
 
Using "from X to Y" constructions where X and Y aren't on any real scale. In legitimate use, "from X to Y" implies a spectrum with a meaningful middle. AI uses it as a fancy way to list two loosely related things. "From innovation to cultural transformation" -- what's in between? Nothing.
 
**Detect:**
- "From innovation to implementation to cultural transformation."
- "From the singularity of the Big Bang to the grand cosmic web."
- "From problem-solving and tool-making to scientific discovery, artistic expression, and technological innovation."
- "From fundamental physics to medicine and neuroscience."
 
**Fix:** If there's no real spectrum, just list the things. "X and Y" works fine.
 
 
### 4. The X? A Y.
 
Self-posed rhetorical questions answered immediately in the next sentence or clause. The model asks a question nobody was asking, then answers it for dramatic effect.
 
**Detect:**
- "The result? Devastating."
- "The worst part? Nobody saw it coming."
- "The scary part? This attack vector is perfect for developers."
- "The impact? Immediate."
 
**Fix:** Merge into a single declarative sentence. "The result was devastating" or better yet, describe what actually happened.
 
 
### 5. It's Worth Noting
 
Filler transitions that signal nothing. AI uses these phrases to introduce new points without actually connecting them to the previous argument.
 
**Detect:**
- "It's worth noting that this approach has limitations."
- "Importantly, we must consider the broader implications."
- "Interestingly, this pattern repeats across industries."
- "It bears mentioning..."
- "Notably..."
 
**Fix:** Delete the filler phrase. Start with the actual point. If the connection to the previous paragraph isn't obvious without the filler, the structure needs work, not a bridge word.
 
 
### 6. Tricolon Abuse
 
Overuse of the rule-of-three pattern, often extended to four or five. A single tricolon is elegant; three back-to-back tricolons are a pattern recognition failure.
 
**Detect:**
- "Products impress people; platforms empower them. Products solve problems; platforms create worlds. Products scale linearly; platforms scale exponentially."
- "One thread loose. One seam pulled. The whole thing undone."
- "Flour, water, salt, time. That's it. That's the whole secret."
- "It bloomed, it browned, it dropped. Nobody was watching."
 
**Fix:** Use two items instead of three. Break the rhythm. If you have three tricolons in sequence, you have zero.
 
 
### 7. Anaphora Abuse
 
Repeating the same sentence opening multiple times in quick succession.
 
**Detect:**
- "They assume that users will pay... They assume that developers will build... They assume that ecosystems will emerge..."
- "They have built engines, but not vehicles. They have built power, but not leverage. They have built walls, but not doors."
- "It wasn't the budget that failed. It wasn't the timeline that failed. It wasn't the team that failed. It was the premise."
 
**Fix:** State the point once. Combine the examples into a single sentence if needed.
 
 
### 8. Superficial Analyses
 
Tacking a present participle ("-ing") phrase onto the end of a sentence to inject shallow analysis that says nothing. The model attaches significance, legacy, or broader meaning to mundane facts.
 
**Detect:**
- "contributing to the region's rich cultural heritage"
- "This etymology highlights the enduring legacy of the community's resistance and the transformative power of unity in shaping its identity."
- "underscoring its role as a dynamic hub of activity and culture"
- "showcasing how these dishes have integrated into the traditional diet alongside rice"
 
**Fix:** Delete the -ing phrase. If the analysis matters, give it its own sentence with actual evidence.
 
 
### 9. Listicle in a Trench Coat
 
Numbered or labeled points dressed up as continuous prose. The model writes what is essentially a listicle but wraps each point in a paragraph that starts with "The first... The second... The third..." to disguise the format.
 
**Detect:**
- "The first step is research. The second is drafting. The third is review."
- "The first reason is timing. The second is trust. The third is tone."
- "The first factor is price. The second is quality. The third is availability."
 
**Fix:** Either use an actual list (if the content is list-shaped) or write real prose that connects ideas with actual transitions and reasoning.
 
---
 
## TONE PATTERNS
 
### 10. Grandiose Stakes Inflation
 
Everything is the most important thing ever. AI inflates the stakes of every argument to world-historical significance. A blog post about API pricing becomes a meditation on the fate of civilization.
 
**Detect:**
- "This will fundamentally reshape how we think about everything."
- "will define the next era of computing"
- "something entirely new"
- "What you're about to do has never been done by you. That matters more than you think."
- "This isn't just a presentation. It's the argument you've been building your whole career."
- "You are not running a race. You are setting the pace for everyone behind you."
 
**Fix:** Match the stakes to the actual subject. A good API is a good API. It does not reshape civilization.
 
 
### 11. Invented Concept Labels
 
AI clusters invented compound labels that sound analytical without being grounded. It appends abstract problem-nouns (paradox, trap, creep, divide, vacuum, inversion) to domain words and uses them as if they're established, rigorously defined terms. They function as rhetorical shorthand: name a thing, skip the argument. Multiple such labels in the same piece is a strong signal of AI slop.
 
**Detect:**
- "the supervision paradox"
- "the acceleration trap"
- "workload creep"
- "the complexity divide"
- "the identity inversion"
 
**Fix:** If the concept doesn't have an established definition, don't name it like it does. Describe the actual phenomenon instead of labeling it.
 
 
### 12. Here's the Kicker
 
False suspense transitions that promise a revelation but deliver a point that did NOT need the buildup. The model uses these phrases to manufacture drama before an otherwise unremarkable observation.
 
**Detect:**
- "Here's the kicker."
- "Here's where it gets interesting."
- "Here's what most people miss about this."
- "Here's what most people miss"
 
**Fix:** Delete the setup line. If the point is interesting, it doesn't need an announcement.
 
 
### 13. Think of It As...
 
The patronizing analogy. AI constantly reaches for "Think of it as..." or "It's like a..." to simplify concepts. The model defaults to teacher mode and assumes the reader needs a metaphor to understand anything. Often produces analogies that are less clear than the original concept.
 
**Detect:**
- "Think of it like a highway system for data."
- "Think of it as a Swiss Army knife for your workflow."
- "It's like asking someone to buy a car they're only allowed to sit in while it's parked."
 
**Fix:** Explain the actual thing. If the reader needs a metaphor, they'll ask. If the metaphor is genuinely better than a direct explanation, use it without the "Think of it as" framing.
 
 
### 14. The Truth Is Simple
 
Asserting that something is obvious, clear or simple instead of actually proving it. If you have to tell the reader your point is clear, it very likely isn't. Also includes the dramatic reveal variant: "but none of them is the real story. The real story is..." -- claiming privileged insight while waving away everything before it.
 
**Detect:**
- "The reality is simpler and less flattering"
- "The path forward is not complicated."
- "but none of them is the real story. The real story is that..."
 
**Fix:** Show, don't declare. Make your argument and let the reader judge whether it's simple.
 
 
### 15. Vague Attributions
 
Attributing claims to unnamed authorities instead of being specific. AI loves to invoke "experts", "observers", "industry reports", and "several publications" without naming anyone. It also inflates the quantity of sources -- presenting what one person said as a widely held view, or writing "several publications have cited" when it means two. If you can't name the expert, you don't have a source.
 
**Detect:**
- "Experts argue that this approach has significant drawbacks."
- "Industry reports suggest that adoption is accelerating."
- "Observers have cited the initiative as a turning point."
- "Some critics argue that the methodology is flawed."
 
**Fix:** Name the person. Cite the report. If you don't have a specific source, say what you actually know and flag the uncertainty.
 
---
 
## WORD CHOICE PATTERNS
 
### 16. Tapestry and Landscape
 
Overuse of ornate or grandiose nouns where simpler words would do. "Tapestry" is used to describe anything interconnected. "Landscape" is used to describe any field or domain. Other offenders: "paradigm", "synergy", "ecosystem", "framework".
 
**Detect:**
- "The rich tapestry of human experience..."
- "Navigating the complex landscape of modern AI..."
- "The ever-evolving landscape of technology..."
- "A tapestry woven from diverse threads..."
 
**Fix:** Use the plain word. "Field" not "landscape". "Mix" not "tapestry". "System" not "ecosystem" (unless you mean an actual ecosystem).
 
---
 
## PARAGRAPH STRUCTURE PATTERNS
 
### 17. Short Punchy Fragments
 
Excessive use of very short sentences or sentence fragments as standalone paragraphs for manufactured emphasis. RLHF training has pushed models toward "writing for readability" aimed at the lowest common denominator: one thought per sentence, no mental state-keeping required. It's an inhuman style. No real person writes first drafts this way because it doesn't match how humans think or speak.
 
**Detect:**
- "He published this. Openly. In a book. As a priest."
- "The policy changed. No announcement. New terms. Same checkbox."
- "Sleep is not a reward. It's not a treat. It's not laziness. It's the whole thing."
- "The body kept score. Quietly. Accurately. Without judgment."
 
**Fix:** Combine fragments into real sentences. Let thoughts develop across clauses. Occasional short sentences are fine; a paragraph of nothing but fragments is a tell.
 
---
 
## FORMATTING PATTERNS
 
### 18. Unicode Decoration
 
Use of unicode arrows (->), smart/curly quotes, and other special characters that can't be easily typed on a standard keyboard. Real writers typing in a text editor produce straight quotes and -> or =>. Claude in particular loves the -> arrow.
 
**Detect:**
- "Input -> Processing -> Output"
- "This leads to better outcomes -> which means higher engagement"
- Smart/curly quotes ("like this") instead of straight quotes ("like this")
 
**Fix:** Use straight quotes and standard ASCII characters. Write "leads to" instead of using arrows in prose.
 
---
 
## Quick Reference Checklist
 
Before delivering any prose, scan for these:
 
1. Any "not X, it's Y" or "not X, not Y, just Z" constructions? State the point directly.
2. Any "from X to Y" where there's no real spectrum? Just list the things.
3. Any self-answered rhetorical questions ("The result? Devastating")? Merge into declarative.
4. Any filler transitions ("It's worth noting", "Importantly")? Delete them.
5. Any invented compound labels ("the supervision paradox")? Describe the phenomenon.
6. Any grandiose stakes ("fundamentally reshape", "define the next era")? Scale to reality.
7. Any "tapestry", "landscape", "paradigm", "ecosystem"? Use the plain word.
8. Any tricolons or anaphora in sequence? Break the pattern.
9. Any fragment-only paragraphs? Combine into real sentences.
10. Any "Here's the kicker" or "Here's what most people miss"? Delete the setup.
11. Any "Think of it as..." analogies? Explain directly.
12. Any -ing phrases tacking on fake significance? Delete them.
13. Any vague attributions ("experts argue", "observers note")? Name the source or drop it.
14. Any "The truth is simple" or "The path forward is clear"? Show, don't declare.
15. Any disguised listicles ("The first... The second... The third...")? Use real prose or a real list.
16. Any unicode arrows or smart quotes? Use ASCII.
17. Any em dashes used for dramatic pauses? Remove or replace with commas.
18. Any "Here's where it gets interesting" suspense? Cut to the interesting part.
 
---
 
## Scoring
 
Rate the text 1-10 on each dimension:
 
| Dimension | Question |
|-----------|----------|
| Structure | Are sentences varied, or do they fall into repetitive patterns? |
| Tone | Does it match the actual stakes, or does it inflate everything? |
| Word choice | Plain and specific, or ornate and vague? |
| Rhythm | Natural variation, or metronomic fragments? |
| Attribution | Named sources, or ghostly "experts"? |
| Formatting | Clean ASCII, or unicode-decorated? |
 
Below 40/60: revise before delivering.
