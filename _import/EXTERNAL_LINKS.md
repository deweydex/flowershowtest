# External links, one by one

184 distinct external addresses remain on the site (355 link occurrences,
because the 2025-2026 course pages exist twice: under Current Teaching and
under Prior Teaching). The import sandbox cannot open any of them, so each
has a verdict from what the address and its context tell us, and a note on
what to do. `check_links.sh` in this folder confirms the HTTP side in a
minute or two from any laptop:

```bash
bash _import/check_links.sh > link_status.tsv
grep -v $'^200\t' link_status.tsv      # anything not 200 needs a look
```

Two hosts answer 200 even when the thing is gone, so they need eyes rather
than the script: YouTube (a removed video still returns a page) and Google
Colab or Drive (a private or deleted file returns a sign-in page). Open
those in a private browser window.

Verdicts:

- **FIXED** changed in this pass.
- **KEEP** a stable, public address; let the script confirm it.
- **UPDATE** works today only through a redirect, or has a better target.
- **CHECK** an address that goes stale often; script or a look needed.
- **ASK** a decision for Josh (see `QUESTIONS_FOR_JOSH.md`).
- **REMOVE** tied to a past class, an account, or a service that has closed.

## Fixed in this pass (no network needed)

| Was | Now | Where |
|---|---|---|
| `[planning.md](http://planning.md)` and readme.md, testing.md, maintenance.md (30 occurrences) | plain `planning.md` in code style | Web Authoring briefs and templates |
| `[yourusername.github.io](http://yourusername.github.io)` and the github.com form (3) | plain code text | Assignment templates |
| `http://Coolors.co` (6), `http://Unsplash.com` (2) | `https://coolors.co`, `https://unsplash.com` | Assignment templates |
| `http://draw.io` (4) | `https://www.drawio.com` (draw.io now redirects there) | Web Authoring project brief |
| `http://stackedit.io/` | `https://stackedit.io/` | Web Authoring 2024-2025 |
| `3blue1brown.com/?topic=neural-networks` | `3blue1brown.com/topics/neural-networks` | Mathematics |
| machinelearningmastery backpropagation link ending in `#` | same address without the `#` | Mathematics |
| Wikipedia links labelled HTML and CSS pointed at each other's article | labels and targets now match | Web Authoring and Databases |

## Josh's own sites and accounts

| Address | Verdict | Note |
|---|---|---|
| https://deweydex.github.io/WADB_Tutorials/ (and `#templates`) | KEEP | Repository exists; GitHub Pages for it should be live. |
| https://deweydex.github.io/AIML_WA/ | KEEP | Repository exists. |
| https://github.com/deweydex (7 links, two spellings) | KEEP | Public profile. |
| https://jsaaron.carrd.co/# | ASK | Under "Socio-Emotional Learning in STEM Contexts: Link to Workshops" on Assorted Teaching Materials. Looks like the old consultancy page. Remove the heading or point it somewhere current. |
| https://jsaaron.com | ASK | Cross-Module Integration Summary says "All resources are linked from jsaaron.com". If that is to be this site, fine; if the domain is not set up, remove the sentence. |

## Google Colab (25) and Google Drive (7)

All are `?usp=sharing` links to files in Josh's Drive. They work only while
the file exists and is shared with "anyone with the link". The script
cannot tell a private file from a public one. Recommendation: open each in
a private window; for the ones on Current Teaching pages, consider copying
the notebook into a GitHub repository (Colab can open notebooks straight
from GitHub, and the link then never expires).

| Address | Verdict | Where |
|---|---|---|
| https://colab.research.google.com/ (4) | KEEP | The service itself. |
| colab .../github/jonkrohn/ML-foundations/... | KEEP | Public GitHub-backed notebook. |
| 23 colab `/drive/...?usp=sharing` notebooks | CHECK | Mathematics, Research and Study Skills, Web Authoring, Maths for IT, FOOP, Programming Design Principles, Technical AI Workshops. |
| 7 drive.google.com folders and files | CHECK | Two are curriculum folders from US teaching (Fun With Functions; Measuring the World) on Assorted Teaching Materials, one is an "Evaluation of the Impact of Comics" file, the rest are Mathematics notebooks. |

## YouTube (15)

| Address | Verdict | Note |
|---|---|---|
| watch?v=aircAruvnKk (3Blue1Brown neural networks, 8 pages) | KEEP | Well-known series. |
| watch?v=bxe2T-V8XRs (playlist, 8 pages) | CHECK | Second "Playlist on Neural Networks"; confirm which channel. |
| playlist PLdo4fOcmZ0oULFjxrOagaERVAMbmG20Xe | KEEP | Microsoft's C# 101 playlist. |
| playlist PLiaHhY2iBX9g6KIvZ_703G3KJXapKkNaF | CHECK | |
| watch?v=8idr1WZ1A7Q, G43vl3RKN5s, HZGCoVF3YvM, LPZh9BOjkQs, SmZmBKc7Lrs, WUvTyaaNkzM, lgUIx75fJ_E, xQlD5uYwYEs | CHECK | Open each; a removed video still returns 200. |
| youtu.be/6YzrVUVO9M0, GkiITbgu0V0, XTcP4oo4JI4 | CHECK | Same. |

## Tied to a past class or an institutional account

| Address | Verdict | Note |
|---|---|---|
| khanacademy.org/join/BDBED472 (Maths for IT 2024-2025) | REMOVE | Class join code for a finished class. |
| khanacademy.org/join/MAR9BPAP (Programming Design Principles) | REMOVE | Same. |
| forms.office.com/e/huXkP8EbkC (Maths for IT) | REMOVE | "Independent learning plan" form for a past class; almost certainly closed. |
| linkedin.com/learning-login/share?account=237718738... (Foundations of AI for Business) | REMOVE or note | Needs the college's LinkedIn Learning licence. |
| teams.microsoft.com channel and team links (Web Authoring, AIML) | ASK | Enrolled students only. Keep with "students only" or remove. |
| khanacademy.org/python-program/... (3, Programming Design Principles) | CHECK | Shared Khan Academy Python programs; should be public. |

## Services that have changed

| Address | Verdict | Note |
|---|---|---|
| https://glitch.com/ (Web Authoring 2024-2025) | REMOVE or UPDATE | Glitch stopped hosting apps in July 2025. Replace with GitHub Pages (already listed) or CodePen. |
| https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview | UPDATE | Anthropic's docs moved to platform.claude.com; the old address redirects. |
| https://ai.google.dev/gemini-api/docs/prompting-intro | UPDATE | Google reorganised these pages; if it 404s, use https://ai.google.dev/gemini-api/docs/prompting-strategies. |
| developer.mozilla.org/en-US/docs/Learn/... (3) | UPDATE | MDN moved "Learn" to "Learn_web_development" in 2025; the old paths redirect. |
| https://greenteapress.com/wp/think-python-2e/ (4 pages) | UPDATE | Third edition exists: https://greenteapress.com/wp/think-python-3rd-edition/ |
| https://v2.scrimba.com/learn-typescript-c03c | CHECK | Scrimba changed its course addresses. |
| https://dotnet.microsoft.com/en-us/platform/try-dotnet | CHECK | Microsoft has retired and moved this page before. |
| https://learn.microsoft.com/en-us/collections/yz26f8y64n7k07 | CHECK | User collections are sometimes deleted. |
| https://artofproblemsolving.com/store/list/all-products | CHECK | If it 404s, use https://artofproblemsolving.com/store |

## University and course PDFs (move often)

| Address | Verdict | Note |
|---|---|---|
| tudublin.ie .../MCT-exam-Easter2019... and .../MCT-... 2017 | CHECK | TU Dublin past maths competency papers; the site reorganises. The test page https://www.tudublin.ie/study/undergraduate/cao/entry-requirements/maths-competency-test/ is the safer link. |
| monroeu.edu .../placementexamreview.pdf | CHECK | |
| iscontent.byu.edu/Canvas/MATH-110/... | CHECK | A Canvas-hosted page; likely to have moved. |
| www3.cs.stonybrook.edu/~pfodor/courses/CSE316/L03-HTML_CSS.pdf | CHECK | Personal course page. |
| library.unsw.edu.au/.../primary-and-secondary... | CHECK | Library sites reorganise. |
| maths.ox.ac.uk .../maths-admissions-test | KEEP | |
| mathsaustralia.com.au/placement-tests/placement-tests/ | CHECK | |

## Reference and learning sites (expected to be fine)

freecodecamp.org (10), developer.mozilla.org root, curriculum and blog,
docs.github.com (4), pages.github.com, codecademy.com (6), khanacademy.org
root, 3blue1brown.com/topics/linear-algebra, ourworldindata.org,
code.visualstudio.com (2), en.wikipedia.org (2), markdownguide.org (2),
markdowntutorial.com, markdownonline.org, flexboxfroggy.com,
cssgridgarden.com, anchoreum.com, theodinproject.com, w3schools.com/sql,
sql-easy.com, sqltoerdiagram.com, docs.python.org, realpython.com,
kaggle.com, playground.tensorflow.org, machinelearningmastery.com,
jetbrains.com/pycharm, edupyter.net, pythonz2h.com, inventwithpython.com,
py4e.com, csharpplayersguide.com, scottlilly.com, tutorialsteacher.com,
programiz.com, onecompiler.com, codechef.com, edabit.com,
platform.openai.com, api-docs.deepseek.com, deepmind.google,
research.google, blog.google, learningfromexamples.com,
garyliang.substack.com, nolanlawson.com, gohugo.io, carrd.co,
creativecommons.org (3), eff.org (2), mozilla.org (2), signal.org (2),
wikimedia.org (2), w3.org, cor.inquirygroup.org, inquirygroup.org,
webwise.ie, thecrashcourse.com, timothyprojectgig.github.io,
atmamani.github.io, audiolabs-erlangen.de, barschazki.com, paper.co.

Verdict KEEP for all of these; the script will show any that have moved.
Three are worth a look even if they answer 200: pythonz2h.com and
markdownonline.org are small sites that may have changed hands, and
barschazki.com is a person's portfolio.

## Placeholder addresses

None remain as links. The example addresses inside the assignment
templates (`yourusername.github.io`, `planning.md`) are now plain text.

## Added in the September 2026 content round (unverified from the sandbox)

| Address | Verdict | Note |
|---|---|---|
| https://www.keithquille.com | CHECK | Supervisor link on the home page and Current Projects; confirm this is his site. |
| https://deweydex.github.io/2plus1Coding | KEEP | Named in that repository's README. |
| https://brilliant.org, https://www.codecademy.com, https://www.khanacademy.org/math, https://tutorial.math.lamar.edu, https://www.3blue1brown.com, https://thecrashcourse.com/topic/literature/ | KEEP | Resources page. |
| https://www.youtube.com/@theartassignment, @3blue1brown, @crashcourse | CHECK | Channel handles; a wrong handle returns a 404. |
