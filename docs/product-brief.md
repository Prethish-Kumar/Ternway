# Ternway product brief

## Vision

Ternway is intended to be a fast, full-featured API testing client: an alternative to Postman that also includes built-in load testing inspired by k6. It should help developers work with APIs without making everyday request testing feel slow or cumbersome.

## Problem

Developers need a convenient way to construct requests, inspect responses, and repeat API tests. They also need to understand how APIs behave under load. Combining these workflows in one client could make it easier to move from functional testing to performance testing.

## Intended users

Developers, QA engineers, and other technical users who build, test, or troubleshoot APIs.

## Product goals

- Make common API testing workflows fast and straightforward.
- Provide the breadth expected of a full API testing client.
- Include load testing as a built-in capability rather than requiring a separate tool.
- Make request results and errors clear enough to support troubleshooting.

## Candidate capabilities

These are planning targets, not implemented features or a committed release scope.

### API testing

- Create, edit, send, and save requests, including methods, URLs, headers, query parameters, and bodies.
- Inspect response status, headers, body, timing, and errors.
- Organize and reuse requests in collections, with environment-specific variables.
- Configure common authentication methods without exposing secrets unnecessarily.
- Define repeatable checks and run groups of requests.
- Import and export API definitions or collections where useful for adoption and interoperability.

### Built-in load testing

- Define workloads that send requests with configurable concurrency, rate, and duration.
- Exercise API requests under sustained or changing load.
- Inspect performance results such as throughput, latency, and error rates.
- Define checks or thresholds to evaluate results against performance expectations.
- Reuse API requests and configuration where practical.

## Product principles

- **Speed:** prioritize responsive common workflows and measure performance before making claims.
- **Clarity:** make requests, responses, load-test results, and failures understandable.
- **Safety:** treat credentials and other sensitive request data carefully; define storage and sharing behavior explicitly.
- **Practicality:** keep the core request workflow approachable as capabilities grow.

## Open decisions

- What is the initial release scope and which API protocols are required first?
- Which workload models, metrics, and thresholds should load testing support first?
- Should load tests run locally, remotely, or in a distributed environment?
- What level of k6 script or result compatibility, if any, is needed?
- Which platforms and deployment model should be supported?
- How should data, credentials, environments, and collections be stored, shared, and synchronized?
- What security, privacy, performance, and compatibility requirements define success?
- Which technologies and application architecture best serve these requirements?

## Next steps

Resolve the initial API and load-testing scope, then turn those decisions into concrete workflows, requirements, and an implementation plan.
