# Markdown Evolution Proposals

This document will approach three types of proposals to evolve the [Markdown Syntax](https://daringfireball.net/projects/markdown/syntax).

- **patch:** these proposals are compatible with the current markdown and their transpilers.
- **superset:** the proposals here are an evolution that accept the current syntax and new features.
- **breaking change:** a new version that override the old markdown syntax

Each type of proposal is divided in two use cases:

- **for document:** the original reason to markdown exist, to be a web markup language to create text documents
- **for web pages:** Markdown is an HTML superset, the idea is to make it render more complex pages, no only documents, then these proposal bring new common components for content of web pages.

## Patch

### Put markdown information at hidden places.

#### Image

Create

```md
![alt attribute](href?HIDDEN_INFORMATION "title")
```

```md
![The Lord of The Rings cape](/img/tlotr.jpg?mdFloat=right&mdWidth=50 "title")
```

- `mdFloat`
- `mdClass`
- `mdWidth`
  - `mdWidth=50` = 50%
  - `mdWidth=200px` = 200px 
- `mdAlign`
- `mdHeight`

#### Link

```md
[content](href?HIDDEN_INFORMATION "title")
```

```md
[The Lord of The Rings cape](#tlotr?mdType=button "title")
```

- `mdType=button`
- `mdAlign`

    teste de bloco de código
    import { a } from 'jquery'
    <span>

## Superset
