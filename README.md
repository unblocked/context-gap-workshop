# context-gap-workshop

## Setup

### MacOS

```
brew install uv gh && gh auth login
gh repo clone your-org/your-repo
```

### Windows

```
winget install astral-sh.uv GitHub.cli
gh repo clone your-org/your-repo
```

### Agent First

Hand this link that has the full instructions.

```
tinyurl.com/contextgap-ai
```

## Commands

### With Local Repo

```
uvx --from git+https://github.com/unblocked/adlc.git adlc baseline --last 1000
uvx --from git+https://github.com/unblocked/engineering-social-graph.git social-graph run --limit 1000
```

### Sample Repo

```
uvx --from git+https://github.com/unblocked/adlc.git adlc baseline --sample
```

## Organization Readiness

[readiness.getunblocked.com](readiness.getunblocked.com)

## Engineering Social Graph

[github.com/unblocked/engineering-social-graph](github.com/unblocked/engineering-social-graph)

## Document Query Engine

[github.com/unblocked/document-query-engine](github.com/unblocked/document-query-engine)
