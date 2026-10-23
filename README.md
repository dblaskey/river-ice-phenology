This archive provides Python/Jupyter code supporting a comparative evaluation of regional river-ice models across Alaska and the Yukon River basin. 
The workflow evaluates daily ice presence and the timing of spring break-up and autumn freeze-up using spatial, temporal, and spatiotemporal holdouts.

The models include a multivariate random forest, temperature-only and feature-ablation random forests, a locally refitted seasonal temperature logistic regression, and a deterministic 30-day 0 °C isotherm benchmark. 
Daily ice-state evaluation includes accuracy, Brier score, ROC-AUC, and probabilistic-model log loss. 
Event-date evaluation includes mean absolute error, root mean square error, signed bias, and paired river-segment bootstrap confidence intervals using common complete-case cohorts.

A fixed-training spatiotemporal hindcast supports site-level trend evaluation using observation-matched annual records, Sen slopes, Mann–Kendall tests, and Benjamini–Hochberg false-discovery-rate adjustment. 
The workflow also assesses sensitivity to the minimum number of annual observations required for trend estimation.

The publication notebook supports two execution modes: regeneration of tables and figures from archived predictions, and model refitting from the required input data. 
It exports analysis results, selected hyperparameters, random seeds, software versions, and input-file hashes. Instructions and input requirements are documented within the notebook.

The temperature logistic regression and isotherm implementations are adapted benchmarks evaluated against this study’s observation definitions and validation design; they are not exact reproductions of all aspects of the original published applications. 
The study evaluates historical predictive performance and trend agreement, rather than directly validating future climate projections.
