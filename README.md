# DubFocus: adaptive soundscapes for deep focus and calm

Live demo: https://dubfocus.netlify.app/

DubFocus is a **browser-based soundscape workstation** built for one thing: helping you craft an audio environment that makes it easier to stay in a focused state for long work sessions, or to settle into meditation / relaxation.
Instead of relying on music, DubFocus lets you *shape* your environment in real time, mixing steady **noise textures**, **binaural beats**, and **ambience** through using your **live microphone**.

## Why this exists (the brain is weird about voices)

Human speech is a special kind of distraction.
Even when you *try* to ignore background conversation, the auditory system tends to “grab” salient changes like onsets, loudness jumps, and brief pauses that momentarily unmask competing speech - exactly the kinds of features that pull attention away from your task.
DubFocus takes a different approach than pure noise-canceling or “just play music.”
From both the literature and hands-on tinkering while building this project, a practical trick is to **reduce the “speech-likeness”** of voices by *transforming* them: e.g., reverb/delay/filtering, resonant harmonics, or granular textures, so the voice starts behaving more like an instrument or a distant texture.
That makes it easier for your brain to stop “parsing meaning”, while still giving you a stable, non-informational layer that can mask interruptions.

## The building blocks

### 1) Noise as a stabilizer for attention

Random auditory noise, most often white or pink noise in the literature, can sometimes improve performance on laboratory attention tasks in groups with elevated attentional difficulties.
A 2024 systematic review and meta analysis reports a small benefit of white and pink noise for individuals with ADHD or high ADHD symptoms, with weaker or negative effects in non ADHD comparison groups.
Source: [Nigg et al., 2024, Journal of the American Academy of Child and Adolescent Psychiatry](https://pubmed.ncbi.nlm.nih.gov/38428577/) and the open full text in [PubMed Central](https://pmc.ncbi.nlm.nih.gov/articles/PMC11283987/).

How DubFocus uses this idea: it gives you a noise generator for masking and stability, with controls so you can make the texture comfortable for long sessions.
If you are aiming for deep focus, the goal is to create a steady, low annoyance bed that masks interruptions and reduces how much meaningful signal gets through.

### 2) Binaural beats as a gentle entrainment tool

Binaural beats are an auditory illusion created by presenting slightly different tone frequencies to each ear.
Some studies report effects on sustained attention or working memory under specific parameters, and other studies find smaller or inconsistent effects.
A recent parametric study in Scientific Reports explored how binaural beat settings and masking can improve sustained attention outcomes and entrainment measures.
Source: [Melnichuk et al., 2025, Scientific Reports](https://www.nature.com/articles/s41598-025-88517-z) and the indexed record in [PubMed](https://pubmed.ncbi.nlm.nih.gov/39910150/).

The grounded takeaway is that binaural beats are a plausible, low risk tool that may help some people and not others.
And **parameters matter**, **comfort matters**, and the only meaningful evaluation is whether they help you sustain attention in **your own** routine.

How DubFocus uses this idea: it includes a binaural beat generator designed for headphone use, so you can test settings while working and keep what actually feels beneficial.

### 3) Real time audio as a feedback loop

You can create a loop between what is happening around you and what you hear after processing.
If typing, room tone, or distant chatter becomes part of a coherent texture, the environment can feel less like random interruptions and more like a continuous soundscape.
In plain language, you are converting unpredictable events into predictable low annoyance textures.

There is also direct research motivation for focusing on speech as the main culprit.
Irrelevant speech can impair performance and can increase stress responses in cognitive tasks.
Source: [Radun et al., 2024, Applied Acoustics](https://www.sciencedirect.com/science/article/pii/S0167876024000564) and the [PubMed record](https://pubmed.ncbi.nlm.nih.gov/38641017/).

## What’s in the demo

- **🎙️ Mic FX (“Dub your reality”)**: take live room sound and sculpt it into a drone/texture.
- **🧠 Binaural beats + noise**: binaural beat generator (headphones) and a noise source for masking.
- **🌧️ Ambience layers**: sample-based ambience (e.g., rain) to build a stable background.
- **🎛️ Modular FX rack**: drag-and-drop effects chain per source (reverb, delay, filters, resonators, granular drone, shimmer, etc.).
- **🛡️ Audio safety**: master limiter and parameter smoothing to reduce clipping/clicks.

## Privacy and safety (important, because microphones are spooky)

- **No recording, no upload**: the demo does not store or send microphone audio to any server.
- **Recommended setup**: use **headphones** and enable your mic if you want environment modulation.
- **Use sane volume**: keep levels comfortable, take ear breaks, and don’t try to “blast away” distraction.

## References

Melnichuk A, Cooper RK, Hawk LW. A parametric investigation of binaural beats for brain entrainment and enhancing sustained attention. Scientific Reports. 2025.
https://www.nature.com/articles/s41598-025-88517-z

Nigg JT, et al. Systematic Review and Meta Analysis: Do White Noise or Pink Noise Improve Cognitive Performance in ADHD or Elevated Attentional Problems. 2024.
PubMed: https://pubmed.ncbi.nlm.nih.gov/38428577/
Open full text: https://pmc.ncbi.nlm.nih.gov/articles/PMC11283987/

Radun J, et al. The effects of irrelevant speech on physiological stress, cognitive performance and subjective experience, with focus on heart rate variability. Applied Acoustics. 2024.
ScienceDirect: https://www.sciencedirect.com/science/article/pii/S0167876024000564
PubMed: https://pubmed.ncbi.nlm.nih.gov/38641017/

Shavit Cohen K, et al. The Dynamics of Attention Shifts Among Concurrent Speech in a Naturalistic Multi speaker Virtual Environment. Frontiers in Human Neuroscience. 2019.
Journal page: https://www.frontiersin.org/journals/human-neuroscience/articles/10.3389/fnhum.2019.00386/full
Open full text: https://pmc.ncbi.nlm.nih.gov/articles/PMC6857110/

Open preprints often appear first on arXiv and bioRxiv.
https://arxiv.org/
https://www.biorxiv.org/
