# Report figures rendered from project artifacts

All figures are available as 300-dpi PNG, PDF, and SVG files.

| Figure | Suggested report use | Source basis |
|---|---|---|
| fig_01_implemented_ctmri_architecture | Chapter 4 system architecture | `src/fusion_model_3d.py`, `scripts/train_fusion_3d_unified.py` |
| fig_02_reproducible_ctmri_workflow | Chapter 4 methodology or Chapter 5 implementation status | Training, inference, and benchmark scripts |
| fig_03_dataset_and_evaluation_design | Chapter 4 dataset design or Appendix C | Local audit and benchmark split |
| fig_04_reconstruction_benchmark | Chapter 5 results or expected outcomes update | `outputs/benchmarks/fusion_ctmri/benchmark_summary.json` |
| fig_05_training_dynamics | Chapter 5 training results | Phase 2 and Phase 3 checkpoints |
| fig_06_visual_evidence_contact_sheet | Appendix G visual proofs | Saved training and inference proof images |

Captions must describe these as reconstruction, fusion, inference, or explainability evidence. They must not be called tumour-classification accuracy figures.
