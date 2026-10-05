# Project W1 Charter
## User
A petroleum geoscience student or early-career geoscientist who works with well logs and needs a quick first impression of the rock types. Managers and other stakeholders are secondary users who may review the outputs.

## Decision supported
Which sections of the well are most likely shale, sandstone, or other lithologies, and which intervals should I re-examine carefully before relying on the interpretation?

## Data
FORCE 2020 open well-log dataset (Norwegian offshore). Licence and columns to be verified in Phase 2.

## Baseline
Gamma-ray cutoff (shale vs non-shale), then a small decision tree.

## Model
Random Forest, then XGBoost.

## Metric
Macro-F1 and per-class recall (accuracy alone hides rare rock types).

## Validation
Whole-well holdout (GroupKFold). No rows from a test well ever appear in training.

## Success
Beat the baseline on unseen wells, or explain honestly why not.

## Risks
Label noise, class imbalance, 2-week deadline, foreign data (not Ghanaian).

## Limits
Decision-support only. Not a certified formation evaluation.

## Timeline (Tier 1, 14 days)
Days 1-2 setup and primer · 3-4 data · 5-11 Stage A · 12-14 app and documentation.
