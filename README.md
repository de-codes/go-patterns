# go-patterns

My workbook for the 23 GoF design patterns in Go. **Start with [HOW-TO-LEARN.md](HOW-TO-LEARN.md).**

## Workflow (per pattern)
1. In the Claude project, type `next pattern` and read the lesson.
2. Copy the lesson's client code into `NN-pattern/main.go`. Run it: `go run ./NN-pattern`
3. Change one thing (add a new variant) and run again.
4. Typed quiz answers go in `NN-pattern/answers/qN.md` (code inside ```go blocks). Anything you want to run goes in `main.go`.
5. Tests go in `NN-pattern/pattern_test.go`. Run all: `go test ./...`
6. Fill in `NN-pattern/NOTES.md` in your own words: hook, analogy, 3-line recap, mistakes I made.
7. Commit: `git add -A && git commit -m "NN-pattern: <what you did>"`

Mixed-quiz answers go in `quiz/`.

## Patterns
| # | Pattern | Type | Mastered |
|---|---|---|---|
| 01 | Strategy | Behavioral | |
| 02 | Observer | Behavioral | |
| 03 | Factory Method | Creational | |
| 04 | Singleton | Creational | |
| 05 | Builder / Functional Options | Creational | |
| 06 | Adapter | Structural | |
| 07 | Decorator | Structural | |
| 08 | Proxy | Structural | |
| 09 | Facade | Structural | |
| 10 | Chain of Responsibility | Behavioral | |
| 11 | Command | Behavioral | |
| 12 | State | Behavioral | |
| 13 | Template Method | Behavioral | |
| 14 | Iterator | Behavioral | |
| 15 | Composite | Structural | |
| 16 | Abstract Factory | Creational | |
| 17 | Prototype | Creational | |
| 18 | Bridge | Structural | |
| 19 | Mediator | Behavioral | |
| 20 | Memento | Behavioral | |
| 21 | Visitor | Behavioral | |
| 22 | Flyweight | Structural | |
| 23 | Interpreter | Behavioral | |
