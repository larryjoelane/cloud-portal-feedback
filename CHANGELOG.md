# Changelog

What changed in Cloud Portal, newest first.

## 2026-11-07

- **Your own OpenRouter account for the coding agent.** Start a session on your own OpenRouter account to use any model, paid ones included, billed to you. You approve each session on OpenRouter's page. The portal never saves your key: it's used for that session only and forgotten when the session ends.
- **Build arguments and build secrets.** Apps can keep values their builds need. Secrets (such as a private npm token) reach only the Dockerfile step that asks for them (`RUN --mount=type=secret,id=NAME,env=NAME`) and never end up in the image. Once saved, a secret's value is never shown again.
- **Start again.** An ended agent session can be started again with the same namespace, model, repository and branch.
- **The agent saves its work more reliably.** It now makes every change in the files rather than pasting code into the chat. When a reply shows code but no file changed, the chat says so and suggests a stronger model.

## 2026-11-05

- **Save to GitHub.** The coding agent's work can be published from the session: pick the changed files, describe them, push a branch and open a pull request, step by step in plain words.

## 2026-11-03

- **Coding agent.** An AI agent that reads, writes and runs code in a sandbox in one of your namespaces, starting from a public GitHub repository if you like. Free models are included.

## Earlier

- Build images from a Dockerfile in the cluster, from a project folder or a public GitHub repository.
- Upload container images directly.
- Deploy apps with HTTPS, storage that survives restarts, and per-namespace budgets.
