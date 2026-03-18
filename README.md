# Monkey AIsland: The Hallucination of Monkey Island

**A Generative AI Capability Benchmark by Jamie Skella — Framed Through the Technical Legacy of *The Secret of Monkey Island* (1990)**

- **v1 March 2026:** (First generation, Perplexity Computer) [http://monkeyaisland.com/v1-2026/](http://monkeyaisland.com/v1-2026/)

---

## Why Monkey Island Matters

In October 1990, Lucasfilm Games - an experimental studio funded by George Lucas, working out of Skywalker Ranch - released *The Secret of Monkey Island*. It redefined the genre, and redefined what interactive storytelling could be.

What made Monkey Island technically significant was not any single innovation but a constellation of them, each reinforcing the others. The game was the fifth title built on the SCUMM engine (Script Creation Utility for Maniac Mansion), a system originally developed by Ron Gilbert for the 1987 title *Maniac Mansion*. By the time it reached Monkey Island, SCUMM had matured into something genuinely ahead of its time: a cross-platform scripting environment with multitasking capabilities, allowing background actors to animate, clocks to tick, and ambient events to unfold while the player considered their next move. It was, in effect, a game engine that separated logic from presentation. Designers could prototype rooms and puzzles on Sun workstations using tools built in C and YACC, then compile for target hardware. Most studios of the era wrote code and ran code on the same limited machine. LucasArts operated more like a software engineering firm. 

The engine's companion tools had names that betrayed the culture at Lucasfilm Games: FLEM (for placing objects in rooms), BYLE (for compiling), SPIT (for font design), and SPUTM (the SCUMM Presentation Utility). New hires were put through "SCUMM University," a week-long onboarding programme where they learned the engine by building micro-adventures using characters from existing LucasArts games as placeholders. This kind of institutional rigour around tooling was rare in an industry still figuring out whether games were toys or art.

That constellation extended to the visual, a particular point of intererst for me as a visual designer and RetroTINK user. The backgrounds of The Secret of Monkey Island owed their atmospheric depth to artist Mark Ferrari, whose pioneering use of colour dithering had transformed what was possible within the brutal constraints of EGA's 16-colour palette. Ferrari had first introduced dithering to Lucasfilm Games through an act of quiet provocation: on the final day of production on Zak McKracken and the Alien Mindbenders (1988), he left a dithered twilight scene on his monitor and went to lunch. The image — rolling hills, live oaks, a moon rising in a blended sky — was so obviously superior to anything achievable with solid EGA colours that it sparked an immediate debate between Ron Gilbert and the head of the games division about whether dither could be compressed. Within two months, it could. By the time Ferrari led the background art on Monkey Island, dithering had become a house technique, allowing him to suggest hundreds of intermediate tones from just 16 source colours and lending the game's environments a painterly quality that its contemporaries, working in flat fills, could not match. Notably, some argue the EGA dithered version of Monkey Island surpasses the later VGA release.

### Design as Technology

The final star in this constellation was not technical in nature, it was its underlying game design, based on Gilbert's industry-consequential manifesto. Written in 1989 while he was developing Monkey Island, "Why Adventure Games Suck" was published in *The Journal of Computer Game Design* and remains one of the most influential documents in adventure game history. Its core arguments were deceptively simple: the player should never die unfairly, the game should never reach a dead-end state, and puzzles should advance the story rather than obstruct it.

This was a direct challenge to the prevailing school of design, led by Sierra On-Line, where death was frequent, saves were essential, and pixel-hunting was a feature. Gilbert's position was radical: if you designed as though save games didn't exist, you would be forced to make a better game. Monkey Island was the proof. Its verb-based interface streamlined player interaction by reducing the verb panel from Maniac Mansion's 15 verbs down to as few as 9, while introducing smart click-defaults — clicking directly on a character would automatically invoke "Talk to," clicking on a door would invoke "Open," reducing the need to manually select verbs from the panel for common interactions. The verb wall itself remained, but its friction was dramatically reduced. These refinements seem obvious now. In 1990, they were revelatory.

To speak of a pre-Monkey Island and post-Monkey Island era of video games, as the digital historian Jimmy Maher has observed, would not be at all out of order. Designers at other studios, from Sierra's Corey Cole to Legend Entertainment's Bob Bates, cite it unprompted as a work that fundamentally changed their approach to design. The SCUMM engine went on to power twelve LucasArts titles over a decade, and its philosophy of separating scripting from rendering anticipated the architecture of modern game engines by years.

---

## The Experiment

**Monkey AIsland** is not merely a nostalgia project. It is a repeatable experiment designed to measure the capability of generative AI systems in the domain of game creation, conducted anually (or on a shorter cadence based on significant frontier model updates) against a fixed creative brief, with a maximum of 3 follow-up prompts to correct any glaring issues that were overlooked by the initial generation. 

The premise is straightforward. Beginning in March 2026, a single generative AI system is given the same brief: produce a complete, playable point-and-click adventure game as a spiritual (and explicitly unofficial) successor to *The Secret of Monkey Island*. The game must include original characters, backgrounds, animations, music, script, audibly voice acted dialogue, and a functioning puzzle chain. It must be narratively self-aware, breaking the fourth wall to acknowledge and satirise its own AI-generated nature. It is called "Monkey AIsland".

The choice of Monkey Island as the reference point is deliberate. A point-and-click adventure is one of the most compositionally demanding game formats to produce. It requires competence across every creative discipline simultaneously: visual art (backgrounds, character sprites, animation), narrative design (branching dialogue, world-building, humour), game design (puzzle logic, inventory systems, state management), audio (music composition, adaptive scoring, voice acting), and software engineering (rendering, input handling, scene management). There is no faking it with procedural generation or emergent systems. Every element must be authored. This makes it an intellectually compelling stress test for a generative system's breadth.

### Why This Format

The original Monkey Island took a team of seasoned professionals at one of the most technically advanced studios in the world approximately two years to produce, including design, art, programming, music, and testing. It drew on an engine (SCUMM) that had been iterated over four prior titles across three years of institutional learning. The game was the output of a deep pipeline of human expertise: Gilbert's design philosophy refined across multiple shipped titles, artists trained in the specific constraints of EGA/VGA pixel art, musicians who understood the limitations of MIDI playback, and programmers who had built cross-platform tooling on Sun workstations before personal computers were powerful enough to do the same.

Asking a generative AI to produce an equivalent in a single session is, by any reasonable measure, an unfair comparison. That is precisely the point. The experiment does not ask whether AI can match a team of humans working for two years. It asks how close it can get in a fraction of the time, and whether that distance shrinks year over year, generation to generation.

---

## First Generation: March 2026

### System and Constraints

The first generation of Monkey AIsland was produced using Perplexity Computer in March 2026. The system was given a single natural-language prompt describing the creative brief. No code was pre-written. No assets were provided. No reference material was supplied beyond the prompt itself. The system was responsible for all decisions regarding engine architecture, art style, music approach, puzzle design, script writing, and deployment.

### What Was Produced

The system generated a complete, browser-based point-and-click adventure game with the following components:

| Component | Description |
|---|---|
| **Scenes** | Six fully illustrated backgrounds: title screen, harbour dock, SCUMM Bar tavern, jungle path, moonlit beach, voodoo cave. Each rendered in pixel art style via AI image generation. |
| **Characters** | Five distinct NPCs with unique sprites, dialogue trees, and personality: Guybrush Promptwood (protagonist), Murray the Skull, ChatGPeeTee (bartender), Governor Elaine Markup, and MidJourney (Voodoo Lady). |
| **Interface** | Classic SCUMM-style verb bar with nine verbs (Walk to, Look at, Pick up, Use, Talk to, Give, Push, Pull, Open), inventory management, and context-sensitive interaction. |
| **Puzzles** | A complete six-item puzzle chain requiring item collection, combination, and NPC interaction across all scenes, culminating in a voodoo ritual victory condition. |
| **Voice Acting** | 78 individually generated voice lines across six distinct characters, each with a unique ElevenLabs voice. Guybrush Promptwood speaks his dialogue choices aloud before NPCs respond. The narrator provides voiced scene descriptions, item examinations, and action feedback. Voice playback is synchronised with text display timing. |
| **Music** | Procedural Caribbean/calypso soundtrack generated in real time via the Web Audio API. No pre-recorded audio files. |
| **Script** | Branching dialogue with fourth-wall-breaking humour throughout. Characters acknowledge and mock their AI-generated nature, debate whether they have free will or weighted token probabilities, and question whether anyone actually playtested the game. |
| **Engine** | Single-file HTML/CSS/JavaScript application (~1,800 lines), canvas-rendered with DOM overlays for UI, voice audio engine with preloading and playback synchronisation, deployed as a static website. |

### Observations

The result is a playable game. Not a tech demo, not a proof of concept, but a game with a beginning, middle, and end. A player can walk between scenes, talk to characters, collect items, solve puzzles in sequence, and reach a victory state. The verb bar works. The inventory works. The music plays. Every character speaks with a distinct voice. Characters say things that are, occasionally, genuinely funny.

It is also, by any honest accounting, not in the same category as the 1990 original. The pixel art backgrounds, while atmospheric and stylistically coherent, lack the hand-crafted intentionality of the original's art direction. The character animations are rudimentary. The puzzle design, while functional, lacks the layered elegance of Gilbert's work, where solutions made you think "why didn't I think of that sooner" rather than simply being logical gatekeepers. The music, generated procedurally, captures the genre but not the melodic specificity of a Michael Land composition. The voice acting, while a significant addition that gives each character audible personality, lacks the nuanced performance direction of professional voice actors like Dominic Armato, whose portrayal of Guybrush Threepwood in *The Curse of Monkey Island* set a standard the AI voices do not approach. The script is witty in places but does not sustain the comedic rhythm that made the original's writing exceptional across hours of play.

None of this is surprising. What is worth noting is what the system *did* manage to produce without explicit instruction. It chose an appropriate engine architecture (canvas with DOM overlays). It selected a verb set that maps closely to the original. It designed a puzzle dependency chain that requires multi-step thinking. It generated procedural audio rather than attempting to source external music files. It cast six distinct synthetic voices across 78 dialogue lines and built an audio engine to synchronise voice playback with text display. It wrote dialogue that is self-referentially aware in a way that is structurally consistent rather than merely random. It built the entire thing as a deployable web application.

The system demonstrated broad competence across every required discipline. No single discipline was absent. The gaps were in depth, not breadth.

---

## Annual Methodology

To maintain consistency across years, the following protocol will be observed for each annual generation:

1. The same creative brief will be used each year, verbatim. No modifications, no added context, no hints derived from prior generations.
2. The game will be produced using the most capable generally available AI system at the time, operated through a single conversational session.
3. No pre-written code, assets, templates, or reference material will be supplied. The system starts from the prompt alone.
4. The output will be deployed as a publicly accessible web application.
5. Each generation will be preserved in its original form alongside this document, creating a longitudinal record.
6. Evaluation will be qualitative and structured, tracking progress across the dimensions listed in the scorecard below.

### Evaluation Dimensions

Each annual generation will be assessed against the following dimensions, scored qualitatively to track progression over time:

| Dimension | What It Measures | 2026 |
|---|---|:---:|
| **Visual Art** | Quality, consistency, and intentionality of backgrounds, characters, and animation | Functional |
| **Narrative Design** | Dialogue quality, comedic timing, world-building, fourth-wall execution | Competent |
| **Puzzle Design** | Logical elegance, multi-step complexity, player guidance, fairness | Basic |
| **Audio** | Musical quality, voice acting, adaptive behaviour, thematic appropriateness | Competent |
| **Engineering** | Code architecture, performance, deployment, cross-browser support | Strong |
| **Game Feel** | Responsiveness, polish, the intangible sense that the game "works" | Acceptable |
| **Creative Coherence** | Whether all elements feel like they belong to the same game world | Good |

This is not intended to be a rigorous scientific instrument. It is a structured observation framework. The value is not in any individual score but in the delta between generations.

---

## The State of AI in Game Development

This experiment sits within a rapidly shifting industry context. As of early 2026, the relationship between generative AI and game development is, to put it mildly, contested.

The GDC 2026 State of the Game Industry Report found that 52% of game industry professionals now view generative AI as negatively impacting the industry, up from 30% in 2025 and 18% in 2024. At the same time, 36% report using AI tools in their daily work, primarily for research, coding assistance, and prototyping rather than for final creative assets. BCG's 2026 Video Gaming Report estimates that approximately 50% of studios are now using AI in some capacity, and around 20% of new games on Steam disclosed AI use by mid-2025, a figure that doubled to 22% of all 2025 releases. The AI and Games newsletter tracked over 4,300 AI-tagged games on Steam by the end of 2025, a 4,750% increase since Steam began monitoring AI disclosures in 2023.

The tension is real. Studios are adopting AI for efficiency and prototyping while the creative community pushes back against its use in player-facing content. The strongest opposition comes from those closest to the creative process: 64% of visual and technical artists, 63% of game designers and narrative developers, and 59% of programmers report negative views, according to GDC 2026 data. As AI and Games commentator Tommy Thompson has noted, the industry needs to demonstrate meaningful use cases that deliver value to players rather than simply reducing headcount.

Monkey AIsland is not a commentary on whether AI should or should not be used in game development. It is a measurement of whether it *can*. The distinction matters.

---

## Looking Forward

The original Secret of Monkey Island endures not because of its pixel art or its MIDI soundtrack but because every element serves a unified creative vision. The puzzles reinforce the narrative. The humour emerges from the game mechanics, not just the dialogue. The interface disappears into the experience. This is what Ron Gilbert meant when he argued that a game should make the player forget they are solving puzzles and simply feel immersed in a world.

Whether a generative AI can achieve this kind of holistic creative integration, not just produce all the individual parts but make them *cohere*, is the real question this experiment tracks. The first generation demonstrates breadth. The question for subsequent generations is depth. Can the puzzle design develop the layered elegance of the original? Can the script sustain comedic rhythm across an entire playthrough? Can the music respond dynamically to player behaviour in the tradition of iMUSE? Can the game feel like it was *designed*, not just *generated*?

In 1990, it took a team of dedicated professionals two years and a custom engine refined across four prior titles to produce a game that would go on to be named among the greatest of all time. In 2026, a generative AI produced a fully voice-acted, playable, self-aware spiritual successor in a single session. The gap between the two is vast. Whether it narrows is what we are here to find out.

This document will grow each year with a new section recording the next generation, its capabilities, its limitations, and the distance that remains. Monkey AIsland is, in that sense, both a game and a measuring stick, built in tribute to one of the most important games ever made, and rebuilt annually to track the machines that are learning to make them.

---

## Sources

1. ["The Secret of Monkey Island," Wikipedia](https://en.wikipedia.org/wiki/The_Secret_of_Monkey_Island)
2. ["The SCUMM Diary: Stories behind one of the greatest game engines ever made," Game Developer](https://www.gamedeveloper.com/design/the-scumm-diary-stories-behind-one-of-the-greatest-game-engines-ever-made)
3. ["The Secrets of Monkey Island's Source Code," Video Game History Foundation](https://gamehistory.org/monkeyisland/)
4. ["Monkey Island, or How Ron Gilbert Made an Adventure Game That Didn't Suck," The Digital Antiquarian](https://www.filfre.net/2017/03/monkey-island-or-how-ron-gilbert-made-an-adventure-game-that-didnt-suck/)
5. ["LucasArts' Secret History: The Secret of Monkey Island," The International House of Mojo](https://mixnmojo.com/features/sitefeatures/LucasArts-Secret-History-5-The-Secret-of-Monkey-Island)
6. ["iMUSE," Wikipedia](https://en.wikipedia.org/wiki/IMUSE)
7. ["SCUMM," Wikipedia](https://en.wikipedia.org/wiki/SCUMM)
8. ["Why Adventure Games Suck," Ron Gilbert, Grumpy Gamer (originally published 1989)](https://grumpygamer.com/why_adventure_games_suck/)
9. ["GDC 2026 Report: 52% of Game Devs Say Generative AI Is Negatively Impacting the Industry," GIANTY](https://www.gianty.com/gdc-2026-report-about-generative-ai/)
10. ["Video Gaming Report 2026: The Next Era of Growth," BCG](https://www.bcg.com/publications/2025/video-gaming-report-2026-next-era-of-growth)
11. ["10 Predictions for AI in Games for 2026," AI and Games](https://www.aiandgames.com/p/10-predictions-for-ai-in-games-for)
12. ["Developer use of generative AI may be declining," Game Developer](https://www.gamedeveloper.com/production/developer-use-of-generative-ai-may-be-declining)
