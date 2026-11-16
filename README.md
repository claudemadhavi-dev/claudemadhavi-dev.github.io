# Madhavi Adusumilli: personal website

Live at **https://claudemadhavi-dev.github.io**

The whole site is one file, `index.html`. There's no build step: edit it, commit, and GitHub Pages republishes within a minute or two.

## How to edit

**On github.com (easiest):** open `index.html`, click the pencil icon, make your change, then click **Commit changes**.

**With Claude:** ask Claude to change the site and push it to this repo.

## Where things are in index.html

Search the file for these markers:

| Section | Search for |
|---|---|
| Headline and intro | `class="hero"` |
| Highlight numbers | `class="readout"` |
| About | `id="about"` |
| Experience | `id="experience"`. Each job is an `<article class="job">` block |
| Agents | `id="building"`. Copy a `<div class="card">` block for each new agent |
| Interests | `id="interests"`. Replace each `Add an interest` chip |
| Contact links | `id="contact"` |
| Colors and fonts | the `:root` block at the top of `<style>` |

### Adding an agent

Replace the "First agent" card (or add another after it) with:

```html
<div class="card">
  <span class="status">Shipped</span>
  <h3>Agent name</h3>
  <p>One or two lines on what it does and what you learned.</p>
  <a href="https://github.com/claudemadhavi-dev/REPO-NAME">View on GitHub →</a>
</div>
```

To drop the dashed "coming soon" style, use `class="card"` instead of `class="card soon"`.
