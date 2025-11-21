# care_reproduce
trying to run the care code (https://github.com/peymanrasouli/CARE)

Adjusted the library versions in requirements (NumPy, SciPy, scikit-learn, hdbscan) to ensure the project runs on Windows with python 3.7.

results of reproduce.py
====================================================================================================
RESULTS (Table 7 Format)
====================================================================================================
Config          ↓O_outcome      ↓O_distance     ↓O_sparsity     ↑O_proximity    ↑O_connectedness ↓O_coherency    ↓O_actionability
----------------------------------------------------------------------------------------------------
{1}             0.00±0.0  0.02±0.0  1.44±0.8  0.70±0.5  0.18±0.4  0.05±0.2  0.08±0.3
{1,2}           0.00±0.0  0.12±0.1  2.80±1.5  1.00±0.0  1.00±0.0  0.10±0.3  0.28±0.5
{1,2,3}         0.00±0.0  0.12±0.1  3.00±1.6  1.00±0.0  1.00±0.0  0.00±0.0  0.42±0.6
{1,2,3,4}       0.00±0.0  0.11±0.1  2.70±1.6  1.00±0.0  0.92±0.3  0.00±0.0  0.00±0.0
====================================================================================================

================================================================================
ASSERTIONS
================================================================================

Config {1}:
  ✓ outcome        : 0.000 (expected 0.00, diff 0.000)
  ✓ distance       : 0.020 (expected 0.02, diff 0.000)
  ✓ sparsity       : 1.440 (expected 1.41, diff 0.030)
  ✗ proximity      : 0.700 (expected 0.58, diff 0.120)
  ✓ connectedness  : 0.180 (expected 0.20, diff 0.020)
  ✓ coherency      : 0.049 (expected 0.05, diff 0.001)
  ✓ actionability  : 0.080 (expected 0.08, diff 0.000)

Config {1,2}:
  ✓ outcome        : 0.000 (expected 0.00, diff 0.000)
  ✓ distance       : 0.120 (expected 0.12, diff 0.000)
  ✓ sparsity       : 2.800 (expected 2.84, diff 0.040)
  ✓ proximity      : 1.000 (expected 1.00, diff 0.000)
  ✓ connectedness  : 1.000 (expected 1.00, diff 0.000)
  ✓ coherency      : 0.102 (expected 0.10, diff 0.002)
  ✗ actionability  : 0.280 (expected 0.36, diff 0.080)

Config {1,2,3}:
  ✓ outcome        : 0.000 (expected 0.00, diff 0.000)
  ✓ distance       : 0.119 (expected 0.12, diff 0.001)
  ✓ sparsity       : 3.000 (expected 3.05, diff 0.050)
  ✓ proximity      : 1.000 (expected 1.00, diff 0.000)
  ✓ connectedness  : 1.000 (expected 1.00, diff 0.000)
  ✓ coherency      : 0.000 (expected 0.00, diff 0.000)
  ✗ actionability  : 0.420 (expected 0.35, diff 0.070)

Config {1,2,3,4}:
  ✓ outcome        : 0.000 (expected 0.00, diff 0.000)
  ✓ distance       : 0.111 (expected 0.11, diff 0.001)
  ✓ sparsity       : 2.700 (expected 2.76, diff 0.060)
  ✓ proximity      : 1.000 (expected 1.00, diff 0.000)
  ✓ connectedness  : 0.920 (expected 0.91, diff 0.010)
  ✓ coherency      : 0.000 (expected 0.00, diff 0.000)
  ✓ actionability  : 0.000 (expected 0.00, diff 0.000)

================================================================================
✗ SOME ASSERTIONS FAILED
================================================================================
