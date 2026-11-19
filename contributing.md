# Contributing

Thanks for helping improve this list.

## What belongs here

Anything that helps someone build, run or operate **Dapr Workflow**:

- SDKs, libraries and tools
- Samples and example applications
- Tutorials, courses and workshops
- Articles, talks and videos
- Durable AI agent projects built on Dapr Workflow

## What does not belong here

- **Other durable execution engines.** This list is scoped to Dapr Workflow, in the same way that a list about any one engine is scoped to that engine. Temporal, Restate, Inngest, DBOS and the rest are out of scope here. For a side-by-side view of the field, see [awesome-durable-executions](https://github.com/edmondop/awesome-durable-executions).
- Dapr content unrelated to workflows or durable execution. The broader [awesome-dapr](https://github.com/mstrYoda/awesome-dapr) list covers Dapr generally.
- Projects that are not publicly available.
- Abandoned projects. Anything without activity in the last 12 months is likely to be removed.
- Marketing pages. Link to the docs, repo or article itself.

## Who maintains this

This list is maintained by [Diagrid](https://www.diagrid.io) (previously Catalyst), which builds a commercial platform on Dapr, and it covers that platform alongside the open-source project. It is not a vendor-neutral comparison of durable execution engines, and it does not try to be. Dapr itself is a CNCF graduated project governed independently of Diagrid.

Within that scope, entries are judged on whether they help someone build with Dapr Workflow, regardless of who published them.

## Entry format

One line per entry, in this shape:

```markdown
- [Name](https://example.com) - Description of what it does, ending with a period.
```

- Put the entry in the most specific section that fits.
- Keep the description to one sentence that says what the thing **does**.
- No marketing language: no "best", "powerful", "revolutionary", "seamless".
- Do not repeat the name inside the description.
- Entries are ordered by how useful they are to a newcomer, not alphabetically.

## Before you open a pull request

```bash
npm install
npm run lint        # awesome-lint
npm run update-toc  # regenerate the Contents section
```

Check that your link resolves and is not already in the list. One pull request per entry is easiest to review, but a themed batch is fine.

## Adding a section

If several related entries do not fit anywhere, open an issue proposing the section before adding it, so the list does not sprawl.
