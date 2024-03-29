ENSO LIFECYCLE
==============
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6656800.svg)](https://doi.org/10.5281/zenodo.6656800)

Figure number: Figure 3.36
From the IPCC Working Group I Contribution to the Sixth Assessment Report: Chapter 3

![Figure 3.36](ar6_wg1_chap3_figure3_36_enso_lifecycle.png?raw=true)


Description:
------------
Life cycle of (left) El Niño and (right) La Niña events in observations (black) 
and historical simulations from CMIP5 (blue; extended with RCP4.5) and CMIP6 
(red). An event is detected when the December ENSO index value in year zero 
exceeds 0.75 times its standard deviation for 1951-2010. (a, b) Composites of 
the ENSO index (ºC). The horizontal axis represents month relative to the 
reference December (the grey vertical bar), with numbers in parentheses 
indicating relative years. Shading and lines represent 5th-95th percentiles and 
multi-model ensemble means, respectively. (c, d) Mean durations (months) of El 
Niño and La Niña events defined as number of months in individual events for 
which the ENSO index exceeds 0.5 times its December standard deviation. Each dot 
represents an ensemble member from the model indicated on the vertical axis. The 
boxes and whiskers represent multi-model ensemble mean, interquartile ranges and 
5th and 95th percentiles of CMIP5 and CMIP6. The CMIP5 and CMIP6 multi-model 
ensemble means and observational values are indicated at top right of each panel. 
The multi-model ensemble means and percentile values are evaluated after 
weighting individual members with the inverse of the ensemble size of the same 
model, so that individual models are equally weighted irrespective of their 
ensemble sizes. The ENSO index is defined as the SST anomaly averaged over the 
Niño 3.4 region (5ºS-5ºN, 170ºW-120ºW). All results are based on 5-month running 
mean SST anomalies with triangular-weights after linear detrending. 


Author list:
------------
- Kosaka, Y.: University of Tokyo, Japan; ykosaka@atmos.rcast.u-tokyo.ac.jp
- McGregor, S.: Monash University, Australia
- Cassou, C.: CNRS-Cerfacs, France
- Kazeroni, R.: DLR, Germany


ESMValTool Branch:
------------------
- ESMValTool-AR6-OriginalCode-FinalFigures: [ar6_chapter_3](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/tree/ar6_chapter_3)


ESMValCore Branch:
------------------
- ESMValCore-AR6-OriginalCode-FinalFigures: [fix_cmip6_models_newcore](https://github.com/ipcc-wgi/ESMValCore-AR6-OriginalCode-FinalFigures/tree/fix_cmip6_models_newcore)


Recipe & diagnostics:
---------------------
Recipe used: [recipes/ipccwg1ar6ch3/recipe_ar6ch3_enso_cmip5+6.yml](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/recipes/ipccwg1ar6ch3/recipe_ar6ch3_enso_cmip5%2B6.yml)

Diagnostics used: 
- [diag_scripts/ar6ch3_enso/define_ensoindex.ncl](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/diag_scripts/ar6ch3_enso/define_ensoindex.ncl)
- [diag_scripts/ar6ch3_enso/draw_lifecycle.ncl](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/ar6_chapter_3/esmvaltool/diag_scripts/ar6ch3_enso/draw_lifecycle.ncl)


Expected image path:
--------------------
- recipe_ar6ch3_enso_cmip5+6_YYYYMMDD_HHMMSS/plots/enso_index/draw_enso_lifecycle/enso_lifecycle.pdf


Software description:
---------------------
- ESMValTool environment file: [IPCC_environments/ar6_newcore_remi_conda_environment.yml](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/main/IPCC_environments/ar6_newcore_remi_conda_environment.yml)
- pip file: [IPCC_environments/ar6_newcore_remi_pip_environment.txt](https://github.com/ipcc-wgi/ESMValTool-AR6-OriginalCode-FinalFigures/blob/main/IPCC_environments/ar6_newcore_remi_pip_environment.txt)


Hardware description:
---------------------
Machine used: Mistral
