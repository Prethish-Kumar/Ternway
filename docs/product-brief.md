# Ternway product brief

## Vision

Ternway is intended to be a fast, full-featured API testing client: an alternative to Postman that also includes a built-in load balancer. It should help developers work with APIs without making everyday request testing feel slow or cumbersome.

## Problem

Developers need a convenient way to construct requests, inspect responses, and repeat API tests. A single client that also offers load balancing could make it easier to work with services running across multiple endpoints.

## Intended users

Developers, QA engineers, and other technical users who build, test, or troubleshoot APIs.

## Product goals

- Make common API testing workflows fast and straightforward.
- Provide the breadth expected of a full API testing client.
- Include load balancing as a built-in capability rather than requiring a separate tool.
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

### Built-in load balancer

- Configure multiple service endpoints and distribute requests between them.
- Make the selected endpoint and request outcome visible for troubleshooting.
- Define routing behavior and failure handling once the intended operating model is established.

Load balancing is not the same as load testing: distributing requests across endpoints does not by itself generate or measure high traffic. Whether Ternway should also provide load testing remains open.

## Product principles

- **Speed:** prioritize responsive common workflows and measure performance before making claims.
- **Clarity:** make requests, responses, routing decisions, and failures understandable.
- **Safety:** treat credentials and other sensitive request data carefully; define storage and sharing behavior explicitly.
- **Practicality:** keep the core request workflow approachable as capabilities grow.

## Open decisions

- What is the initial release scope and which API protocols are required first?
- Is the load balancer limited to requests sent by Ternway, or should it also serve external clients as a standalone proxy?
- Which routing strategies, health checks, and failure behaviors are needed?
- Is load testing also a product goal? If so, what workloads and measurements should it support?
- Which platforms and deployment model should be supported?
- How should data, credentials, environments, and collections be stored, shared, and synchronized?
- What security, privacy, performance, and compatibility requirements define success?
- Which technologies and application architecture best serve these requirements?

## Next steps

Resolve the load-balancer operating model and initial release scope, then turn those decisions into concrete workflows, requirements, and an implementation plan.
