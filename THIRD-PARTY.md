# Third-party notices

This site's own text and markup are Grispy's. The following third-party material
is served from it, under its own terms.

## Lucide icons

The guide draws two controls as inline SVG rather than as look-alike characters,
so that a picture of a button in the guide is the same artwork the popup renders:

| Icon | Where |
|---|---|
| `ellipsis` | `guide/saving-and-filling/` — the menu beside the saved date |
| `plus` | `guide/saving-and-filling/` — the *This form* strip's create chip |

Both are copied verbatim as path data from `lucide-static@1.34.0`, by way of the
extension's own `src/shared/icons.js`, which vendors the same version. **There is
one copy of each shape and it is that file** — these are transcriptions of it, not
a second source. Nothing is fetched at runtime: this site loads no script, no
font and no stylesheet from any other origin, which is the same property
`/privacy/` claims for the extension.

Source: <https://lucide.dev> · <https://github.com/lucide-icons/lucide>

**Both notices below apply.** `ellipsis` descends from the Feather project, under
the name Lucide renamed — it was Feather's `more-horizontal` — which the
extension's own notice establishes. `plus` shares its name and its two-stroke
geometry with a Feather icon, and that descent has **not** been checked against
Feather's source the way the extension's entries were, so the MIT notice is
applied to it conservatively rather than on evidence.

### ISC License (Lucide)

```text
ISC License

Copyright (c) 2026 Lucide Icons and Contributors

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### MIT License (Feather)

```text
The MIT License (MIT)

Copyright (c) 2013-present Cole Bemis

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
