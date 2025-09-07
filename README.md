# Custom GPT JSONs

A focused library of opinionated JSON configs for custom GPTs that enforce style, audit messaging, accelerate drafting, and tighten content operations.

## What’s included

These files are ready to paste into the ChatGPT GPT editor and adapt to your use case.

| File | What it does |
| --- | --- |
| `18F Style Guide GPT.JSON` | Enforces the 18F style guide across drafts. |
| `Content Shrinker GPT.json` | Compresses content while preserving substance and intent. |
| `Content-Theater-Detector.json` | Flags “content theater” and demands evidence or sources. |
| `Contrarian_Tech_Analyst-v2.json` | Produces contrarian, defensible analysis to pressure-test narratives. |
| `Death by Gen Z Messaging.json` | Scores immaturity/“Gen Z” risk and prescribes remediation. |
| `IT-Website-Messaging-Auditor.json` | Audits IT/enterprise website copy against buyer expectations. |
| `LinkedIn-Summary-Builder.json` | Drafts sharp, outcome-oriented LinkedIn summaries. |
| `NotionPolicyWriterGPT.json` | Drafts policies/procedures structured for a Notion wiki. |
| `Ops_Cover_Letter_Writer.JSON` | Generates operations-savvy cover letters tied to outcomes. |
| `Outcome-Based Resume Editor.JSON` and `outcome-resume-editor.json` | Reframes resumes to measurable outcomes and impact. |
| `resume-pmm-conversion.json` | Adapts resumes toward product marketing manager roles. |
| `Partner Case Study Assistant.json` and `Partner_Case_Study_Assistant.json` | Builds customer/partner case studies with credible proof. |
| `ChatGPT_Prompt_Drafting_Checklist.csv` | A quick checklist to raise prompt quality and consistency. |
| `custom_gpt_governance_playbook.pptx` | Slides covering governance guardrails for custom GPTs. |

## Quick start

1) Open the GPT editor  
Go to ChatGPT → **Explore GPTs** → **Create** → open the **Configure** tab.

2) Load a JSON config  
Open a file from this repo, copy its JSON, and paste it into the **Instructions** (and related fields if the config is split by sections). If your editor supports importing from file, you can import the JSON instead.

3) Enable the right capabilities  
In **Configure**, turn on Web browsing, Code Interpreter/Data, or Image generation only if the config calls for them. Keep tools minimal unless the JSON specifies otherwise.

4) Publish and iterate  
Use the included checklist CSV to tighten your instructions, then publish privately, test on real content, and refine.

## Usage patterns

- Use auditors before writers  
  Run an auditor JSON (e.g., messaging or style) to surface gaps, then feed those findings into a writer/rewriter JSON.

- Chain for quality  
  Typical chain: Lint/score → Rewrite → Validate → Final format. Keep the chain short and measurable.

- Demand receipts  
  Any config that makes claims should also require citations, examples, or links. Bake this into the instructions.

## Conventions and tips

- Keep instructions assertive and unambiguous  
  Say what to do and what to avoid. Ban vague marketing filler and require examples.

- Minimize tools and knowledge files  
  Only enable what’s essential. Remove anything the model tends to misuse.

- Validate JSON before use  
  If you edit configs, validate with a JSON linter to avoid silent failures.

## Roadmap

- Consolidate duplicates and version configs with clear change notes.  
- Add A/B rubrics for rewrite vs. consultative modes across multiple configs.  
- Ship a minimal test harness that runs a standard prompt suite against each JSON.  
- Introduce schema fragments for reusable guardrails (tone, evidence, bias checks).

## Contributing

Open an issue describing the use case and the measurable outcome you want. PRs should include:
- The JSON config  
- A short rationale  
- A three-prompt test script and expected behaviors

## License

CC0-1.0. See `LICENSE`.

## Credits

Maintained by Will Kelly. Built for working writers, editors, and operators who need consistent outputs and less hand-holding.
```

[1]: https://github.com/will-kelly/Custom-GPT-JSONs "GitHub - will-kelly/Custom-GPT-JSONs"
[2]: https://help.openai.com/en/articles/8554397-creating-a-gpt?utm_source=chatgpt.com "Creating a GPT"
