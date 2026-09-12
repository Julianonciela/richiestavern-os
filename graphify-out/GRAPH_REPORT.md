# Graph Report - rt-os  (2026-09-12)

## Corpus Check
- 4 files · ~5,423 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 25 nodes · 21 edges · 4 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `b6eab4a3`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- Richie's Tavern Operating System (RT-OS)
- The First Impression
- Reading the Room
- vercel.json

## God Nodes (most connected - your core abstractions)
1. `Richie's Tavern Operating System (RT-OS)` - 8 edges
2. `The First Impression` - 5 edges
3. `Reading the Room` - 4 edges
4. `buildCommand` - 1 edges
5. `outputDirectory` - 1 edges
6. `installCommand` - 1 edges
7. `routes` - 1 edges
8. `Project identity` - 1 edges
9. `Tech stack` - 1 edges
10. `File map` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Import Cycles
- None detected.

## Communities (4 total, 0 thin omitted)

### Community 0 - "Richie's Tavern Operating System (RT-OS)"
Cohesion: 0.22
Nodes (8): Access codes, Active cron jobs (VPS), Design tokens, File map, Key conventions, Project identity, Richie's Tavern Operating System (RT-OS), Tech stack

### Community 1 - "The First Impression"
Cohesion: 0.33
Nodes (5): The 10-Second Rule, The First Impression, The Promise, Why It Works, Why the first 30 seconds matter

### Community 2 - "Reading the Room"
Cohesion: 0.40
Nodes (4): Reading the Room, The Golden Rule, The skill that separates good from great, What to Look For

### Community 3 - "vercel.json"
Cohesion: 0.40
Nodes (4): buildCommand, installCommand, outputDirectory, routes

## Knowledge Gaps
- **18 isolated node(s):** `buildCommand`, `outputDirectory`, `installCommand`, `routes`, `Project identity` (+13 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 21 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What connects `buildCommand`, `outputDirectory`, `installCommand` to the rest of the system?**
  _18 weakly-connected nodes found - possible documentation gaps or missing edges._