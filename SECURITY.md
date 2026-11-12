# Security policy

This is the policy of every spec-family repository that has none of its own.
spec-core, spec-brief, spec-graph, spec-guard and spec-harness each keep
their own SECURITY.md, which says the same for that tool.

## Reporting a vulnerability

Report it privately, through GitHub's private vulnerability reporting: the
repository's **Security** tab, then **Report a vulnerability**. Only the
maintainer sees the report.

Do not open a public issue, pull request or discussion about a vulnerability,
and do not show it in one, until a fix is out.

A useful report names the repository and the version or commit, what an
attacker has to control, what happens then, and the smallest reproduction
you have.

## What to expect

- An acknowledgement of the report.
- A fix in a release, with an advisory that says which versions are affected
  and what to upgrade to. For spec-family/action and
  spec-family/spec-kit-extension, which users pin by tag, the advisory names
  the tag to move to.
- Credit in the advisory and the changelog, if you want it.

The spec family has a single maintainer; a fix is made on the latest
release only.
