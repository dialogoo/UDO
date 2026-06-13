# UDO, User Data Ownership 

> A human-centric recommendation engine that puts users in control of their own data and preferences.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status: Early Development](https://img.shields.io/badge/status-early%20development-orange)]()

---

## What it is

UDO is a recommendation system built around a simple principle: the user is the expert on themselves. Instead of black-box predictions inferred from passive behaviour, UDO lets users write their own preferences, review every input the system holds about them, and understand why any suggestion appears.

**Motto: User Data Ownership.**

---

## Core features

**Expressive input** users define their tastes in their own words: primary preferences, secondary desires, contextual notes. Structured but human.

**Reversible feedback**  likes, scores, and reactions are not permanent signals silently shaping a hidden model. They are visible, editable, and removable at any time.

**Transparent recommendations** a dedicated view lets users trace why a suggestion appears. No black box.

**You own your data**  UDO stores data locally or in a user-controlled backend. Nothing is hidden or harvested.

**Composable**  designed to integrate with marketplaces, media apps, or any user-facing system.

---

## System design

UDO is built around four components:

1. **Input engine** structured fields and open text (primary preferences, secondary desires, contextual info). Users write what they want, not just click what they see.

2. **Feedback tracker** likes, dislikes, scores, emotional tags. All accessible, editable, and reviewable. Nothing is final.

3. **Recommendation core** uses LLM + rules-based filtering to propose items from a public or private catalogue. Logic is inspectable.

4. **User dashboard** view, revise, or remove any input. See how recommendations respond. The user's model of themselves is always visible.

---

## The road ahead

UDO is designed to grow in two stages, each meaningful on its own:

**Stage 1. Transparency (current focus)**
The preference UI and dashboard. Users see and control everything the system holds about them. The vector may still live on the server at this stage — but it is legible, editable, and belongs conceptually to the user. This is already a meaningful gap from every mainstream recommendation system today.

**Stage 2. Sovereignty**
The vector moves to the client device, encrypted at rest under a key the user controls. The server holds the model and catalogue; it never stores a user profile. Inference loads the vector transiently, scores items, and discards it. A future AI system cannot retroactively reprocess data that was never stored.

The motivation: a preference vector is a detailed map of a person's psychology. As AI systems grow more capable, that map becomes more dangerous in the wrong hands. Stage 1 makes it visible. Stage 2 makes it yours.

Full design specs are in [`docs/`](docs/).

---

## Status

Early development. The project is at the design and scaffolding stage.

We welcome discussions, ideas, and issue reports. If you'd like to collaborate, please [open an issue](https://github.com/dialogoo/UDO/issues).

---

## License

MIT
