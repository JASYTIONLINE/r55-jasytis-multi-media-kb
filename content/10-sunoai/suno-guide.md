---
title: "How to Write Suno-4.5-Compliant Lyrics & SSIGs"
description: "The master guide for writing Suno 4.5-compliant lyrics and SSIGs. Explains formatting, prompting, and proven techniques for reliable generation."
tags: [suno, lyrics, ssig, guide, quartz]
draft: false
date: 2025-09-29
---

# Suno Guide – Writing Lyrics & SSIGs  

## Introduction  
This page is the **master guide** for creating Suno v4.5-compliant lyrics and style signatures (SSIGs).  
It explains the formatting, prompting, and proven best practices that make Suno generate music the way you intend.  

When you finish this page, you’ll be able to:  
- Format lyrics correctly for Suno 4.5.  
- Use tags, meta-tags, and parentheticals without breaking vocal delivery.  
- Apply expressive formatting to shape phrasing and emotion.  
- Write SSIGs that reliably instruct Suno on genre, arrangement, vocal tone, and mood.  

For worked examples, see:  
- [[example-lyric-sheet-I'll-always-remeber|Example Lyric Sheet – I'll Always Remember]]  
- [[suno-glossary|Suno Glossary – Reference Terms]]  

---

## Writing Suno Lyrics  

### Section Tags  
Use standard markers to structure the song. Suno expects these and will perform more predictably:  
`[Intro]`, `[Verse]`, `[Pre-Chorus]`, `[Chorus]`, `[Refrain]`, `[Bridge]`, `[Interlude]`, `[Breakdown]`, `[Tag]`, `[Coda]`, `[Outro]`, `[End]`.  

### Meta-Tags  
Control instruments, vocal tone, or mood for each section with key:value tags:  
```
[Instrument: Piano]  
[Mood: Reflective]  
[Vocal: Whisper]  
```  
Always place meta-tags **above the section** they affect.  

---

## Expressive Formatting  

Use formatting sparingly to guide delivery:  
- `UPPERCASE` → emphasis or shouting  
- `…` → pause or breath  
- `loooove` → sustain a note  
- `no-no-no` → staccato rhythm  

Too much formatting can confuse phrasing, so apply it only where it matters.  

---

## Parentheticals  

Parentheses allow short vocal cues:  
- `(whisper: don’t leave)`  
- `(echo: ever… ever…)`  
- `(ad-lib: yeah!)`  

Keep them brief. Suno interprets longer parentheticals as lyrics to sing.  

---

## Length & Limits  

- Stay under ~7,500 characters in the Lyrics box.  
- Avoid bloated copy-pasted choruses; repeat them intentionally.  
- Test lyrics in chunks if you’re unsure.  

---

## Example: Suno-Ready Lyric Block  

```text
[Intro]  
[Instrument: Piano, Mood: Reflective]  

[Verse 1]  
I walk alone into the night…  
My heart beats slow, searching for light  

[Pre-Chorus]  
(whisper: hold on)  
Every step brings me closer to you  

[Chorus]  
I’ll always REMEMBER, forever remember!!!  
Your arms around me, loooove pulling through  
```

---

## Writing Suno SSIGs  

The **Style Signature (SSIG)** tells Suno how to perform the song.  
It is separate from lyrics and controls **genre, instrumentation, vocal style, arrangement flow, and emotional tone**.  

### Rules for SSIGs  
- Write in plain descriptive phrases.  
- Do not include lyrics.  
- Cover genre, vocal style, instrumentation, rhythm, arrangement flow, and mood progression.  
- Compact, but detailed enough to lock Suno into the intended performance.  

### Example SSIG  
```text
Melancholy waltz • Sultry female vocal, smoky tone • Passionate verse delivery inspired by Patsy Cline’s “Crazy” and Dolly Parton’s “Jolene” • Key change at bridge from C Major to A Minor • Emotional contour through instrumentation: piano + strings in intro, upright bass + brushed snare in verses, swelling strings in pre-chorus, full drums in chorus • Drop to minimal piano and bass during bridge, then rebuild to full arrangement in final chorus • Mood progression: tender → yearning → desperate → cathartic release
```

---

## Next Steps  

- Use [[example-lyric-sheet-I'll-always-remeber|I’ll Always Remember Lyric Sheet]] to see a polished, fully formatted lyric + SSIG entry.  
- Reference [[suno-glossary|Suno Glossary]] for definitions of every key term.  
- Once your lyrics and SSIG are complete, you can move into production using [[guide-music-video-creation|Music Video Creation Guide]].  

---
