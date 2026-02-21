# cat-emotional-resonance-ranker

Ranks cat pictures by emotional resonance — the degree to which each image stirs genuine feeling in the viewer.

## Purpose

Not all cat pictures are created equal. Most are seen and forgotten. A rare few make you stop, hold your breath, and feel something you did not plan to feel. This function finds those pictures. It separates images that are merely viewed from images that are genuinely felt, ranking them by the depth and honesty of the emotional experience they create.

Technical photographic quality is deliberately secondary. A blurry snapshot alive with feeling will rank above a studio portrait that is emotionally flat. What matters is charm — that hard-to-name quality that makes a person stop scrolling, smile, or feel a pang of affection for a small animal they have never met.

## Input

The function accepts an array of cat images (minimum 2). Images may vary in quality, format, composition, and context — from professional photographs with careful lighting to hasty snapshots taken because a cat did something extraordinary and brief. The function receives them all equally and evaluates each for emotional resonance.

```json
{
  "type": "array",
  "minItems": 2,
  "items": {
    "type": "image",
    "description": "A cat picture to evaluate for emotional resonance."
  }
}
```

## Output

A score vector of the same length as the input array. Each score reflects the relative emotional resonance of the corresponding image. Higher scores indicate images that create stronger felt connection with the viewer. The scores can be used to rank, sort, or filter the input collection from most to least emotionally resonant.

## What It Evaluates

The function measures emotional resonance across three distinct qualities. Each captures a different facet of what makes a cat picture move from ordinary to unforgettable.

### 1. Vulnerability

The degree to which the image captures a cat in a moment of unguarded openness. Cats are composed creatures by nature, so when a photograph catches one with its defenses down — mid-yawn with its entire ridiculous mouth on display, asleep in a position that defies anatomy and dignity, or blinking slowly with an expression that can only be described as trust — something shifts in the viewer.

**Scores higher:** Private, unposed moments. A cat asleep in an absurd position. Eyes half-closed in trust. Body gone completely soft, suggesting total safety. Moments the cat did not perform for anyone.

**Scores lower:** Stiff or alert poses. Cats visibly aware of the camera. Images that are visually striking but emotionally guarded — admirable but hard to feel.

### 2. Narrative Atmosphere

The degree to which the image suggests an emotional world beyond the edges of the frame. Some cat pictures are records of a cat in a place. Others are windows into a story you can almost hear — created by the interplay of cat, light, setting, and mood.

**Scores higher:** Images that generate involuntary narrative. A kitten asleep inside a shoe (a story about smallness). A cat silhouetted on a crumbling wall at dusk (a story about solitude). A cat at a rain-streaked window (an invitation to wonder). Images with emotional weather the viewer steps into without deciding to.

**Scores lower:** Cats isolated against plain or featureless backgrounds. Images that are visually competent but closed — complete in a way that asks nothing of the imagination.

### 3. Spontaneous Delight

The degree to which the image produces an immediate, involuntary emotional response before the viewer has time to analyze it. This is the stop-scrolling quality — pre-cognitive, arriving before judgment or taste.

**Scores higher:** Humor (a cat's face caught at an angle that mimics a human emotion). Absurdity (physics-defying positions, the places cats choose to sit). Unforced beauty that bypasses aesthetics and lands as pure feeling. Surprise — images that feel like encounters rather than compositions.

**Scores lower:** Images that are pleasant or technically accomplished but predictable. Pictures that can be appreciated but do not ambush the heart.

## Use Cases

- **Content curation:** Surface the images that will genuinely move an audience from large submission pools, rather than selecting only the technically sharpest.
- **Animal shelter adoption listings:** Identify which photographs best convey a cat's personality and spark the immediate, wordless impulse to care — connecting adoptable cats with families.
- **Community platforms:** Elevate posts that deliver genuine daily joy, ensuring the images that make someone's morning lighter rise to the top.
- **Social media management:** Rank candidate posts by emotional impact to maximize authentic engagement driven by feeling rather than visual polish.
- **Personal photo organization:** Sort through camera rolls to find the keepers — the images worth sharing, printing, or returning to.

## Philosophy

These three qualities are not a checklist. An image need not score highly in all three to rank well. A picture that is extraordinarily vulnerable but low in narrative atmosphere can still devastate. An image rich in atmosphere but modest in vulnerability can still haunt. And an image that delivers pure spontaneous delight with little of the other two can still be the best thing a person sees all week.

The function's deeper conviction is that emotional resonance is not an accident and not a formula — it is a relationship between subject and viewer, between moment and meaning, between what is seen and what is felt. What we are ranking is not the quality of photographs. We are ranking the quality of feeling they create.