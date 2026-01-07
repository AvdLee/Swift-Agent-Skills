# Swift Concurrency Agent Skill

An expert-level Agent Skill that transforms Claude into a Swift Concurrency specialist, helping you write safe, performant concurrent code and migrate to Swift 6 with confidence.

This skill is based on the comprehensive [Swift Concurrency Course](https://www.swiftconcurrencycourse.com?utm_source=github&utm_medium=agent-skill&utm_campaign=swift-concurrency-skill), distilling years of real-world experience into actionable guidance for AI assistants.

## What This Skill Offers

This skill provides Claude with comprehensive knowledge of Swift Concurrency best practices, enabling it to:

### Guide Your Concurrency Decisions
- Choose the right tool for the job (async/await, actors, tasks, task groups)
- Understand when to use `@MainActor`, custom actors, or `nonisolated`
- Navigate isolation domains and prevent data races at compile time
- Apply `Sendable` conformance correctly for value and reference types

### Write Safe Concurrent Code
- Avoid common pitfalls like actor reentrancy and retain cycles
- Prevent data races with proper isolation
- Handle task cancellation and error propagation correctly
- Manage memory safely in concurrent contexts

### Optimize Performance
- Identify and fix concurrency bottlenecks using Xcode Instruments
- Choose between serialized, asynchronous, and parallel execution
- Reduce actor contention and unnecessary suspension points
- Understand the tradeoffs of parallelism

### Migrate to Swift 6
- Step-by-step migration strategies for existing codebases
- Enable strict concurrency checking incrementally
- Rewrite closure-based code to async/await
- Migrate from Combine/RxSwift to Swift Concurrency
- Use migration tooling for upcoming Swift features

### Test Concurrent Code
- Write reliable tests using Swift Testing (recommended) or XCTest
- Handle `@MainActor` isolation in tests
- Use `withMainSerialExecutor` for deterministic testing
- Avoid flaky tests with proper async handling

### Integrate with Core Data
- Safely pass data between isolation domains using `NSManagedObjectID`
- Implement the Data Access Object (DAO) pattern
- Use custom actor executors when needed
- Avoid common Core Data concurrency pitfalls

## What Makes This Skill Different

**Expert Knowledge**: Based on real-world experience migrating large production codebases to Swift 6, distilled from the comprehensive [Swift Concurrency Course](https://www.swiftconcurrencycourse.com?utm_source=github&utm_medium=agent-skill&utm_campaign=swift-concurrency-skill).

**Non-Opinionated**: Focuses on industry-standard best practices and compile-time safety, not architectural preferences. Works with any Swift project, coding style, or architecture.

**Swift 6.2 Ready**: Covers the latest Swift Concurrency features including:
- Default Actor Isolation
- `isolated deinit`
- Global Actor Conformance for protocols
- `nonisolated(nonsending)` and `@concurrent`
- Approachable Concurrency build settings
- Concurrency-safe notifications (iOS 26+)

**Practical & Concise**: Assumes Claude is already smart. Focuses on what developers need to know, not what they already understand. Includes code examples for every pattern.

## Following the Agent Skills Open Format

This skill follows the open format for giving agents new capabilities and expertise as described at [agentskills.io](https://agentskills.io/home).

> [!NOTE]
> Agent Skills are folders of instructions, scripts, and resources that agents can discover and use to do things more accurately and efficiently.

Agent Skills are supported by leading AI development tools, including:

- **Cursor** (recommended)
- Claude Code
- Codex

[Check out the full list of adoption](https://agentskills.io/home#adoption).

## Skill Structure

```
swift-concurrency/
├── SKILL.md                    # Main skill file with decision trees
└── references/
    ├── async-await-basics.md   # Fundamentals of async/await syntax
    ├── tasks.md                # Task lifecycle, cancellation, priorities
    ├── sendable.md             # Isolation domains and Sendable conformance
    ├── actors.md               # Actor isolation, global actors, reentrancy
    ├── async-sequences.md      # AsyncSequence and AsyncStream patterns
    ├── threading.md            # Threads vs tasks, suspension points
    ├── memory-management.md    # Retain cycles, weak self, isolated deinit
    ├── core-data.md            # Core Data integration patterns
    ├── performance.md          # Optimization with Xcode Instruments
    ├── testing.md              # Testing concurrent code
    └── migration.md            # Step-by-step Swift 6 migration guide
```

## How to Use

1. **Clone or download** this repository
2. **Place the `swift-concurrency` folder** in your project's `.agent-skills/` directory
3. **Start coding** - Claude will automatically discover and use the skill

Your AI assistant will now have expert-level knowledge of Swift Concurrency and can help you:
- Write new concurrent code from scratch
- Debug concurrency issues and data races
- Migrate existing code to Swift 6
- Optimize performance bottlenecks
- Make informed decisions about concurrency patterns

## Contributing

Found an issue or have a suggestion? Feel free to open a PR or issue. This skill is maintained to reflect the latest Swift Concurrency best practices and will be updated as the language evolves.

## About the Author

Created by [Antoine van der Lee](https://www.avanderlee.com), a Swift Concurrency expert and creator of the [Swift Concurrency Course](https://www.swiftconcurrencycourse.com?utm_source=github&utm_medium=agent-skill&utm_campaign=swift-concurrency-skill). With years of experience migrating large production codebases to Swift 6, this skill distills practical knowledge into actionable guidance for AI assistants.

## License

This skill is open-source and available under the MIT License. See [LICENSE](LICENSE) for details.



