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

### EuroDocBench

**Can your document AI read a European invoice?**

```bash
eurodocbench-score --gold gold/test.jsonl --pred predictions.jsonl
```

A synthetic, exactly labelled benchmark for extracting 12 key fields from
invoices in 12 European locales and five layouts, with a born-digital text
track and a simulated-scan track. A zero-shot small LLM finds names and
identifiers reliably but gets only about half of the amounts right — the
European number formats, dates and VAT breakdowns are where it fails.

**[Repository](https://github.com/sinceaihq/eurodocbench)** ·
**[Dataset](https://huggingface.co/datasets/sinceaihq/eurodocbench)** ·
**[Results](https://huggingface.co/spaces/sinceaihq/eurodocbench-results)** ·
**[Report](https://github.com/sinceaihq/eurodocbench/blob/main/docs/REPORT.md)**

---

### EuroPII Guard

**Find and redact European personal data before text leaves your organisation.**

```bash
echo "Henkilötunnus 150685A123D, IBAN DE89 3704 0044 0532 0130 00" | europii redact
```

Checksum-validated detection of national identity numbers from 22 European
countries, EU VAT numbers, IBANs, payment cards, phone numbers and e-mail
addresses. Pure Python, runs offline or in the browser, plugs into Presidio.
A privacy-assistance tool, not a compliance guarantee.

**[Repository](https://github.com/sinceaihq/europii-guard)** ·
**[Demo](https://huggingface.co/spaces/sinceaihq/europii-guard-demo)** ·
**[Benchmark](https://huggingface.co/datasets/sinceaihq/europii-bench)** ·
**[Report](https://github.com/sinceaihq/europii-guard/blob/main/docs/REPORT.md)**

---

### SafePrompt

**Check what you paste into AI chat for personal data and secrets — locally.**

A Chromium extension that checks text when you paste it into ChatGPT or Gemini
(Claude opt-in), finds European national ID numbers (checksum-validated, 22
countries), EU VAT numbers, IBANs, contact details and API keys, and gives you
a sanitized version with placeholders you can restore in the answer. Nothing
leaves your browser, and it never sends anything for you.

**[Repository](https://github.com/sinceaihq/safeprompt)** ·
**[Download](https://github.com/sinceaihq/safeprompt/releases/latest)** ·
**[Demo](https://huggingface.co/spaces/sinceaihq/safeprompt-demo)** ·
**[Benchmark](https://huggingface.co/datasets/sinceaihq/safeprompt-bench)**

---

### DocToSheet

**Invoices and receipts to a spreadsheet, on your own computer — every value traceable.**

```bash
doctosheet extract invoice.pdf -o invoices.xlsx
```

Reads European e-invoices exactly (Factur-X / ZUGFeRD, XRechnung, Peppol,
Finvoice), PDFs and scans, shows where on the page each value came from, and
never exports a computed amount as if it were printed. Evaluated on invoices
from producers never seen during development.

**[Repository](https://github.com/sinceaihq/doctosheet)** ·
**[Demo](https://huggingface.co/spaces/sinceaihq/doctosheet-demo)** ·
**[Evaluation](https://github.com/sinceaihq/doctosheet/blob/main/docs/EVALUATION.md)**

---

### GroundClaim

**Your agent says the tests pass. GroundClaim checks.**

```bash
groundclaim check --base main --trace run.jsonl --message-file message.md
```

Checks AI agents' completion claims — tests pass, committed, pushed, PR
opened, deployed — against git, run traces, test reports and CI, with verdicts
that say how strong the evidence is. Includes a GitHub Action for pull
requests and a benchmark that measures how often a checker confirms a false
claim.

**[Repository](https://github.com/sinceaihq/groundclaim)** ·
**[Benchmark](https://huggingface.co/datasets/sinceaihq/groundclaim-bench)** ·
**[Report viewer](https://huggingface.co/spaces/sinceaihq/groundclaim-viewer)** ·
**[Report](https://github.com/sinceaihq/groundclaim/blob/main/docs/BENCHMARK.md)**

---

Get in touch: **builders@sinceai.fi**
