# Contributing to FED‑Badge

Thank you for considering a contribution to **FED‑Badge**! We welcome bug reports, feature requests, documentation improvements, and code patches of every size.

## Code of Conduct

Be kind and constructive. Treat everyone with respect. Harassment, trolling, or personal attacks will not be tolerated in any issue, pull request, or discussion.

## How to Contribute

1. **Fork** the repository on GitHub.
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/fed-badge.git
   cd fed-badge
   ```
3. **Create a feature branch** — never work directly on `main`:
   ```bash
   git checkout -b feat/my-awesome-feature
   ```
4. **Make your changes.** The entire tool lives in `index.html` and `styles.css`, so most edits are self‑contained. Keep the code clean and well‑commented.
5. **Test locally** by opening `index.html` in your browser. Verify the Generator, Presets, ASCII Studio, and Docs tabs all work.
6. **Commit** with a clear, descriptive message:
   ```bash
   git commit -m "feat: add gradient color support to Raw SVG badges"
   ```
7. **Push** to your fork:
   ```bash
   git push origin feat/my-awesome-feature
   ```
8. **Open a Pull Request** against the `main` branch of [`FED-OS/FED-Badge`](https://github.com/FED-OS) and fill out the PR template.

## Branch Naming

| Type | Prefix | Example |
| :--- | :--- | :--- |
| New feature | `feat/` | `feat/ascii-export` |
| Bug fix | `fix/` | `fix/copy-clipboard-safari` |
| Docs | `docs/` | `docs/update-readme` |
| Chore | `chore/` | `chore/cleanup-gitignore` |

## Commit Message Format

We loosely follow [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): short description

optional longer body
```

Common types: `feat`, `fix`, `docs`, `style`, `refactor`, `chore`.

## Reporting Bugs

Open a [GitHub Issue](https://github.com/FED-OS) and include:

- A clear title and description of the bug.
- Steps to reproduce.
- Expected vs. actual behavior.
- Your browser and operating system.
- Screenshots if applicable.

## Suggesting Features

Have an idea? Start a conversation in [GitHub Discussions](https://www.fedpromptly.com/forum) or open an issue tagged **enhancement**. We love hearing how you'd use the tool.

## Areas We'd Love Help With

- New preset badges for popular services.
- Additional ASCII animation styles (matrix, snowfall, etc.).
- Accessibility improvements (keyboard navigation, ARIA labels).
- Browser compatibility testing across Firefox, Safari, and Edge.
- Translations of the documentation.

## Questions?

Reach us through:

- **Forum:** [fedpromptly.com/forum](https://www.fedpromptly.com/forum)
- **GitHub Org:** [FED-OS](https://github.com/FED-OS)
- **Discussions:** Use the Discussions tab on the repository.

Thank you for helping make FED‑Badge better for everyone! ⚡
