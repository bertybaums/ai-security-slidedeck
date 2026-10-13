# Your Risk-Averse Mindset Needed — NCURA Regional Meeting 2026

An HTML-based slide deck for the NCURA Regional Meeting '26 session *Your Risk-Averse Mindset Needed: Responsibly Navigating the AI Adoption Rodeo*, on AI security for research administrators.  
Hosted on GitHub Pages at: **[your-github-pages-url]**

---

## Presentation Sections

| # | Section | Slides |
|---|---------|--------|
| — | Introduction | 1 – Title, 2 – Presenters, 3 – Overview |
| 01 | AI Model Training | 4 – Section divider, 5 – True/False interactive, 6 – What is an AI Model? (graphic), 7 – Neural Networks (graphic), 8 – Inspired by Biology (graphic), 9 – Training vs. Inference (graphic), 10 – Training process flow, 11 – Models Deployed for Inference (graphic), 12 – Model inversion attack flow, 13 – Response Mining (graphic), 14 – Takeaways |
| 02 | Malicious Attacks | 15 – Section divider, 16 – Resume ranking interactive, 17 – Resume attack reveal, 18 – Prompt anatomy diagram, 19 – Prompt injection examples, 20 – Prompt Injection with Agentic AI (graphic), 21 – Takeaways |
| 03 | Risk Classification | 22 – Section divider, 23 – Shadow AI interactive, 24 – Classify data risk (interactive), 25 – Approved services per tier, 26 – NVIDIA DGX Spark spotlight, 27 – Takeaways |

| — | Conclusion | 28 – Q&A, 29 – Contact information |

**Total:** 29 slides ✓

---

## Navigation

| Input | Action |
|-------|--------|
| `→` / `↓` / `Space` | Next slide |
| `←` / `↑` | Previous slide |
| `Home` / `End` | Jump to first / last slide |
| Swipe left / right | Next / previous (touch devices) |

---


## Layout

Content is positioned inside a safe zone that clears the NCURA Regional Meeting '26 mountain banner along the bottom of the content background:

| Property | Value |
|----------|-------|
| Safe zone top | 102 px |
| Safe zone bottom | 350 px |
| Slide canvas | 1920 × 1080 px |

The center mountain peak reaches ~342 px from the bottom (y ≈ 738), so the safe zone ends at y = 730. With no logo at the top, the zone sits 50 px higher than the Annual Meeting layout while keeping the same 628 px height. Full-width graphic slides use fixed image heights that extend past the safe zone over the mountains, stopping above the NCURA banner text.

The title slide (`.title-safe`) places white text over the mountains, inside the template's title box (y = 740 to 1040).

---

## Customization

**To add or edit slide content**, open `index.html`. Each slide is a `<div class="slide ...">` block. Any element with `data-step` starts hidden and is revealed one at a time with Space/→ before the deck advances to the next slide. Use this for bullet list items (`<li data-step>`) and process-flow nodes.

**Presenters** appear on slide 2 and the contact slide (29) in a three-column grid: Nathan Wiggins (`wiggins.jpg`), Bert Baumgaertner (`Bert.webp`), and Lucas Marshall (`marshall.jpeg`), rendered as `<img class="photo-circle" style="object-fit:cover;" />` (`contact-avatar` on the contact slide). To swap in a different photo, replace the file in the repo root or the `src` on the corresponding img in `index.html`. Without a photo, a `<div class="photo-circle">AB</div>` shows initials on a blue gradient.

**Fonts:** Arial throughout. No external font dependencies.

**Images:** Both background PNGs (`Title_Slide.png`, `Slide_Template.png`) are referenced from the repository root. On the `regional` branch they are the NCURA Regional Meeting '26 backgrounds from the regional PowerPoint template (1672 × 941 source, scaled to fill the 1920 × 1080 canvas).

---

## GitHub Pages Setup

1. Go to **Settings → Pages** in this repository.
2. Set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. Save — the site will publish at `https://<username>.github.io/<repo-name>/`.

---

## License

Presentation content © 2026 [Presenter Name] / NCURA. All rights reserved.
