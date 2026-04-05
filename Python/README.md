## 1) Python Distilled:
- Advancements: page 62
- Will probably not finish it, too "distilled", doesn't go enough in depth

## 2) Fluent Python:
- Started: 14/01/2026
- Chapters read: 1, 2, 3, 19
- Advancements: ...
    - Chapter: Data Class Builders, read until 198
    
Next move: read chapters 19 to 21. Get a global understanding, then implement something real and fun to fully understand the concepts while making back and forth with the book.



Ch. 3 — Dictionaries and Sets (read almost fully)
This is “Python-in-production” core: dict merging, missing keys, defaultdict, hashability, views, performance implications.
Direct payoff: cleaner code, fewer bugs, better data modeling, interview strength.

Ch. 6 — Object References, Mutability, and Recycling (read almost fully)
This is the source of 80% of subtle bugs in Python codebases (aliasing, shallow copy, default mutable args, is vs ==).
Direct payoff: debugging speed, correctness, avoiding footguns.

Ch. 8 — Type Hints in Functions (selective but important)
Focus on:
optional/union, generics (list[str], dict[str, X])
protocols/ABCs basics (what typing is really doing)
“mypy more strict” mindset
Direct payoff: large codebase readability, safer refactors, strong signal in interviews.

Ch. 17 — Iterators, Generators, and Classic Coroutines (read the “iter/generator/itertools” parts)
Focus on:
iterables vs iterators
generator functions/expressions
itertools patterns
“when to use generator expressions”
Direct payoff: writing clean, memory-efficient code; very useful in data-ish tasks + interviews.



If you do only those 4, you’ll already be way ahead of most Python devs.
High ROI “add-ons” (only the useful sections)
These are “open when needed” chapters:

Ch. 4 — Unicode Text Versus Bytes (skim now, revisit when pain hits)
You don’t need to master it today, but when you hit encoding issues in logs/files/APIs, this chapter saves hours.

Ch. 9 — Decorators and Closures (read the practical bits)
Read:
closures + nonlocal (so you understand what you’re seeing)
functools.cache/lru_cache
singledispatch
Skip fancy decorator theory unless you actually implement decorators.

Ch. 19–21 — Concurrency / Executors / Async (read conceptually, not line-by-line)
For Checkout backend, this matters, but you can keep it conceptual until you touch async/concurrency directly. Your main win here is knowing:
what the GIL means (and what it doesn’t)
when threads/processes/async make sense
where people accidentally block the event loop

Ch. 22 — Dynamic Attributes and Properties (read the “properties for validation/caching” parts)
Very relevant to “clean up 200-line functions” and enforcing invariants.