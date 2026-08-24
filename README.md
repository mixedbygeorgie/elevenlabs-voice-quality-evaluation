# ElevenLabs Voice Quality Evaluation

## Purpose

This practitioner-led listening evaluation examines whether an ElevenLabs Instant Voice Cloning workflow preserves speaker identity while producing intelligible, editable and technically deliverable audio.

The project is a small practical comparison, not a statistical model benchmark. It documents the capture conditions, scoring rubric, results, limitations and production implications.

## Evaluator

Christer George is a senior recording, mixing and mastering engineer with 20+ years of hands-on voice and vocal production experience. His work includes more than 1,000 released and unreleased songs, demos and vocal productions and more than 500 commercially released mixes.

## Evaluation questions

1. Did either clone convincingly preserve the evaluator's voice identity?
2. How did two practical source-capture conditions affect artifacts and production usability?
3. Were the outputs intelligible and usable across English, Norwegian and Spanish?
4. Which problems were repairable, and which required a new clone or regeneration?

## Method summary

- Product: ElevenLabs Instant Voice Cloning
- Model: Eleven Flash v2.5
- Voice settings: Stability 50, Similarity 75, Style 0
- Speaker: evaluator's own voice
- Source-capture profiles: iPhone 15 Pro (`clean`) and MacBook Air 13-inch, M3 (`challenged`)
- Outputs: six short MP3 files across English, Norwegian and Spanish
- Review: expert listening against a 1–5 production rubric with timestamped observations

Text, model and voice settings were held constant within each language pair. Because the two conditions used different capture devices and the original recording distance, source format, monitoring chain and level-matching method were not documented, this should be read as a paired practical comparison rather than a strict single-variable experiment.

## Headline result

The clean-condition composite score was 3.71 versus 3.33 for the challenged condition. Artifact score showed the largest difference, falling from 4.00 to 2.67.

That average does not determine success for a cloning use case. All six outputs scored 1/5 for identity. One Spanish output was technically deliverable as a generic synthetic voice, but neither clone was acceptable as a faithful reproduction of the evaluator's voice.

## Repository contents

* `TEST_PLAN.md` — executed method and deviations from a strict controlled design
* `EVALUATION_RUBRIC.md` — listening criteria, score definitions and the identity acceptance gate
* `SCORES.md` — complete score transcription and condition averages
* `FINDINGS.md` — timestamped evidence, interpretation, limitations and production recommendations
* `audio/` — six evaluated generated outputs and two original source-reference recordings

## Status

**Evaluation completed on 2026-08-24.** The documentation, all six evaluated generated outputs and both original source-reference recordings are included. The findings are limited to this speaker, model, voice-setting configuration and the two documented source-capture profiles.



## Ethics and consent

No third-party voice should be uploaded without explicit permission. Samples should not contain confidential client audio, copyrighted scripts that cannot be redistributed or personal information. Generated outputs must be labelled clearly and must not be used to impersonate or mislead.

## Portfolio context

- [LinkedIn](https://www.linkedin.com/in/christer-george-a5195353)
- [Selected commercial audio portfolio](https://open.spotify.com/playlist/71M808TSSbE6GFslvIPUCP?si=cb7886ec4a6f4873)
