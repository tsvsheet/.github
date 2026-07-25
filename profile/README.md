# tsvsheet

> **A spreadsheet in plain text.** A `.tsvt` file _is_ the spreadsheet — a tab-separated grid whose cells are values or `=formulas` that address other cells in A1 notation, computed by a processor, versioned as text, diffed line by line.

Spreadsheets earned their place by making computation visible: a grid you can read, formulas you can point at. What they never earned is a file format — binary blobs and XML archives that no diff can explain and no text editor can open. tsvsheet keeps the grid and the formulas and drops everything else: a `.tsvt` file is tab-separated text, so `=if(A1, C3, D3)` is written verbatim with no quoting or escaping, versioned like source code, reviewed line by line.

The language is specified grammar-first: the ANTLR4 grammar in [tsvsheet](https://github.com/tsvsheet/tsvsheet) is the source of truth, implementations follow it, and the same file computes identically in every runtime.

The org also hosts **[isnow](https://github.com/tsvsheet/isnow)** — a date/time pattern language for repetition: one compact expression describes anything from a fixed instant to a complex recurrence, and answers a single question: _is it now?_

## Explore

- **[tsvsheet](https://github.com/tsvsheet/tsvsheet)** — the grammar-first language home and specification
- **[isnow](https://github.com/tsvsheet/isnow)** — the date/time pattern language and specification
- **[All repositories](https://github.com/orgs/tsvsheet/repositories)** — implementations, integrations, and tooling
