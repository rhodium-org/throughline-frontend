# throughline-frontend

The **Google HTML/CSS Style Guide** expressed as a
[throughline](https://pypi.org/project/throughline/) **source** — a standalone,
grounded requirements graph that a consuming project composes with
`tl` from [throughline](https://pypi.org/project/throughline/) 3.11.0 or later.

This repository holds no code. It is a directory of small YAML items with permanent
UIDs, validated by `tl check`. Consumers import it under a namespace and reference
its rules as `frontend:SR-0001`.

## One of three alternative frontend sources

`throughline-frontend` is one of **three alternative frontend sources**, offered as
choices so a project can pick the one matching its priority:

- **`throughline-frontend`** (this repo) — the **markup / style-conventions** choice,
  re-expressing the Google HTML/CSS Style Guide (how HTML and CSS are *authored*).
- **`throughline-frontend-web-vitals`** — the runtime **performance / Core Web Vitals**
  choice.
- **`throughline-frontend-mdn`** — the **web-platform / MDN** choice.

A project composes the one whose emphasis matches its priority; here that priority is
**HTML/CSS authoring style**. The three are orthogonal and **can** be composed together,
but they are presented as alternatives rather than a stack you are expected to adopt
wholesale.

## Status

<!-- tl:count type == 'user_requirement' -->
8
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
41
<!-- tl:end --> style rules, published to [`docs/spec.md`](docs/spec.md):

- `INT-0001` — the root intent (why the guide exists), `normative: false`.
- Each major guide section as a `user_requirement` that `derives_from` the intent.
- Every individual rule as a `system_requirement` that `implements` its section,
  carrying the guide reference in `attrs.source_ref`.

The counts above are rendered from the live graph by the `tl:count` directive, so
they cannot drift.

## Editions — dated tags

The guide is a living document. A material revision is cut as a dated tag on this
repo (e.g. `v2026-08`); a consumer pins the ref it wants.

## Composing it

```toml
[[sources]]
namespace = "frontend"
url = "https://github.com/rhodium-org/throughline-frontend"
ref = "v2026-08"
```

Then reference a rule from your own items:

```yaml
links:
- target: frontend:SR-0001      # Google HTML/CSS Style Guide: use HTTPS for embedded resources
  type: satisfies
```

`tl check` in the consuming project composes this source and resolves the reference.
A `tl` older than 3.11.0 reports it as `namespace-unresolved`.

## Local checks

```sh
pip install throughline
tl check --strict     # the graph must stay sound
tl docs --check       # docs/spec.md must match the graph
```

## Provenance

The Google HTML/CSS Style Guide is © Google, licensed CC BY 3.0. See [NOTICE](NOTICE)
and https://google.github.io/styleguide/htmlcssguide.html. This repository is
Apache-2.0 for its structure and tooling; the reproduced rule text remains Google's.
