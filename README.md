# X-Camp Partner Resources

Winner letters. A partner sends one of these pages to the winners of its contest. The page
congratulates the winner. It also shows the X-Camp courses and the award credit.

Your site is live at
**https://x-camp-academy-ca.github.io/xcamp-partner-resources/**

## Pages

| Contest | UTM source | URL |
|---|---|---|
| GPL 2026 | `gpl` | [open](https://x-camp-academy-ca.github.io/xcamp-partner-resources/xcamp-winner-letter-2026-gpl.html) |
| HPI 2026 | `hpi` | [open](https://x-camp-academy-ca.github.io/xcamp-partner-resources/xcamp-winner-letter-2026-hpi.html) |
| LIT 2026 | none — see below | [open](https://x-camp-academy-ca.github.io/xcamp-partner-resources/xcamp-winner-letter-2026-lit.html) |
| TACO 2026 | `taco` | [open](https://x-camp-academy-ca.github.io/xcamp-partner-resources/xcamp-winner-letter-2026-taco.html) |
| TeamsCode 2026 | `teamscode` | [open](https://x-camp-academy-ca.github.io/xcamp-partner-resources/xcamp-winner-letter-2026-teamscode.html) |
| Template | — | [open](https://x-camp-academy-ca.github.io/xcamp-partner-resources/xcamp-winner-letter-template.html) |

The text is the same on each page. Only the UTM source is different. The UTM source tells
you which partner sent the click.

## How to make a new letter

1. Copy an existing letter. Give the copy the new name.
2. Change the UTM source on all 18 links to the new partner.
3. Check the count. Each page must have 18 links with the same UTM source.
4. Ask Shanshan for the UTM source if the partner is new. Shanshan owns the UTM list.

Use this pattern for the file name:

```
xcamp-winner-letter-{year}-{partner}.html
```

- Write all characters in lower case. Use a hyphen between words.
- `{partner}` must be the same as the UTM source for that partner.
- Name the page after the **contest**, not after the partner. One partner can hold two
  contests. Example: Harker Programming Club holds both HPI and GPL.

## Open problems

**1. The LIT letter has no UTM source.** Its 18 links do not track. This letter went to the
LIT winners in June 2026, so X-Camp has no click data from it. Add `utm_source=lit` before
you send this page again.

**2. The UTM source `gpl` is new.** Shanshan's table of September 28 has `hpi`. It does not
have `gpl`. Ask Shanshan to add `gpl` to the table.

**3. The template page is empty.** The file holds 2 bytes. Fill the page or delete the file.

**4. One old link is dead.** `XCamp_Winner_Letter.html` went to 114 winners on 24 June 2026.
That file is no longer in this repository. The link returns a 404 error.

## Google Analytics

Each page has the Google Analytics tag `G-L64HE50P6M` in the `<head>` block. The template
page does not have the tag. Copy this block into each new page:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-L64HE50P6M"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-L64HE50P6M');
</script>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
```

Google keeps this data for 30 days only. Download a report before the data expires.
