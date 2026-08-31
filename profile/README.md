# Open Engineering Architecture

<p align="center">
  <img src="../assets/hero-banner.png" alt="Open Engineering Architecture" width="100%">
</p>
<p align="center">
  <strong>Make the system understandable before making it complicated.</strong>
</p>

⸻

## Architecture as a First-Class Artifact

Open Engineering Architecture is the architectural home of the Open Engineering ecosystem.

It describes how Open Engineering is structured, how its parts relate to one another, where responsibilities belong, and how the architecture evolves over time.

Architecture here is not merely a collection of diagrams.

It is an executable body of knowledge connecting intent, structure, decisions, models, systems, and runtime reality.
```
Intent
  ↓
Architecture
  ↓
Definitions
  ↓
Compositions
  ↓
Implementations
  ↓
Runtime
  ↓
Observations
  └──────────────→ Architecture
```
The architecture therefore forms part of a continuous engineering feedback loop.

⸻

## The Four Dimensions

Open Engineering describes its architecture through four complementary dimensions.

### 1. Ontology

What things mean.

The ontology establishes the concepts and vocabulary used throughout Open Engineering.

It answers questions such as:

* What is a Pico?
* What is a Capsule?
* What is a Composer?
* What is an Observation?
* What is Evidence?
* What constitutes a Workflow?
* How are these concepts related?

The ontology gives the ecosystem a shared semantic foundation.
```
Concept
   │
   ├── meaning
   ├── relationships
   ├── constraints
   └── vocabulary
```
⸻

### 2. Product Model

What things exist as products and capabilities.

The Product Model organizes Open Engineering into understandable engineering capabilities.

Examples include:

* Definitions
* Conventions
* Capsules
* Composers
* Picos
* Builders
* Sandcastles
* Packages
* Crates
* Sites
* Voices
* Stories
* Academy
* Language Server

The Product Model answers:

What does Open Engineering provide?

⸻

### 3. Systems of Record

Where authoritative information lives.

Open Engineering is deliberately distributed across repositories, schemas, packages, registries, documentation, and runtime systems.

Architecture identifies which source is authoritative for which information.
```
Concept
    ↓
Definition
    ↓
Repository
    ↓
Artifact
    ↓
Registry
```
This prevents architecture from becoming detached from the engineering artifacts it describes.

⸻

### 4. Runtime Architecture

How things actually work.

Runtime Architecture describes the deployed and executing system.

It covers concerns such as:

* Kubernetes
* Crossplane
* FluxCD
* Backstage
* Minikube
* AI agents
* Picos
* Composers
* MCP
* external tools
* messaging
* events
* workflows
* memory
* observability

The Runtime Architecture connects conceptual architecture with operational reality.

⸻

## Architectural Layers

A useful way to understand Open Engineering is as a progression from meaning to execution.
```
┌─────────────────────────────────────────────┐
│                  Ontology                   │
│           What does everything mean?       │
├─────────────────────────────────────────────┤
│               Product Model                 │
│             What do we provide?             │
├─────────────────────────────────────────────┤
│              Systems of Record              │
│           Where does truth reside?          │
├─────────────────────────────────────────────┤
│             Runtime Architecture            │
│             How does it execute?            │
└─────────────────────────────────────────────┘
```
These are not isolated layers.

They are different views of the same engineering system.

⸻

## Architectural Primitives

At the heart of Open Engineering is a small set of reusable architectural primitives.

| Primitive | Responsibility |  
| --- | --- |  
| Observation | Capture what is happening |  
| Investigation | Understand what was observed |  
| Execution | Perform an action |  
| Events | Represent meaningful occurrences |  
| Messaging | Exchange information |  
| Workflow | Coordinate activities |  
| Memory | Retain useful context |  
| Evidence | Support claims and conclusions |  
| Reporting | Communicate findings and state |  
| Composition | Assemble capabilities into larger systems |  

Higher-level capabilities should preferably be composed from these primitives rather than introducing unnecessary new abstractions.

⸻

## From Architecture to Engineering

Architecture should lead somewhere.

Open Engineering connects architectural intent to implementation through a traceable chain.
```
Architecture
     │
     ▼
 Definitions
     │
     ▼
 Conventions
     │
     ▼
   Schemas
     │
     ▼
 Compositions
     │
     ▼
  Artifacts
     │
     ▼
   Runtime
```
This allows architecture to become progressively machine-understandable.

Instead of architecture existing only in documents, architectural knowledge can inform:

* validation;
* IDE assistance;
* code completion;
* generation;
* policy;
* automation;
* documentation;
* visualization;
* AI-agent reasoning.

⸻

## Architecture Is Navigable

A large architecture should not require one enormous diagram.

Open Engineering favors views.

A view answers a particular question for a particular audience.

For example:
```
Open Engineering
       │
       ├── Ecosystem View
       │
       ├── Product View
       │
       ├── Capability View
       │
       ├── Runtime View
       │
       ├── Deployment View
       │
       └── Component View
```
Readers should be able to move from context into detail while retaining an understanding of where they are in the larger system.

⸻

## Architecture as Code

Where practical, architectural information should be represented in structured, version-controlled forms.

That includes:
```
architecture
├── models
├── views
├── decisions
├── definitions
├── relationships
├── schemas
└── documentation
```
This makes architecture:

* reviewable;
* diffable;
* testable;
* searchable;
* visualizable;
* automatable;
* consumable by AI agents.

Diagrams become views generated from architectural knowledge, rather than the architecture itself.

⸻

#3 Visual Architecture

Open Engineering favors architecture visualizations that help people explore systems rather than merely document them.

The architectural toolchain may therefore combine approaches such as:

* LikeC4 for architecture-as-code and navigable views;
* Structurizr/C4 concepts for architectural decomposition;
* SvelteKit for interactive architectural experiences;
* Babylon.js where spatial or 3D representations improve understanding;
* Open Engineering Language Server for schema-aware authoring assistance.

The visualization technology is replaceable.

The architectural model is the durable asset.

⸻

## Architecture Decisions

Important architectural choices should be explicit.

Architecture Decision Records capture:
```
Context
   ↓
Problem
   ↓
Options
   ↓
Decision
   ↓
Consequences
```
An ADR is not simply a historical note.

It provides evidence explaining why the architecture became what it is.

Together, architectural models and ADRs describe both:

what exists

and

why it exists that way

⸻

## Architecture and AI

Open Engineering is designed for an engineering environment in which humans and AI agents work together.

That changes what architectural documentation needs to be.

Architecture should be understandable by both.
```
Human
  │
  ├──────┐
  ▼      ▼
Architecture
  ▲      ▲
  ├──────┘
  │
AI Agent
```
Structured architectural knowledge allows agents to reason about:

* boundaries;
* responsibilities;
* dependencies;
* conventions;
* allowed relationships;
* architectural decisions;
* available capabilities;
* runtime topology.

Architecture therefore becomes part of the context from which engineering agents operate.

⸻

#3 The Architecture Feedback Loop

### Architecture is never finished.

Runtime systems generate observations.

### Observations generate evidence.

Evidence may trigger investigations.

### Investigations may lead to decisions.

Decisions change architecture.
```
Architecture
     ↓
Implementation
     ↓
Runtime
     ↓
Observation
     ↓
Evidence
     ↓
Investigation
     ↓
Decision
     └──────────────→ Architecture
```
This is how Open Engineering keeps architecture connected to reality.

⸻

## Relationship to the Open Engineering Ecosystem

Open Engineering Architecture does not own every implementation.

Instead, it describes how the ecosystem fits together.
```
                    Open Engineering
                          │
                     Architecture
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
   Definitions       Conventions       Composers
        │                 │                 │
        └────────────┬────┴────┬────────────┘
                     │         │
                  Capsules    Picos
                     │         │
                     └────┬────┘
                          │
                       Runtime
```
Individual Open Engineering organizations remain responsible for their respective domains.

Architecture provides the shared map.

⸻

## Guiding Principles

Open Engineering Architecture follows a small number of principles:

### Architecture explains relationships.
A catalog of components is not yet an architecture.

### Models precede diagrams.
Diagrams are views onto architectural knowledge.

### Architecture is versioned.
Architectural evolution should be visible through source control.

### Decisions are evidence.
Important choices should retain their reasoning.

### Runtime informs architecture.
The deployed system is an important source of architectural truth.

### Views serve questions.
Different audiences require different architectural perspectives.

### Machines are readers too.
Architectural knowledge should increasingly be structured so tools and agents can consume it.

### Architecture should enable engineering.
Its purpose is not documentation for its own sake, but better decisions and better systems.

⸻

## Repository Philosophy

Repositories within this organization should represent durable architectural concerns rather than becoming a dumping ground for implementation details.

A repository belongs here when its primary purpose is to answer questions such as:

What is the architecture?

How are these concepts related?

Why was this architectural decision made?

What architectural constraints apply?

How should this system be viewed?

Implementation should remain close to the product or capability that owns it.

⸻

## Open Engineering

Open Engineering treats software engineering as more than producing source code.

It connects:

meaning → architecture → definitions → composition → implementation → runtime → evidence → learning

Architecture provides the map connecting those worlds.

<p align="center">
  <strong>Understand the system. Model the system. Build the system. Learn from the system.</strong>
</p>
<p align="center">
  <a href="https://open-engineering.io">open-engineering.io</a>
</p>
