# Awesome Dapr Workflow [![Awesome list badge](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Dapr Workflow libraries, samples and resources, from the Dapr project, Diagrid and the wider community. Maintained by Diagrid; scoped to Dapr Workflow rather than durable execution in general. Community links are not endorsed by, affiliated with, or maintained by the Dapr project. Pull requests welcome!

Dapr Workflow is the durable execution engine built into [Dapr](https://dapr.io), a CNCF graduated project. Workflows are written as ordinary code, and a run that is interrupted by a crash, a restart or a deployment resumes from the last completed step instead of starting again.

## Contents

- [Getting started](#getting-started)
- [Documentation](#documentation)
- [Courses and tutorials](#courses-and-tutorials)
- [SDKs](#sdks)
- [Durable AI agents](#durable-ai-agents)
- [Patterns and examples](#patterns-and-examples)
- [Engine internals](#engine-internals)
- [Tools](#tools)
- [Articles](#articles)
- [Videos](#videos)
- [Webinars and workshops](#webinars-and-workshops)
- [Communities](#communities)
- [Related awesome lists](#related-awesome-lists)

## Getting started

- [Dapr Workflow overview](https://docs.dapr.io/developing-applications/building-blocks/workflow/workflow-overview/) - What the engine does and when to reach for it.
- [How to author a workflow](https://docs.dapr.io/developing-applications/building-blocks/workflow/howto-author-workflow/) - Writing your first workflow and activities.
- [Workflow quickstart](https://github.com/dapr/quickstarts/tree/master/workflows) - Runnable quickstart in several languages.
- [Dapr CLI](https://github.com/dapr/cli) - Installs and runs Dapr locally with `dapr init`.

## Documentation

- [Workflow patterns](https://docs.dapr.io/developing-applications/building-blocks/workflow/workflow-patterns/) - Task chaining, fan-out/fan-in, monitors, external events and child workflows.
- [Features and concepts](https://docs.dapr.io/developing-applications/building-blocks/workflow/workflow-features-concepts/) - Determinism, replay, versioning and the constraints they impose.
- [Workflow architecture](https://docs.dapr.io/developing-applications/building-blocks/workflow/workflow-architecture/) - How the engine is built on actors and how state is persisted.
- [Agent integrations](https://docs.dapr.io/developing-ai/agent-integrations/) - Running agent frameworks on Dapr Workflow.

## Courses and tutorials

- [Dapr University: Dapr Workflow](https://www.diagrid.io/dapr-university) - Free video course with hands-on exercises.
- [Workflow tutorials](https://github.com/dapr/quickstarts/tree/master/tutorials/workflow) - Longer tutorials from the Dapr quickstarts repo.
- [Dapr samples](https://github.com/dapr/samples) - Community-contributed samples, several using workflows.
- [Advent of Workflow](https://github.com/diagrid-labs/advent-of-workflow) - Daily challenges for learning durable workflows.
- [Aspire hands-on workshop](https://github.com/diagrid-labs/dapr-workflow-aspire-hands-on) - Build an Aspire .NET Dapr Workflow app step by step.

## SDKs

Workflows can be authored in any of these languages.

- [Go](https://github.com/dapr/go-sdk) - Dapr SDK for Go.
- [Python](https://github.com/dapr/python-sdk) - Dapr SDK for Python.
- [.NET](https://github.com/dapr/dotnet-sdk) - Dapr SDK for .NET.
- [Java](https://github.com/dapr/java-sdk) - Dapr SDK for Java.
- [JavaScript](https://github.com/dapr/js-sdk) - Dapr SDK for JavaScript and TypeScript.
- [Rust](https://github.com/dapr/rust-sdk) - Dapr SDK for Rust.

## Durable AI agents

- [Dapr Agents](https://github.com/dapr/dapr-agents) - Framework for building agents whose state and tool calls run as workflow activities.
- [Agent durability demo](https://github.com/diagrid-labs/agent-durability-demo) - 100 agents draining 10 accounts while the runtime is disrupted.
- [Durable SRE agent](https://github.com/diagrid-labs/diagrid-holmesgpt) - HolmesGPT investigations running as durable workflows.

## Patterns and examples

- [Resiliency and durable execution](https://github.com/diagrid-labs/dapr-resiliency-and-durable-execution) - Applications demonstrating resiliency policies alongside durable execution.
- [Workflow patterns in Spring Boot](https://github.com/diagrid-labs/workflow-patterns-spring-boot) - Dapr Workflow pattern examples for Spring Boot.
- [Workflow demos in Java](https://github.com/diagrid-labs/dapr-workflow-demos-java) - Chaining, fan-out/fan-in and more, in Spring Boot.
- [Spring Boot onboarding](https://github.com/diagrid-labs/dapr-workflow-spring-boot-onboarding) - Employee onboarding modelled as a workflow.
- [Quarkus onboarding](https://github.com/diagrid-labs/dapr-workflow-quarkus-onboarding) - The same scenario on Quarkus.
- [Workflow versioning](https://github.com/diagrid-labs/dapr-workflow-versioning) - Applying versioning to workflows already in flight.

## Engine internals

- [durabletask-go](https://github.com/dapr/durabletask-go) - The durable task engine Dapr Workflow is built on.
- [durabletask-protobuf](https://github.com/dapr/durabletask-protobuf) - Protocol definitions shared by the engine and its clients.
- [durabletask-python](https://github.com/dapr/durabletask-python) - Python client for the engine.
- [durabletask-dotnet](https://github.com/dapr/durabletask-dotnet) - .NET client for the engine.
- [durabletask-java](https://github.com/dapr/durabletask-java) - Java client for the engine.
- [durabletask-js](https://github.com/dapr/durabletask-js) - JavaScript client for the engine.

## Tools

- [Dapr Dev Dashboard](https://github.com/diagridio/dev-dashboard) - Local dashboard for inspecting running workflows and their event history, alongside apps, sidecars, actors and pub/sub.
- [Dapr Skills](https://github.com/diagrid-labs/dapr-skills) - AI coding-assistant skills for scaffolding and reviewing Dapr applications, including workflows.
- [Diagrid](https://www.diagrid.io/platform) - Managed service that hosts the workflow engine and its state stores, so there is no Dapr infrastructure to run yourself.

## Articles

- [An in-depth guide to Dapr Workflow patterns in .NET](https://www.diagrid.io/blog/in-depth-guide-to-dapr-workflow-patterns) - Walkthrough of each pattern with .NET code.
- [Four durable agentic patterns](https://www.diagrid.io/blog/four-durable-agentic-patterns) - Patterns for making an agent loop survive a restart.
- [Agentic durable execution](https://www.diagrid.io/blog/what-is-agentic-durable-execution) - What durability means once an agent, rather than a developer, decides the next step.
- [Dapr actors for scalable workflows and AI agents](https://www.diagrid.io/blog/understanding-dapr-actors-for-scalable-workflows-and-ai-agents) - How the actor model underpins the workflow engine.
- [Versioning .NET workflows in Aspire](https://www.diagrid.io/blog/how-to-version-net-workflows) - Changing a workflow without breaking runs already in flight.
- [Improving the local Dapr Workflow experience](https://www.diagrid.io/blog/improving-the-local-dapr-workflow-experience-diagrid-dashboard) - Inspecting state and event history while developing locally.

## Videos

- [Dapr YouTube channel](https://www.youtube.com/@DaprDev) - Talks, community calls and demos from the Dapr project.
- [Failure is not an option](https://www.diagrid.io/videos/failure-is-not-an-option-durable-execution-dapr-2) - Talk on why distributed applications need durable execution.

## Webinars and workshops

- [Durable workflow patterns in C# with Dapr and Aspire](https://www.diagrid.io/webinars/in-flight-workflows-no-breaking-changes) - Hands-on workshop through the core patterns.
- [Dapr Workflows for Spring Boot 4 developers](https://www.diagrid.io/webinars/dapr-workflows-spring-boot-4-developers-workshop) - Workshop aimed at Java developers.
- [Durable SRE investigations with HolmesGPT](https://www.diagrid.io/webinars/durable-sre-investigations-putting-holmesgpt-into-production) - Taking an SRE agent's investigations to production as durable runs.

## Communities

- [Dapr community](https://dapr.io/community/) - Community calls, mailing list and social channels.
- [Dapr Discord](https://bit.ly/dapr-discord) - The `#workflow` channel is the fastest route to a maintainer.
- [dapr/community](https://github.com/dapr/community) - Governance, working groups and meeting notes.

## Related awesome lists

- [All lists](https://github.com/sindresorhus/awesome)
- [Durable executions](https://github.com/edmondop/awesome-durable-executions)
- [Workflow engines](https://github.com/meirwah/awesome-workflow-engines)
- [Dapr](https://github.com/mstrYoda/awesome-dapr)
- [Agent harnesses](https://github.com/Picrew/awesome-agent-harness)
- Languages with a Dapr SDK:
  - [Go](https://github.com/avelino/awesome-go#readme)
  - [Python](https://github.com/vinta/awesome-python#readme)
  - [.NET](https://github.com/quozd/awesome-dotnet#readme)
  - [Java](https://github.com/akullpp/awesome-java#readme)
  - [JavaScript](https://github.com/sorrycc/awesome-javascript#readme)
  - [Rust](https://github.com/rust-unofficial/awesome-rust#readme)
