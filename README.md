# Jonah Wood

Electrical & Computer Engineering at Northeastern, class of 2030. Former FTC
robotics kid. I mostly build things from scratch to find out how they work —
engines, optimisers, and whatever tool the day needed.

### Things I've built

**[canvas-achieve-sync](https://github.com/IfAnyoneCould/canvas-achieve-sync)** — Python
I kept missing assignments that lived in four different places, so I wrote
something to put them all in one list. It pulls from the Canvas API, the
Achieve textbook platform (browser-driven, since there's no API), the
university calendar and a homework packet parser, reconciles everything against
existing tasks, and writes to Google Tasks. Runs unattended every two hours on
a scheduled task and has been for months. Source and target backends are
separate, so adding a new one doesn't touch the sync logic.

**[cpp-game-engine](https://github.com/IfAnyoneCould/cpp-game-engine)** — C++20, SDL2, OpenGL
A 2D engine with no framework underneath it. Fixed 240 Hz physics on an
accumulator with rendering decoupled, SAT and AABB collision, sprite sheets and
animation, bitmap text. The part I like most is that levels are authored as
images: you paint a PNG, and a small text file maps pixel colours to object
templates, so the engine builds the world from the picture.

**[Evolution_Engine](https://github.com/IfAnyoneCould/Evolution_Engine)** — Go
A genetic algorithm that optimises *any* program. It talks to workers over
stdin/stdout with one JSON array of weights in and one fitness number out, so
the thing being optimised can be written in any language. First working version
spawned a process per evaluation and took ~900 ms a batch; moving to persistent
workers on a pooled channel got it under 1 ms.

**[neu-clubs](https://github.com/IfAnyoneCould/neu-clubs)** — Python ·
**[downloads-janitor](https://github.com/IfAnyoneCould/downloads-janitor)** — PowerShell
Two smaller tools. The first scrapes Northeastern's club directory into one
sortable table of all 933 student groups because the official site can't be
filtered usefully. The second keeps my Downloads folder from becoming a
workspace again — it archives by age into dated buckets, ages a folder by the
newest file inside it so active work is never swept, and logs every move to a
ledger so anything can be put back.

### Currently

Rewriting my N-dimensional Perlin noise generator, which produces noise that is
technically random and aesthetically wrong.

### Tools

C++ · Go · Python · Java · PowerShell · SDL2/OpenGL · CMake · Docker · PostgreSQL
