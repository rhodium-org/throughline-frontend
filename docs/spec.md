# Google HTML/CSS style — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from the YAML items, so the published spec can never drift from the graph.

This source re-expresses the **Google HTML/CSS Style Guide** as a grounded IDD graph: each major section is a `user_requirement`, and every individual rule is a `system_requirement` that `implements` its section. The guide reference lives in `attrs.source_ref`; the throughline UIDs are this source's own and immutable — a consumer cites a rule as `frontend:SR-0001`, never by section name.

It carries
<!-- tl:count type == 'user_requirement' -->
8
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
41
<!-- tl:end --> style rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — HTML and CSS are authored in one consistent, maintainable style** — `intent`, status `approved`

> The Google HTML/CSS Style Guide exists so that markup and style sheets across a large codebase read as though written by one author: consistent structure, formatting, naming and feature choices, with structure, presentation and behaviour kept separate, so that any engineer can read and change front-end code they did not write.

**source_ref**: Google HTML/CSS Style Guide
<!-- tl:end -->

## General Style Rules

<!-- tl:item UR-0001 -->
**UR-0001 — General Style Rules** — `user_requirement`, status `approved`

> Rules that apply to both HTML and CSS governing how external resources are referenced.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: General — Style Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: General — Style Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | approved | Use HTTPS for embedded resources |
<!-- tl:end -->

## General Formatting Rules

<!-- tl:item UR-0002 -->
**UR-0002 — General Formatting Rules** — `user_requirement`, status `approved`

> Rules that apply to both HTML and CSS governing indentation, capitalisation and whitespace.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: General — Formatting Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: General — Formatting Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0002 | system_requirement | approved | Indent by two spaces at a time |
| SR-0003 | system_requirement | approved | Use only lowercase |
| SR-0004 | system_requirement | approved | Remove trailing whitespace |
<!-- tl:end -->

## General Meta Rules

<!-- tl:item UR-0003 -->
**UR-0003 — General Meta Rules** — `user_requirement`, status `approved`

> Rules that apply to both HTML and CSS governing encoding, comments and action items.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: General — Meta Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: General — Meta Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0005 | system_requirement | approved | Use UTF-8 without a BOM |
| SR-0006 | system_requirement | approved | Explain code with comments as needed |
| SR-0007 | system_requirement | approved | Mark todos with TODO |
<!-- tl:end -->

## HTML Style Rules

<!-- tl:item UR-0004 -->
**UR-0004 — HTML Style Rules** — `user_requirement`, status `approved`

> Rules governing document type, validity, semantics, fallbacks and attributes in HTML.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: HTML — Style Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: HTML — Style Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0008 | system_requirement | approved | Use the HTML5 document type |
| SR-0009 | system_requirement | approved | Use valid HTML where possible |
| SR-0010 | system_requirement | approved | Use elements for their semantic purpose |
| SR-0011 | system_requirement | approved | Provide multimedia fallbacks |
| SR-0012 | system_requirement | approved | Separate structure, presentation and behaviour |
| SR-0013 | system_requirement | approved | Use entity references only where required |
| SR-0014 | system_requirement | approved | Omit optional tags where beneficial |
| SR-0015 | system_requirement | approved | Omit type attributes for style sheets and scripts |
| SR-0016 | system_requirement | approved | Avoid unnecessary id attributes and hyphenate needed ones |
<!-- tl:end -->

## HTML Formatting Rules

<!-- tl:item UR-0005 -->
**UR-0005 — HTML Formatting Rules** — `user_requirement`, status `approved`

> Rules governing line breaks, line wrapping and quotation marks in HTML.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: HTML — Formatting Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: HTML — Formatting Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0017 | system_requirement | approved | Put each block, list or table element on its own line |
| SR-0018 | system_requirement | approved | Wrap long lines with consistent indentation |
| SR-0019 | system_requirement | approved | Quote attribute values with double quotes |
<!-- tl:end -->

## CSS Style Rules

<!-- tl:item UR-0006 -->
**UR-0006 — CSS Style Rules** — `user_requirement`, status `approved`

> Rules governing validity, naming, selectors and value notation in CSS.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: CSS — Style Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: CSS — Style Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0020 | system_requirement | approved | Use valid CSS where possible |
| SR-0021 | system_requirement | approved | Name classes by meaning, not appearance |
| SR-0022 | system_requirement | approved | Keep class names as short as possible but as long as necessary |
| SR-0023 | system_requirement | approved | Separate words in class names with a hyphen |
| SR-0024 | system_requirement | approved | Optionally prefix selectors with an application-specific namespace |
| SR-0025 | system_requirement | approved | Do not qualify class selectors with type selectors |
| SR-0026 | system_requirement | approved | Avoid ID selectors |
| SR-0027 | system_requirement | approved | Use shorthand properties where possible |
| SR-0028 | system_requirement | approved | Omit units after a zero value |
| SR-0029 | system_requirement | approved | Include a leading zero in fractional values |
| SR-0030 | system_requirement | approved | Use three-character hex notation where possible |
| SR-0031 | system_requirement | approved | Avoid !important declarations |
| SR-0032 | system_requirement | approved | Avoid user agent detection and CSS hacks |
<!-- tl:end -->

## CSS Formatting Rules

<!-- tl:item UR-0007 -->
**UR-0007 — CSS Formatting Rules** — `user_requirement`, status `approved`

> Rules governing declaration order, indentation, spacing and quotation marks in CSS.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: CSS — Formatting Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: CSS — Formatting Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0033 | system_requirement | approved | Alphabetise declarations |
| SR-0034 | system_requirement | approved | Indent all block content |
| SR-0035 | system_requirement | approved | End every declaration with a semicolon |
| SR-0036 | system_requirement | approved | Put a space after a property colon |
| SR-0037 | system_requirement | approved | Put a space before a declaration block |
| SR-0038 | system_requirement | approved | Separate selectors and declarations by new lines |
| SR-0039 | system_requirement | approved | Separate rules by blank lines |
| SR-0040 | system_requirement | approved | Use single quotes for CSS values and selectors |
<!-- tl:end -->

## CSS Meta Rules

<!-- tl:item UR-0008 -->
**UR-0008 — CSS Meta Rules** — `user_requirement`, status `approved`

> Rules governing the organisation of a style sheet with section comments.

*Derives from:* INT-0001

**source_ref**: Google HTML/CSS Style Guide: CSS — Meta Rules
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google HTML/CSS Style Guide: CSS — Meta Rules') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0041 | system_requirement | approved | Group sections with a section comment |
<!-- tl:end -->

