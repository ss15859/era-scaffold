# era-scaffold

Frozen scaffold (utils / plotting / baseline loading) for the **lite** ERA
causal candidate notebook (`era_candidate_causal_lite.ipynb`).

**Generated code — do not edit here.** The source of truth is
`notebooks/era_candidate_causal.ipynb` in the (private) `automl-csep-eval`
repo; `scripts/build_era_lite.py` regenerates `era_scaffold/` and the lite
notebook together. The notebook clones this repo at a **pinned commit** and
does `sys.path.insert(0, <clone dir>)`, then:

```python
from era_scaffold import (query_comcat_chunked, build_daily_csep_series,
                          evaluate_fn, load_baselines)
etas_scores_wrt_obs = load_baselines()   # cwd must be the reproducibility repo
```
