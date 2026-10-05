# Project W1 Charter

## User
A junior geoscientist or student who needs a quick first-pass look at a well's lithology.

## Decision supported
Where are the likely sandstone, shale and carbonate intervals, and which intervals are too uncertain to trust without expert review?

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
