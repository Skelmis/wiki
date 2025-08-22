+++
date = '2025-08-17'
title = 'Reporting Engines'
+++
Need to write reports in a consistent format but don't want to use boring old word? These might be what your looking for.

{{< toc >}}

I've done a bunch of stuff in this space over the years and figured it'd be nice to collate the various reporting engines I have found in a single space.

## Pandoc
_The classic file converter_

Takes in whatever you want, creates whatever you desire. Lacks a lot of functionality on its own that a reporting engine should have (in my opinion).

Link: <https://pandoc.org/>

## Pike by Skelmis
_Built by me to generate anything, not just pentest reports_

Reporting is complicated, and that annoys me. Pike provides a high degree of flexibility allowing end users to do whatever they want however they want.

I use this for all my bug bounty needs as well as an intermediary on professional reports I write.

Features such as:
- Insanely fast out of the box (Max runtime of ~5-10 seconds)
- Easy to implement custom plugins for use in markdown files
- Call directly to the docx engine where required

Uses:
- Markdown & Jinja2
- Layout is defined as Markdown file
- Call directly to the word docx library from markdown when needed

Generates:
- Markdown
- Docx
- PDF

Via:
- `python main.py`

Link: <https://github.com/skelmis/pike>

## Report Forge by Itz-D0dgy
_Built by a friend who tried alternatives and didn't like em_

ReportForge is a high-performance pentest report generation tool (for now) built with Golang, designed for speed, efficiency, and flexibility. Using HTML and CSS3 for templating, it enables fully customizable, visually stunning reports that can be exported to PDF 

Uses:
- Markdown & Go's templating support

Generates:
- HTML
- PDF from said HTML

Via:
- `go run ...`

Link: <https://github.com/itz-d0dgy-2nd/ReportForge>

## Report Ranger by Volkis
_The closest thing to an industry standard reporting engine I've found._

A document generator that builds the appropriate markdown for use with the pandoc-latex-template or to HTML code. Automatically sorts all vulns and appendices, uses Jinja2 for templating.

Personally I've heard mixed takes on it, with people often struggling to extend the functionality.

Uses:
- Markdown & Jinja2

Generates:
- PDF's via Pandoc/LaTeX
- HTML

Via:
- `python reportranger ...`

Link: <https://gitlab.com/volkis/report-ranger>

## Report Repulsor by Volkis
_The replacement to report ranger_

A tool/template for building reports using [Typst](https://typst.app/).

Never personally used it, but Typst seems like a potentially cool LaTeX replacement. If considering, look at the Typst format spec and example findings to see if you actually like the template language.

Uses:
- Typst

Generates:
- PDF

Via:
- `python generatemeta.py watch`
- `typst` binary

Link: <https://gitlab.com/volkis/rr>

## Sysreptor by Syslifters

A customizable and powerful penetration testing reporting platform for offensive security professionals. Simplify, customize, and automate your pentest reports with ease. 

Uses:
- Markdown
- HTML / Vuejs for styling

Generates:
- PDF

Via:
- Browser connecting to running server / local deployment

Link: <https://github.com/Syslifters/sysreptor>

## Writehat by Black Lanturn Security

A pentest reporting tool written in Python that runs in the browser with support for a bunch of nice quality of life features.

Uses:
- Markdown

Generates:
- HTML
- PDF

Via:
- Browser connecting to server / local deployment

Link: <https://github.com/blacklanternsecurity/writehat>

## Notable Mentions

The following provides a list of other pentesting engines n such. I've never read into them much but hey its a list <https://inventory.raw.pm/tools.html#title-tools-collaboration-and-report>