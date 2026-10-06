# How to learn with this setup

Two pieces work together:
- **Claude project "Object Design Learning"** teaches, quizzes and grades. It holds the instructions and the question bank.
- **This folder (`go-patterns`)** is where your code, answers and notes live. It's connected to the project, so Claude can read it.

---

## 1. Commands to use in the Claude project

| Say this | What happens | Where |
|---|---|---|
| `next pattern` | Full lesson for the next unmastered pattern, then Q1–Q10 one at a time | New chat. Rename it to the pattern name afterwards. |
| `quiz me` | Mixed, unlabeled questions across all mastered patterns | New chat called "Quiz – <date>" |
| `refresh me` | 5-line recap + 3 new questions at your weak level | That pattern's own chat |
| `review my code in NN-pattern` | Claude reads your files from this folder and grades them | That pattern's chat |
| `show client code` / `explain again simpler` | Fills any gap in the lesson | Anytime |

Rhythm: **after every 2 mastered patterns, open a quiz chat.** If you miss a question, go back to that pattern's chat and say `refresh me`.

Each chat ends with a **progress card** (Mastered / Weak spots / Next). If a new chat seems unsure where you are, paste the latest card.

---

## 2. At the laptop (this folder)

For each pattern `NN-pattern/`:

1. **Lesson:** paste the client code into `main.go` and run `go run ./NN-pattern`.
2. **Break it on purpose:** add a variant, remove a method, read the compiler error.
3. **Typed answers:** `answers/qN.md` (code in ```go blocks). Runnable answers go in `main.go`.
4. **Ask for a review:** `review Q5 in NN-pattern` in the pattern's chat.
5. **Tests (Q9):** `pattern_test.go`, then `go test ./NN-pattern`.
6. **Notes:** fill in `NOTES.md` in your own words when the pattern is mastered.
7. **Commit after each question:** `git add -A && git commit -m "NN-pattern Q5"`
8. **Mark it mastered** in the README table.

Before a quiz chat: reread only the `NOTES.md` files (about 2 minutes each).

---

## 3. Away from the computer (phone)

Claude can't reach this folder while the laptop is asleep or the Claude desktop app is closed, so:

- **Lesson and recall questions (Q1–Q5, Q10):** answer by hand on paper, then send a photo. Typing short text answers is fine too.
- **Code questions:** use **go.dev/play**. Paste the lesson code, change it, tap **Run**, then tap **Share** and paste the link into the pattern's chat for review.
- **Quiz chats:** work well on a phone. Answer in text or with a photo.
- **Back at the laptop:** copy anything worth keeping from the chat or Playground links into `answers/` or `main.go`, update `NOTES.md`, and commit.

---

## 4. Habits that make it stick
- Never skip the "break it on purpose" step. The compiler errors teach you why the pattern exists.
- Write `NOTES.md` from memory first, then check it against the lesson.
- When you see a pattern in your work code, write it under "Where I saw it at work".
- Mixed quizzes matter more than rereading. Getting things wrong in a quiz is how you learn them.
