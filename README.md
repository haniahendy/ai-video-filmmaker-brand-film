# NOORFRAME - "Stories From Cairo" (AI Spec Brand Film)

A 20-second spec brand film for **NOORFRAME**, a fictional Cairo production-studio
brand, following one filmmaker's arc across a single day: morning rooftop shoot,
market-alley filming, the night edit, and the private screening.

**Watch:** `film2_noorframe_20s.mp4` - 1920x1080, 24 fps, 20.000 s, stereo audio.

> AI-generated content. All four scenes were generated with AI video/image tools
> and carry the tools' own watermarks. NOORFRAME is a fictional brand; no real
> product, company, or endorsement is depicted or implied.

## Scenes and sources

| # | Scene | Tool / mode | Native resolution | Notes |
|---|-------|-------------|-------------------|-------|
| B1 | Rooftop shoot, golden hour | Vidu Q4 image-to-video from a generated anchor frame | 1080p | Establishes the filmmaker (dark curly hair, beige linen shirt) |
| B2 | Market alley filming | Vidu reference-to-video (B1 anchor for identity) | 540p | Upscaled to 1080p in the grade |
| B3 | Night edit suite | PixVerse V6 reference-to-video (@image1 = B1 anchor for identity) | 540p | Upscaled to 1080p in the grade; dual-monitor edit timeline with golden-hour rooftop footage |
| B4 | Private screening room | PixVerse V6 image-to-video over a Vidu text-to-image still | 360p | Upscaled to 1080p in the grade; dark static scene, holds up well |
| Card | NOORFRAME - Stories From Cairo | ffmpeg drawtext | 1080p | Original tagline for a fictional brand |

Character consistency across B1/B2/B3 comes from anchoring every generation to
the same reference identity rather than repeated text descriptions (which drift).

## Audio

Original synthesized ambient score (numpy: Gmaj7 pad with a soft pulse and
shimmer), mixed under the clips' own AI-generated ambience where a clip carries
an audio stream, then loudness-normalized to -16 LUFS / -1.5 dBTP.

## Edit

ffmpeg only: per-scene trims (4.3 s each), unified grade
(contrast/saturation/vignette), 24 fps conform, end card, score mix.
Final container is exactly 20.000 s.

## Honest limits

- B2 and B4 were generated below 1080p and upscaled; fine detail is softer in
  those scenes. B4 is natively 360p, visible mainly in seat textures.
- AI watermarks are retained by design (disclosure), which makes the film a
  workflow/portfolio sample rather than a deliverable-grade master.
- The tools generate the pixels; the concept, shot list, prompts, anchors,
  selection/rejection of takes, grade, score, and edit are the craft on show.

## Cost

$0. Free-tier generations on Vidu and PixVerse (daily/reward credits).
