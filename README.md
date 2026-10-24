# Selected engineering projects

A minimal static gallery for the existing root GitHub Pages repository. Semantic HTML and CSS; no dependencies, JavaScript, build step, analytics, or external fonts.

## Preview and publication

Run `python3 -m http.server 8000` and open `http://localhost:8000`.

Relative stylesheet links work at the root Pages URL, `https://lfarci.github.io/`. The repository already serves a placeholder there. This branch prepares the gallery only: a draft PR is not proof of deployment. After approved merge, verify the Pages deployment and rendered page before linking from other surfaces. No deployment workflow is added or dispatched for this change.

## Project content contract

Each `<article>` in `index.html` is one project record. Keep these fields explicit:

| Field | HTML representation |
| --- | --- |
| Name | Unique `h3` and `aria-labelledby` |
| Problem and role | `dl` entries describing purpose and personal contribution |
| Stack | Labeled list |
| Status | Text, not color alone |
| Preview | Labeled illustration or current screenshot with useful alternative text |
| Source/demo | Descriptive links; demo only when deployed |
| Limitations | Visible paragraph |
| Decisions/findings | `dl` entry supported by public evidence |

Initial content uses public README evidence from [C# Quest Tracker](https://github.com/lfarci/csharp-quest-tracker) and [Agent Portability Lab](https://github.com/lfarci/agent-portability-lab), reviewed October 24, 2026. Previews are illustrations, not screenshots or fabricated runtime results. Scope experimental findings to the versions and dates actually tested.

## Review checklist

- Check source/demo/result links and project status.
- Inspect mobile and desktop widths, including horizontal overflow at 320px.
- Navigate by keyboard, including the skip link and visible focus rings.
- Preserve heading order, descriptive links, contrast, and reduced-motion behavior.
- Keep private and client-sensitive information out of public output.
- After deployment is confirmed, track website, GitHub profile, and LinkedIn gallery links in their owning issues. This PR updates no other surface.
