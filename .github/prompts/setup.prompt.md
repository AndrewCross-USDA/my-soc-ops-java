---
agent: agent
description: Get my development workspace ready
tools: ['vscode/openSimpleBrowser', 'execute/runTask', 'execute/runInTerminal', 'read', 'search', 'todo']
---

## Mandatory development checklist
- [ ] Verify Java 21 JDK
- [ ] Lint passes
- [ ] `./mvnw clean package` passes
- [ ] `./mvnw test` passes
- [ ] Start `./mvnw spring-boot:run`
- [ ] Open the site and give a short welcome tour