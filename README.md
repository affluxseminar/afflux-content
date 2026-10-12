# afflux-content

The seminar programme, nothing else: `data/talks/` (one JSON file per seminar), `photos/` (speaker
portraits) and `files/` (slides and minutes as PDF, PPT or PPTX). Public, because the programme is
public. The site's admin writes here through a token limited to this repository; the secretary
normally never opens it. GitHub's web editor works as a fallback.

A seminar entry may carry `slides` and `minutes`: either an `https://` address or the name of a
file placed in `files/` (letters, digits, dots, hyphens; at most 40 MB). Past sessions appear in
the archive by themselves, with links to the recording, the slides and the minutes when present.

Nobody who edits this repository needs, or has, any access to the site's code, the server, the
databases or any credential: this repository holds **no secrets and no workflows**. The site's
own deploy workflow (in the code repository) checks this repository out read-only every 15
minutes and rebuilds when its latest commit changed; the owner can also trigger a rebuild by hand.
