# Observable CLI

TODO

- ✅ statically render Markdown using markdown-it
- ✅ highlight fenced code blocks using highlight.js
- ✅ JavaScript fenced code blocks ```js
- ✅ JavaScript embedded expressions ${…}
- ✅ automatic reloading when the Markdown is edited
- ✅ viewof equivalent using Generators.input
- ✅ display errors
- vanilla Observable JavaScript
  - ✅ top-level declarations
  - ✅ unbound references (inputs)
  - ✅ awaits
  - ✅ display(…) function
  - ✅ implicit display(…) for expressions
  - ✅ better view shorthand for Generators.input(display(input))
  - ✅ top-level function declaration
  - ✅ top-level class declaration
  - ✅ top-level destructuring patterns (const [x, y] = [0, 0.10])
  - ✅ comprehensive tests for the compiler
  - ✅ static feature detection: files, databases, secrets
  - asynchronous reactive top-level assignment (let y; await; y = 1)
  - implicit declaration for unbound assignment (x = 1)
- rename view(…) to input(…)?
- ✅ embedded JavaScript expressions behave like htl.html (no inspector)
- ✅ file attachments
- database clients (databases registered in YAML or observablehq.json)
- secrets (defined via environment variable?)
- proxied fetch (bypass CORS; registered in YAML or observablehq.json)
- data table display for tabular data (query results, CSV, _etc._)
- SQL fenced code blocks
- more robust inline expressions
  - handle template strings `…` (code_inline)
  - handle backslashes (text_special)
- fenced code block options
  - echo to show code in output
  - output name for SQL cells
  - source database for SQL cells
- HTML fenced code blocks?
- TeX fenced code blocks?
- Graphviz/dot fenced code blocks?
- testing
- routing
- detect broken socket and reconnect
- detect server restart and reload
- snapshot cache
  - proxied fetch
  - database client queries
- static site generation (yarn build)
  - including file attachments
  - including database client query snapshots
  - including fetch snapshots
  - for secrets, use encrypted hash parameters?
- incremental update
  - when Markdown changes
  - when JavaScript changes (both expressions and code blocks)
  - when other live code changes (e.g., SQL, TeX)
  - when attached files change
- imports
  - npm packages
  - local ES modules
  - local Observable Markdown files
  - cloud Observable notebooks?
  - configurable import map?
  - self-host recommended libraries?
  - equivalent to version locking/integrity sha
- standard library 2.0
  - remove deprecated features for standard library
  - Generators.asyncInput
- support ES observables in addition to generators?
- ✅ self-host Observable Runtime instead of jsDelivr CDN
- better theme colors for highlight.js
- better logic for clearing display after invalidation
- Symbol.for("observablehq.display") for custom inspectors?
- header and footer (meta tags, last updated date)
- table of contents (right sidebar)
- cross-notebook navigation (left sidebar)
- footer has link to edit me on GitHub
- client-side search (minisearch)?
- themes
  - default light/dark theme
  - dashboard theme for wide layout
  - custom header and footer