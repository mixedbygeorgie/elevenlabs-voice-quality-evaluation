# Findings

## Setup

- Date: 2026-08-24
- Product: ElevenLabs Instant Voice Cloning
- Model: Eleven Flash v2.5
- Voice settings: Stability 50, Similarity 75, Style 0
- Speaker and consent: evaluator's own voice
- Languages: English, Norwegian and Spanish
- Clean source profile: iPhone 15 Pro
- Challenged source profile: MacBook Air 13-inch, M3
- Generated files: MP3

## Acceptance logic

This evaluation separates two questions:

1. Is the audio technically usable as a synthetic voice?
2. Does it faithfully reproduce the intended speaker?

For a voice-cloning use case, identity is a hard acceptance gate. A technically clean output with an identity score of 1/5 may be usable as a generic voice, but it is not an acceptable clone.

## Findings

### 1. Technical usability did not translate into identity fidelity

All six outputs received an identity score of 1/5. The clean Spanish output achieved the highest composite score, 3.875, and contained no significant technical defect. It was technically deliverable as a generic synthetic voice, but it still did not convincingly reproduce the evaluator's voice.

**Production implication:** Neither voice clone passed the intended identity requirement. Post-production can repair hiss, tonal balance or isolated artifacts; it cannot turn a fundamentally incorrect vocal identity into a faithful clone. All six outputs therefore require a new clone or regeneration before identity-critical delivery.

### 2. The challenged capture profile produced more audible artifacts

The mean artifact score fell from 4.00 under the clean condition to 2.67 under the challenged condition, the largest measured difference between the two profiles. The English challenged output contained hiss and distortion throughout 00:00–00:06, including a pronounced defect on “voice.” The Norwegian and Spanish challenged outputs also contained audible defects near 00:00–00:02.

**Production implication:** Cleaner source capture reduced repair work in this test. Challenged outputs should be screened for hiss and distortion before editorial work; regeneration is preferable when technical defects occur together with failed identity.

### 3. Intelligibility remained relatively strong, but delivery was not fully reproducible

Mean intelligibility remained 4.33 for clean outputs and 4.00 for challenged outputs. Pronunciation remained strong overall, although the Norwegian challenged output mispronounced “energi” at 00:00–00:02. The evaluator also heard changes in speed and rhythm between the clean and challenged English and Norwegian outputs. Spanish was the most consistent pair in this small sample.

**Production implication:** Correct words and plausible phrasing are not sufficient QA criteria. Pairwise review must also consider timing, rhythm, pronunciation and whether the performance is suitable for the intended context.

## Production recommendation

Use a two-stage acceptance process:

1. **Identity gate:** Compare the generated voice directly with the consented source. If identity is not recognisable, create a new clone or regenerate before spending time on cleanup.
2. **Technical delivery gate:** Only after identity passes, assess intelligibility, pronunciation, prosody, artifacts, stability and editability. Select or regenerate defective phrases before applying conventional post-production.

For future evaluations, generate multiple takes per condition and document source format, distance, monitoring and level matching. This would help separate persistent model behaviour from take-specific variation.

## What required human audio judgment

The arithmetic averages made several outputs look broadly usable, but they did not express the central production failure: the voices did not sound like the intended speaker. Expert listening was also required to distinguish generic technical cleanliness from actual identity fidelity, to hear the pushed and mid-heavy vocal character, and to decide whether a defect justified editing or complete regeneration.

## Limitations

- One consenting speaker and six very short outputs, approximately two to six seconds each
- One model and one voice-setting configuration
- One generated output per language and source condition
- Different recording devices were used for the two source profiles, so this was not a strict single-variable comparison
- Recording distance, original source format, monitoring chain and level-matching method were not documented
- Subjective expert listening rather than objective or statistical measurement
- Norwegian evaluated natively; English and Spanish evaluated from fluent/advanced-speaker perspectives
- No external native-speaker validation for English or Spanish
- Product behaviour may change after the evaluation date

## Bottom line

The challenged source profile produced more technical artifacts, but source cleanliness was not the decisive failure. Both clones failed to reproduce the evaluator's identity. The test therefore demonstrates why clone fidelity and technical audio quality must be evaluated separately.
