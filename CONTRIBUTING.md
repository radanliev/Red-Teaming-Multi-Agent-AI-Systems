# Contributing

Thanks for contributing to the Red-Teaming Multi-Agent AI Systems course repository.

## How to contribute
1. Fork the repository and create a branch for your change:
```bash
git checkout -b feature/your-feature
	2.	Make changes and add tests or verification notes where appropriate.
	3.	Commit with a clear message:
git commit -m "Add Session 2 demo script: prompt injection lab"
	4.	Push to your fork and open a Pull Request.
File conventions
	•	Keep markdown simple and accessible.
	•	Put session demos in SESSIONS/.
	•	Put interactive/slido assets in SLIDO/.
	•	Add resources and citations inline where necessary.

Licence

Contributions are made under the same licence as the repository (MIT by default). If you need a different licence for third-party content, include a NOTICE.md.
---

### Instructions to add files to the repo
If you want me to, I can produce a ready-to-apply patch or a `git` command sequence. For manual updates, use:

```bash
# inside repo root
mkdir -p SESSIONS SLIDO
# create files with your editor and paste content from above
git add README.md SESSIONS/*.md SLIDO/slido_questions.csv CONTRIBUTING.md
git commit -m "Add browser-based demo guides, Slido questions and contributing guide"
git push origin main
