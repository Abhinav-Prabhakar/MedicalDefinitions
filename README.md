<div align="center">
  <img src="assets/og.png" alt="one·liners — Medicine, in one line." width="100%" />
</div>

<div align="center">

# one·liners · Medical Terminology

**Medicine, in one line.**

A quiet medical dictionary you can practise: 327 definitions across 6 subjects — word parts, body systems, clinical abbreviations, documentation, diagnostics and pharmacology basics — with an adaptive two-way quiz and a memory of what you actually know.

<a href="https://abhinav-prabhakar.github.io/MedicalDefinitions/">
  <img src="https://img.shields.io/badge/OPEN%20THE%20APP-live-2364aa?style=for-the-badge&logo=githubpages&logoColor=white" alt="Open the live app" />
</a>

<br /><br />

<img src="https://img.shields.io/badge/definitions-327-2364aa?style=flat-square" alt="327 definitions" />
<img src="https://img.shields.io/badge/subjects-6-0a0f18?style=flat-square" alt="6 subjects" />
<img src="https://img.shields.io/badge/PWA-offline--ready-0a0f18?style=flat-square&logo=pwa&logoColor=white" alt="PWA offline ready" />
<img src="https://img.shields.io/badge/backend-none-d23f45?style=flat-square" alt="No backend" />
<img src="https://img.shields.io/badge/vanilla-HTML%20%C2%B7%20CSS%20%C2%B7%20JS-11877f?style=flat-square" alt="Vanilla HTML CSS JS" />
<img src="https://img.shields.io/badge/deploy-GitHub%20Pages-0a0f18?style=flat-square&logo=github&logoColor=white" alt="GitHub Pages" />

</div>

<p align="center"><sub>Screenshots use sample study data. The app itself starts clean, on your device.</sub></p>

---

## Why this exists

Medical language is built from parts: *cardi-*, *-itis*, *-ectomy*. Learn the parts and the abbreviations, and a chart stops looking like a cipher. **one·liners** gives every term one line, quizzes it both ways, and brings back the ones you keep confusing — *hyper-* and *hypo-* included.

A clinical serif for terms, a clean sans for everything else, and an ECG trace that never stops. Each subject carries one colour, used in small doses. No accounts, no server, no noise.

> **Recognition is not recall.** Recognising *hematocrit* on a lab sheet is not the same as naming it from its meaning. So the quiz asks both ways.

---

## Screenshots

<table>
  <tr>
    <td width="50%">
      <img src="assets/screenshot-home-light.png" alt="Home in light mode" width="100%" />
      <p align="center"><sub><strong>Light by default</strong> · today, activity, subject mastery</sub></p>
    </td>
    <td width="50%">
      <img src="assets/screenshot-home-dark.png" alt="Home in dark mode" width="100%" />
      <p align="center"><sub><strong>Dark when you choose it</strong> · remembered across visits</sub></p>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="58%">
      <img src="assets/screenshot-subject-light.png" alt="A subject's definitions with per-definition mastery" width="100%" />
      <p align="center"><sub><strong>Every definition has a memory.</strong> Hover a row for its mastery and source.</sub></p>
    </td>
    <td width="42%">
      <img src="assets/screenshot-quiz-dark.png" alt="A two-way quiz in dark mode" width="100%" />
      <p align="center"><sub><strong>Answers explain themselves.</strong> The definition, and what you picked.</sub></p>
    </td>
  </tr>
</table>

<div align="center">
  <img src="assets/screenshot-mobile-subject.png" alt="one·liners on a phone" width="310" />
  <p><sub><strong>320 → 1440px.</strong> The same quiet interface, not a crushed desktop.</sub></p>
</div>

---

## What's inside

**327 one-liners** across **6 subjects**, written for pre-health undergraduates and nursing students.

- **Core** — Word Parts, Body Systems, Clinical Abbreviations, Documentation, Diagnostics, Pharmacology Basics

| Subject | Definitions | Units |
| --- | ---: | --- |
| **Word Parts** | 48 | Prefixes · Roots · Suffixes · Combining forms |
| **Body Systems** | 60 | Integumentary · Skeletal and muscular · Cardiovascular · Respiratory · Nervous · Digestive, urinary, and endocrine |
| **Clinical Abbreviations** | 50 | Vital signs and measurements · Diagnoses and conditions · Procedures and tests · Medications and routes · Departments and roles · Time and frequency |
| **Documentation** | 50 | Medical records · SOAP and progress notes · Orders and prescriptions · Consent and legal · Coding and billing basics |
| **Diagnostics** | 69 | Laboratory values · Imaging modalities · Physical exam terms · Diagnostic procedures · Pathology and cytology |
| **Pharmacology Basics** | 50 | Pharmacokinetics · Pharmacodynamics · Drug classes · Routes and formulations · Adverse effects and interactions |

Every definition is one sentence, 8–28 words, and carries a source locator. Hover a
definition's mastery rail to see where it came from. Coverage, gaps and assumptions are
documented in [`data/README.md`](data/README.md).

---

## Two directions of recall

Every round mixes both question types, balanced 5/5. You cannot coast on recognition.

| Prompt | You choose | What it trains |
| --- | --- | --- |
| `-ectomy` | one of four definitions | term → meaning |
| “Percentage of blood volume made up of red blood cells.” | one of four terms | meaning → term |

- **The term is never in the question.** When a definition has to mention its own term, the
  quiz blanks it out, so meaning → term tests meaning.
- **Wrong answers that look right.** Distractors come from each definition's curated
  look-alikes, then from similar wording in the same unit — never four random strangers.
- **Adaptive sampling.** The three weakest definitions are guaranteed a slot; the rest are
  weighted toward low mastery.
- **Keyboard complete.** <kbd>1</kbd>–<kbd>4</kbd> or <kbd>A</kbd>–<kbd>D</kbd> to choose,
  <kbd>Enter</kbd> for next, <kbd>Esc</kbd> to leave, <kbd>r</kbd> to repeat a round.

---

## A memory you can see

Mastery is one confidence score per definition, stored locally: **+30%** for a correct answer,
**−40%** for a miss. Four clean answers reach 100%.

| After | Score | Reads as |
| --- | --- | --- |
| no attempts | 0% | `new` |
| 1 correct | 30% | `learning` |
| 2 correct | 60% | `familiar` |
| 3 correct | 90% | `solid` |
| a miss | −40% | re-learn |

The subject page shows a 2px bar on every definition; cards show a bar profile of the whole
subject; the home page has a daily goal stack and a quiet, monochrome activity trail.

---

## Offline, installable, private

- **Full PWA** — manifest, service worker, maskable icons. Works offline after the first load.
  Install from the browser's own menu (Chrome: the install icon in the address bar; iOS Safari:
  **Share → Add to Home Screen**; macOS Safari: **File → Add to Dock**).
- **No accounts, no analytics, no server.** Progress lives in `localStorage` under
  `oneliners.medical-terminology.*` and never leaves the device.
- **Self-hosted type** — Source Sans 3, Source Serif 4. No external font requests.
- **Light by default**, dark when you choose it, remembered before first paint.

---

## Sources

| Source | Publisher | License |
| --- | --- | --- |
| [Medical Terminology 2e](https://wtcs.pressbooks.pub/medterm/) | WisTech Open (Wisconsin Technical College System) | CC BY 4.0 |
| [Anatomy and Physiology 2e](https://openstax.org/books/anatomy-and-physiology-2e) | OpenStax (Rice University) | CC BY-NC-SA 4.0 |
| [MedlinePlus Medical Dictionary: Common Abbreviations](https://medlineplus.gov/) | National Library of Medicine (MedlinePlus) | Public domain (US government) |
| [CDC Infection Control Abbreviations](https://www.cdc.gov/) | Centers for Disease Control and Prevention | Public domain (US government) |
| [Joint Commission Do Not Use Abbreviations List](https://www.jointcommission.org/) | The Joint Commission | unknown |
| [ISMP List of Error-Prone Abbreviations](https://www.ismp.org/) | Institute for Safe Medication Practices | unknown |
| [CMS Evaluation and Management Medical Record Documentation](https://www.cms.gov/training-education/medicare-learning-networkr-mln/compliance/medicare-provider-compliance-tips/evaluation-management-services) | Centers for Medicare & Medicaid Services | Public domain (US government) |
| [CMS Medical Record Maintenance and Access Requirements](https://www.cms.gov/files/document/mln4840534-medical-record-maintenance-access-requirements.pdf) | Centers for Medicare & Medicaid Services | Public domain (US government) |
| [Fundamentals of the Legal Health Record and Designated Record Set](https://journal.ahima.org/) | AHIMA | unknown |
| [Best Practices in Medical Record Documentation and Completion](https://journal.ahima.org/) | AHIMA | unknown |
| [Personal Health Records](https://medlineplus.gov/personalhealthrecords.html) | National Library of Medicine (MedlinePlus) | Public domain (US government) |
| [MedlinePlus Medical Tests](https://medlineplus.gov/lab-tests) | National Library of Medicine (MedlinePlus) | Public domain (US government) |
| [MedlinePlus Diagnostic Imaging](https://medlineplus.gov/diagnosticimaging.html) | National Library of Medicine (MedlinePlus) | Public domain (US government) |
| [MedlinePlus Medical Encyclopedia](https://medlineplus.gov/encyclopedia.html) | National Library of Medicine (MedlinePlus) | Public domain (US government) |
| [NCI Dictionary of Cancer Terms](https://www.cancer.gov/publications/dictionaries/cancer-terms) | National Cancer Institute | Public domain (US government) |
| [Drugs@FDA Glossary of Terms](https://www.fda.gov/drugs/drug-approvals-and-databases/drugsfda-glossary-terms) | U.S. Food and Drug Administration | Public domain (US government) |
| [MedlinePlus Drug Therapy](https://medlineplus.gov/drugtherapy.html) | National Library of Medicine (MedlinePlus) | Public domain (US government) |
| [Pharmacology for Nurses](https://openstax.org/books/pharmacology/pages/1-key-terms) | OpenStax (Rice University) | CC BY 4.0 |

Definitions are paraphrased one-liners, not excerpts. Raw source material is not redistributed.

> [!IMPORTANT]
> Educational vocabulary only; not medical advice.

---

## Run it locally

```bash
# A server is required: the app fetches its data.
python3 -m http.server 8000
# → http://localhost:8000/
```

No build step, no dependencies. `index.html` is the whole app.

```text
.
├── index.html             # the entire app
├── manifest.webmanifest   # PWA manifest
├── sw.js                  # offline app shell + data cache
├── data/
│   ├── curriculum.json    # sections and subjects the app loads
│   ├── sources.json       # where every definition comes from
│   ├── collection.json    # scope, audience, assumptions
│   ├── README.md          # coverage report
│   └── subjects/*.json    # one file per subject
└── assets/                # icons, social card, screenshots, fonts
```

---

## The one·liners family

Same instrument, different vocabularies. Each has its own look, data and progress.

| Collection | Repository |
| --- | --- |
| [Electronics, in one line.](https://abhinav-prabhakar.github.io/ECEDefinitions/) | [`Abhinav-Prabhakar/ECEDefinitions`](https://github.com/Abhinav-Prabhakar/ECEDefinitions) |
| [Anatomy and physiology, in one line.](https://abhinav-prabhakar.github.io/AnatomyDefinitions/) | [`Abhinav-Prabhakar/AnatomyDefinitions`](https://github.com/Abhinav-Prabhakar/AnatomyDefinitions) |
| [Electricity, in one line.](https://abhinav-prabhakar.github.io/NECDefinitions/) | [`Abhinav-Prabhakar/NECDefinitions`](https://github.com/Abhinav-Prabhakar/NECDefinitions) |
| [HVAC, in one line.](https://abhinav-prabhakar.github.io/HVACDefinitions/) | [`Abhinav-Prabhakar/HVACDefinitions`](https://github.com/Abhinav-Prabhakar/HVACDefinitions) |
| **[Medicine, in one line.](https://abhinav-prabhakar.github.io/MedicalDefinitions/)** | [`Abhinav-Prabhakar/MedicalDefinitions`](https://github.com/Abhinav-Prabhakar/MedicalDefinitions) |
| [Nursing, in one line.](https://abhinav-prabhakar.github.io/NursingDefinitions/) | [`Abhinav-Prabhakar/NursingDefinitions`](https://github.com/Abhinav-Prabhakar/NursingDefinitions) |
| [Pharmacology, in one line.](https://abhinav-prabhakar.github.io/PharmacologyDefinitions/) | [`Abhinav-Prabhakar/PharmacologyDefinitions`](https://github.com/Abhinav-Prabhakar/PharmacologyDefinitions) |
| [Plumbing, in one line.](https://abhinav-prabhakar.github.io/PlumbingDefinitions/) | [`Abhinav-Prabhakar/PlumbingDefinitions`](https://github.com/Abhinav-Prabhakar/PlumbingDefinitions) |
| [Software, in one line.](https://abhinav-prabhakar.github.io/SoftwareDefinitions/) | [`Abhinav-Prabhakar/SoftwareDefinitions`](https://github.com/Abhinav-Prabhakar/SoftwareDefinitions) |
| [The law, in one line.](https://abhinav-prabhakar.github.io/LegalDefinitions/) | [`Abhinav-Prabhakar/LegalDefinitions`](https://github.com/Abhinav-Prabhakar/LegalDefinitions) |

### Credits

Definitions are paraphrased from the openly licensed medical references listed above. Built on the [one·liners](https://github.com/Abhinav-Prabhakar/ECEDefinitions) engine. Fonts: Source Sans 3, Source Serif 4 (SIL Open Font License 1.1).

<div align="center">
  <sub>If this helps you read your first chart, star the repo. It keeps the dictionary growing.</sub>
</div>
