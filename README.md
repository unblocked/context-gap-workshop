# How to map, measure, and close the context gap

We are going to do three things in this lab: work out where your organization stands today, measure what your delivery looks like right now, and work out what it would take to close that gap.

## Setup

To prepare for that we need to set up some tools on your machine, or if you have an agent like claude code handy you can just point it at this url [tinyurl.com/contextgap-ai](tinyurl.com/contextgap-ai).

They run locally, nothing will leave your machine.

This will show you roughly where your delivery stands, who on your team holds the knowledge everyone else depends on, and where the bottlenecks are.

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

## Commands

### adlc

This command runs a tool called adlc, which stands for AI development lifecycle. It reads the pull request history of the repository you cloned and reports how fast that repository ships.

```
uvx --from git+https://github.com/unblocked/adlc.git adlc baseline --last 1000
uvx --from git+https://github.com/unblocked/engineering-social-graph.git social-graph run --limit 1000
```

### social-graph (Requires repo access)

This command runs a tool called social-graph. It reads the same pull request history and works out who reviews whose work and where the expertise in the codebase lives.

## Organization Readiness

[readiness.getunblocked.com](readiness.getunblocked.com)

## Engineering Social Graph

[github.com/unblocked/engineering-social-graph](github.com/unblocked/engineering-social-graph)

## Document Query Engine

[github.com/unblocked/document-query-engine](github.com/unblocked/document-query-engine)
