# Lessons

Read before every piece of work. Add to it after every piece of work and every feedback round. Date each entry, keep it to one to three lines, and put it under the right heading. When a lesson holds everywhere, move it into `brand.md` and delete it here.

---

## What Kurtis liked and removed

- **2026-11 · Simplest personal option wins.** He picked the Dalen-style personal letter over the recommended hybrid. Lead with his own story.
- **2026-11 · No avatar or logo above the headline.** Both were tried; he removed them. Start with the headline.
- **2026-11 · Pills show the handle, not the platform name.** Icon + "@kurtiswin".
- **2026-11 · Brand-coloured outline icons, not platform colours.** Red YouTube and gradient Instagram were replaced with gold outlines; gold beat white.
- **2026-11 · Fewer words (signup ended as just email + button).** He cut the video caption, the visible card heading, topic descriptions and the "no spam" line, and cut eight topics to three. Default to labels only, and few of them.
- **2026-11 · Real logos, done the brand's way.** Letter tiles and an invented "JB" monogram were rejected; the Java Bonito icon must match its own favicon (whole wordmark across a black square).
- **2026-11 · Black everything.** Grey cards and pill fills read as cheap; black with a hairline and a gold hover ring reads premium.
- **2026-11 · Space = luxury.** He asked for the hero lower and slightly more space between blocks. Err towards more air.
- **2026-11 · One column, shared edges.** Video went 1.2× text width → half width → finally exactly the column width, with the email form the same width and the card frame dropped. Everything lines up to the headline's edges.
- **2026-11 · Gold for one word only.** "nine" went gold, then back to white; only "beautiful" in the headline stays gold.
- **2026-11 · He'll rename things himself.** He renamed the board "KurtisWin - Design Board" outside the session. Keep his names.

- **2026-11 · The board is a world, not just a brand.** It became "KurtisWin - World Building Design Board": a My world card of square logo tiles (KurtisWin photo, Java Bonito, Woolton FC, Stories from Football, Kate's Cafe) that filter the board, each world's work tagged `data-world`. New work for any project goes on this board under its world.

- **2026-11 · New styles go in "Other ideas", never over the live site.** When Kurtis likes another creator's site, build a separate idea page in his palette and add it under KurtisWin · Other ideas on the World Building board. First one: Simple letter, after zackkravits.com.

## Technical traps

- **Inline icon chips look raised** when the link is `inline-flex`/`inline-grid`, and commas drift. Keep the link inline and make the icon an inline `img` at 1.4em with `vertical-align: -.36em` (Poppins), then measure.
- **Phone width limits line count.** At 390px the story already uses the full width; "one fewer line" only applies on laptop unless the font gets smaller. Say so.
- **Phone screenshots are 3× pixels.** Scale coordinates before cropping assets out of his screenshots.
- **Reference sites blocked.** danieldalen.com, sandcastle.studio and javabonito.co.uk could not be fetched from the cloud session. Ask for screenshots or screen recordings.
- **Mixed DJI clips (H.264 + HEVC)** join cleanly with ffmpeg's concat filter after scaling each to the same size, SAR and frame rate.
- **Artifact republish conflicts.** If the board was published elsewhere, merge that version (e.g. his title change) before republishing.
- **Topic rows wrap on small phones.** Three topics fit on one line from 375px with 12.5px labels and .08em spacing; check 320px and accept a centred second line.
- **White flash when pulling past the ends on a phone.** Set `html{background:#000}` (not just `body`) and `<meta name="theme-color" content="#000000">` so the overscroll area and phone browser bar stay black. Inside the claude.ai artifact viewer the outer frame may still show its own colour.
- **`hidden` loses to `display:grid`.** Add `[hidden]{display:none!important}` so filtered sections really hide.
