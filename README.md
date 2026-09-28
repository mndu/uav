# Universal Activation Verbalizer — EMNLP 2026 project website

Static project page for **Universal Activation Verbalizer: A Unified Framework for Cross-Model Activation Explanation**. It follows the visual style of the SAEExplainer and Rep2Text pages, with no top navigation or conference badge.

## Preview

From this directory, run `python3 -m http.server 8002` and open http://localhost:8002. No build step or package installation is required.

## Files

- `index.html`: authors, abstract, method, results, examples, and citation.
- `style.css`: shared visual style from the SAEExplainer website.
- `paper.css`: paper-specific responsive layout adjustments.
- `script.js`: BibTeX copying and manual-selection fallback.
- `assets/`: Figures 1 and 3 cropped from the supplied PDF, plus a favicon.
- `1341_Universal_Activation_Verb.pdf`: supplied paper, unchanged.

## Publication

Website: https://mndu.github.io/uav/

Repository: https://github.com/mndu/uav

GitHub Pages deploys `main` from `/ (root)`. The website and supplied PDF are published with the author's permission.

Research code: https://github.com/hy-zhao23/ActExp

arXiv: https://arxiv.org/abs/2605.25903

## Content provenance

The supplied PDF is the source for all authors, affiliations, figures, abstract, quantitative values, and selected qualitative examples. EMNLP 2026 acceptance is provided by the author. Bibliography details that are not yet confirmed (page numbers, ACL Anthology URL, and DOI) are omitted.

- Table 3 provides all four cross-donor result rows.
- Table 2 provides selected trained baselines and UAV settings, using overall mean scores. The page explicitly points to the full paper for task-specific results, training-free baselines, and uncertainty.
- Figure 3 provides the adapter/LoRA ablation and its fact-retrieval BERTScore values (0.196 and 0.402).
- Appendix D.1 and Table 12 provide training costs and validation losses.
- Table 19 provides the successful Westfield Group example and the incorrect Osaka district example. Source excerpts are context for the reader and are not claimed to be input to the verbalizer at evaluation time.
- Decoder reuse is described precisely: adapters remain donor- and layer-specific, and adapter-only transfer freezes the already-trained decoder-side LoRA.

No third-party template code was copied. The existing family of project pages originally drew visual inspiration from Ctrl-X and DisCoScene.
