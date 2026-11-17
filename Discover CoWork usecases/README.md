# Discover Your Own AI Use Cases

An offline-first community guide and interactive lab for discovering evidence-led AI use cases, planning a bounded experiment and recording what you learn. The lab is a self-contained HTML page with inline CSS and JavaScript; there is no build, package installation, sign-in or dependency setup.

## Start here

- [Open the interactive lab](index.html) — opens as a working page locally or on GitHub Pages; GitHub's repository file view shows the source instead.
- [Discover Your Own AI Use Cases - Interactive Lab.html](Discover%20Your%20Own%20AI%20Use%20Cases%20-%20Interactive%20Lab.html) — the exact named original interactive companion.
- [Discover Your Own AI Use Cases.md](Discover%20Your%20Own%20AI%20Use%20Cases.md) — the full community guide, including the master discovery prompt and safety boundaries. Read it directly in GitHub or a Markdown viewer; a Pages host may serve the raw Markdown rather than render it.

This scaffold uses the selected **Interactive Lab + Markdown guide**, not the earlier static blog. The prior static `index.html` is not included. Here, `index.html` is a byte-identical copy of the selected interactive lab, provided so GitHub Pages has a conventional entry page.

## What is included

- A discovery-prompt builder with route, scope, focus and source-boundary inputs.
- Searchable illustrative patterns, filtered by category and relative effort; these are not findings about the visitor.
- An experiment planner covering sources, output, stop conditions, human review and learning.
- A self-reported manual-versus-assisted minutes comparison and review checklist.
- Explicit copy/download controls for prompts and experiment cards.
- A companion guide covering evidence, limitations and sanitised community learning.

The lab **does not run AI, connect to Microsoft 365 or other work context, retrieve evidence, send messages, modify work records or activate automation**. Copy the prompt into your organisation-approved experience yourself. Named experiences do not imply feature parity, access, availability, licensing or pricing guarantees. Relative effort labels are not measured credit use, and examples are not validated savings claims.

## Repository layout

```text
ai-use-cases-community/
├── index.html
├── Discover Your Own AI Use Cases - Interactive Lab.html
├── Discover Your Own AI Use Cases.md
├── README.md
├── .nojekyll
└── .gitignore
```

The ZIP has this single enclosing folder. It contains no Git history, `.git` directory, workflows, dependencies or licence file. `.nojekyll` keeps the Pages source as plain static files. `.gitignore` excludes common operating-system/editor cruft; it is not a privacy or secret-scanning control.

## Preview offline

1. Extract the ZIP on your computer.
2. Open `ai-use-cases-community/index.html` in a current browser.
3. Use the builder, filters and planner without a server or internet connection. External reference pages require internet access only if you choose to follow their links.

JavaScript must be enabled for the interactive lab. The Markdown guide remains readable without JavaScript. Clipboard permissions can prevent automatic copying, particularly for local `file:` pages: select the prompt and use your normal Copy command if needed. Download behaviour also depends on browser settings and permissions; check your downloads folder.

## Upload to a GitHub repository

These steps are for you to perform; creating this scaffold has not created or published a remote repository.

1. **Extract `AI Use Cases GitHub Repository.zip`. Do not upload the ZIP itself.**
2. Create a repository in your GitHub account, choosing its name and visibility deliberately. An empty repository avoids conflicts with generated starter files. Review content and reuse rights before making it public.
3. In the repository, use the upload-files link offered for an empty repository, or **Add file → Upload files** where available.
4. **Upload the CONTENTS of `ai-use-cases-community/` to the repository root — not the parent folder.** Include all six files, including `.nojekyll` and `.gitignore`. Your operating system may hide dotfiles; enable hidden-file display if necessary.
5. Enter a meaningful commit message and complete GitHub's commit/propose-changes flow. If you use a branch and pull request, merge the changes into the intended publishing branch.
6. Confirm that `index.html`, both exact named originals, `README.md`, `.nojekyll` and `.gitignore` appear at the repository root, not inside an extra `ai-use-cases-community` directory. The README should render on the repository page.

The separately supplied `AI Use Cases Repository README.md` is an identical reference copy of this README. You do not need to upload that extra standalone filename; the archive already contains `README.md` in the right place.

## Optional: enable GitHub Pages

Hosting is optional; local preview works without it. Availability depends on your account plan, repository visibility and organisation settings. GitHub Free supports Pages for public repositories; private-repository support depends on the plan. Repository admin or maintainer permissions are needed to configure the source.

1. After committing the files, open the repository's **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose the branch containing these files (for example, `main` if that is your branch) and the **root (`/`)** folder, then save.
4. Wait for deployment. Return to **Settings → Pages** and use **Visit site** to open the generated address. Copy the actual address displayed by GitHub; no account-specific site URL is assumed here.
5. Test the builder, filters, planner and downloads on the published site. If publishing fails, inspect the Pages deployment run in the repository's Actions area.

No custom workflow file is supplied or required for this branch-based setup, although GitHub itself uses an Actions deployment run behind the scenes. Publishing can take several minutes. Do not choose `/docs`: this scaffold places `index.html` in the root.

**Treat a Pages site as public internet content, even when its source repository is private.** Host the generic guide and lab only, never private work data, exports or internal evidence.

## Privacy, security and limitations

- The supplied lab has no analytics, external libraries, application network requests or browser-storage implementation. Its only external page links are the official product references, opened when clicked.
- Form values and generated text live in memory in the current tab. Reloading or closing the page loses entries; there is no application autosave or recovery. Browser extensions, browser/session-restoration features and device policies are outside the lab's control.
- Explicit copying and downloading create persistent copies outside the tab. Clipboard history, downloaded files, backups and anything you paste elsewhere remain your responsibility. Refreshing the page does not delete them.
- The no-network statement describes the lab code, not the hosting service: loading a hosted page contacts GitHub Pages, which can process normal hosting/request information under its own policies. Following an external reference contacts that website.
- Never commit personal information, confidential material, credentials, private correspondence, tenant links, customer details or internal project data. A public repository and its history are not a place for work evidence.
- Exports are not automatically sanitised. Review and redact every prompt/card before sharing. Keep authorised source evidence in its approved environment; use only permitted sources and retain human review and decision-making.
- The page cannot verify source claims, actual AI capabilities, permissions, security or measured business value. A checklist is not approval or certification.

## Maintaining the two HTML copies

Both named originals are preserved byte-for-byte in this initial package, and `index.html` exactly matches the named HTML original. The duplicate is intentional: the descriptive filename preserves the selected source while `index.html` provides the site entry point.

For later maintained releases, deliberately update the named lab and copy its complete bytes to `index.html` in the same change; compare them before committing so the two entry points never drift. Do not edit just one copy. If you need an immutable historical original, keep this initial ZIP as your baseline before making future changes. Review JavaScript, links, downloads and privacy behaviour whenever updating the lab. Changes to either source should be explicit, reviewed revisions, not silent substitutions.

## Dates, references and scope

The originals retain their **7 November 2026** community publication date and **7 November 2026** product-reference check date. Packaging them does not revalidate or update their product claims. This README adds repository/hosting guidance only, not new product claims. No private corporate sources have been added.

GitHub instructions were checked against these official GitHub Docs on **17 November 2026**; interfaces and policies can change:

- [Adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [Configuring a publishing source for GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Creating and viewing a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)

## Licence and community reuse

**No licence has been selected on your behalf.** A public upload does not itself grant unrestricted reuse rights. Before public distribution or reuse, confirm ownership and permissions for both originals and any contributions, then choose an appropriate licence if you wish to grant reuse rights. No endorsement by Microsoft or GitHub is implied.

For community contributions, share only sanitised work patterns, redacted prompts, review methods, measured observations and limitations. Do not include source correspondence, identifying details, private links or unsupported performance claims. Check contribution rights and proposed content before merging anything into a public repository.
