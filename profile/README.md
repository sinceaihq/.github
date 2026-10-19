## Since AI

Global execution-focused AI innovation ecosystem — [sinceai.ai](https://sinceai.ai)

---

### AI Shipcheck

**Your AI says it's done. Shipcheck tells you if it's ready to ship.**

```bash
npx ai-shipcheck .
```

An evidence-backed production-readiness scanner for JavaScript and TypeScript
projects. It reads your code locally and reports what would bite you in
production — missing row-level security, routes that write without an
authorisation check, secrets bundled into the browser, LLM endpoints with no
rate limit — each with a file, a line, and a rule you can look up.

No signup. No API key. Nothing is uploaded, and nothing in the scanned
repository is ever executed.

**[Repository](https://github.com/sinceaihq/ai-shipcheck)** ·
**[npm](https://www.npmjs.com/package/ai-shipcheck)** ·
**[Rules](https://github.com/sinceaihq/ai-shipcheck/blob/main/docs/rules/README.md)** ·
**[Good first issues](https://github.com/sinceaihq/ai-shipcheck/issues?q=is%3Aopen+label%3A%22good+first+issue%22)**

Contributions are welcome — especially reports of a rule firing on correct
code, which are treated as the most serious class of bug in that project.

---

### EuroTender

**CPV codes for European public tenders, in any EU language, on a CPU.**

```python
from eurotender import predict_cpv
predict_cpv("Development and maintenance of municipal IT systems")
```

A multilingual classifier that suggests Common Procurement Vocabulary codes
for tender notices, trained on 510k TED notices and evaluated on 234k notices
published after the training period (82 % top-1, 94 % top-5 for the CPV
division, 22 languages). The model, the leakage-controlled dataset and a demo
that runs entirely in the browser are on Hugging Face.

**[Repository](https://github.com/sinceaihq/eurotender)** ·
**[Model](https://huggingface.co/sinceaihq/eurotender-cpv-baseline)** ·
**[Dataset](https://huggingface.co/datasets/sinceaihq/eurotender-cpv)** ·
**[Demo](https://huggingface.co/spaces/sinceaihq/eurotender-cpv-demo)** ·
**[Report](https://github.com/sinceaihq/eurotender/blob/main/docs/REPORT.md)**

---

Get in touch: **builders@sinceai.fi**
