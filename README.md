🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

> Build a social bingo game. Learn to direct an AI development team.

Soc Ops is a hands-on VS Code GitHub Copilot Agent Lab built around a real Spring Boot
application. Start with a playable social bingo board, then use Copilot's agentic tools to
shape its design, generate themed prompts, and add features with tests.

[Start the workshop](workshop/GUIDE.md) · [Run the game](#run-locally) · [Browse the lab](#workshop-path)

## The Mission

At an in-person mixer, players find people who match each square and mark their board. Five
in a row wins. The game is deliberately small enough to understand quickly and rich enough to
give AI-assisted development real work to do.

| What you build | What you practice |
|---|---|
| A responsive 5 x 5 social bingo board | Context engineering for repository-aware agents |
| Fresh, randomized prompt boards | Design-first iteration with specialized agents |
| Win detection, persistence, and a victory state | Red-green-refactor development and multi-agent workflows |

## Workshop Path

The lab takes about one hour and assumes familiarity with Java and VS Code. Work through the
chapters in order, or jump to the capability you want to explore.

| Part | Focus | Time |
|---|---|---|
| [**00**](workshop/00-overview.md) | Overview and environment checklist | Start here |
| [**01**](workshop/01-setup.md) | Setup and context engineering | 15 min |
| [**02**](workshop/02-design.md) | Design-first frontend development | 15 min |
| [**03**](workshop/03-quiz-master.md) | Create a themed Quiz Master agent | 10 min |
| [**04**](workshop/04-multi-agent.md) | Deliver a feature with multiple agents | 20 min |

The full guide is also available on the [GitHub Pages workshop site](https://copilot-dev-days.github.io/agent-lab-java/).

## Run Locally

**You need:** [Java 21 JDK](https://adoptium.net/) or later. The included Maven Wrapper handles Maven for you.

```bash
cd socops
./mvnw spring-boot:run
```

Open [http://localhost:8080](http://localhost:8080), choose **Start Game**, and find your first five-in-a-row.

## Project Snapshot

- **Java 21** and **Spring Boot 3.4** provide the application and board API.
- **Thymeleaf** serves the game shell; the browser manages the interactive board and restores game state locally.
- **Maven**, **JUnit**, and **Checkstyle** keep each workshop increment reliable.

## Build And Test

```bash
cd socops
./mvnw clean package
```

```bash
cd socops
./mvnw test
```

The workshop site deploys to GitHub Pages whenever changes are pushed to `main`.
