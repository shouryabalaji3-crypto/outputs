# CT+MRI Benchmark Limitations

Generated: 2026-09-17T21:33:08.127539+00:00

## What was measured

The frozen Phase 3 checkpoint was evaluated for CT reconstruction from paired CT+MRI inputs. Metrics are computed after normalization to [0, 1]: normalized MAE, MSE, RMSE, PSNR, a Gaussian-window 3D SSIM approximation, and normalized cross-correlation.

## What was not measured

No tumour accuracy, AUROC, F1, sensitivity, specificity, or diagnosis was measured. The checkpoint was trained self-supervised on paired scans without verified tumour labels.

## Dataset separation

- Zenodo held-out test: same preprocessing family as training, 3 subjects.
- IBSR external DICOM: external domain-shift probe. It is not pooled with the Zenodo benchmark.

## Registration warning

The current DICOM track converts each selected series and independently resizes CT and MRI to 128 x 128 x 128. It does not perform rigid registration. Therefore external IBSR metric values are engineering diagnostics, not clinically meaningful image-registration or generalization claims.

## Series selection

The DICOM runner records the selected CT and MRI series and the selection keyword in each case JSON. Review these records before using any result in a report.
