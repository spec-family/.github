# The spec family

**Hold your code, and the agents that write it, to what your Markdown says.**

Four deterministic command-line tools that read the Markdown a repository
already keeps - specifications, ADRs, READMEs, agent instructions, briefs -
and check what it says against the code, the git history and the changes an
agent made. No model reads the documents, nothing leaves the machine, and a
run says the same thing every time.

| Tool | Keeps true |
| --- | --- |
| [spec-guard](https://github.com/spec-family/spec-guard) | the rules any Markdown states, run against the code; each claim held to its evidence |
| [spec-graph](https://github.com/spec-family/spec-graph) | the documents against each other and the repository: references, retired decisions, ticked boxes, the paths an agent's instructions name |
| [spec-brief](https://github.com/spec-family/spec-brief) | the briefs a round of agent work runs under, and which of them can run side by side |
| [spec-harness](https://github.com/spec-family/spec-harness) | a round of agent work against its brief: a guard on the agent's writes, and an audit at the end |

## Start here

- **[spec-family.github.io](https://spec-family.github.io)**: what each tool does, with output the released tools printed.
- **[spec-family/example](https://github.com/spec-family/example)**: a small repository the four keep true, with two pull requests they turn red.
- **In CI**: [spec-family/action](https://github.com/spec-family/action), one GitHub Action for all four.
- **With Spec Kit**: [spec-family/spec-kit-extension](https://github.com/spec-family/spec-kit-extension).
- **For an agent**: spec-guard and spec-harness are MCP servers, listed in the official MCP Registry as `io.github.spec-family/*`.
- **How they fit together**: the [overview](https://github.com/spec-family/spec-core/blob/main/docs/overview.md) and the [adopting guide](https://github.com/spec-family/spec-core/blob/main/docs/adopting.md).

Install from npm under the `@spec-family` scope, and run a tool as
`npx --no-install @spec-family/<tool>`: the unscoped names on npm are not
these packages.

## Tried it?

Open an issue in the tool's repository and say what happened: a finding that
was wrong, a page that did not make sense, or simply that it ran on your
repository. Each repository's issue form asks for what helps.
