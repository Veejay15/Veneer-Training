# How to edit the mockups

You can change any text on these pages yourself. No software to install, no code to run.
Edits go live automatically about 30 seconds after you save.

## Where things live

| Page | File to edit | Live at |
|---|---|---|
| Comparison page | `index.html` | https://veneer-training.vercel.app/ |
| Version 1 | `v1/index.html` | https://veneer-training.vercel.app/v1/ |
| Version 2 | `v2/index.html` | https://veneer-training.vercel.app/v2/ |

## Making an edit

1. Open the file you want to change, for example `v2/index.html`
2. Click the **pencil icon** at the top right
3. Press **Ctrl+F** and type a few words of the text you want to change, to jump straight to it
4. Change the words between the `>` and `<` symbols. For example:

   `<h3>The Veneer Blueprint Course</h3>`

   To rename it, only touch the middle part:

   `<h3>The Blueprint Course</h3>`

5. Click **Commit changes**, add a short note like "shortened course heading", and confirm
6. Wait about 30 seconds, then refresh the live page

## The one rule

**Only change the words. Leave the angle brackets alone.**

Everything inside `< >` is instruction for the browser, not text that appears on the page.
If you delete a `<` or a `>` by accident, that section may disappear or look broken.

Some characters are written in code so they display correctly:

| You will see | It shows as |
|---|---|
| `&amp;` | & |
| `&rsquo;` | ' |
| `&ldquo;` `&rdquo;` | " " |
| `&middot;` | · |
| `&mdash;` | — |

Leave those as they are, or type them the same way if you need a new one.

## If something looks broken

Nothing is ever lost. Every change is saved separately and any of them can be undone.

Open the **Commits** list, find your change, and tell VJ. It takes about a minute to put back.
Or just make another edit to fix the text.

## What you cannot change this way

Layout, colors, spacing, images and the order of sections are controlled by the styling at
the top of each file. Those are easy to break by accident, so send those to VJ instead.

Text, headings, prices, button labels and links are all safe to edit yourself.

## Want to preview before it goes live?

Instead of committing straight away, choose **Create a new branch for this commit** on the
commit screen. That gives you a separate preview link to check first, and nothing changes
on the main link until it is approved.
