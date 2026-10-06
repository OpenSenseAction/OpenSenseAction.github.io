# Real World Usage Examples

End-to-end examples demonstrating how the OpenSense software ecosystem is applied to real-world problems, including method intercomparisons across the different packages.

## CML Processing Method Intercomparison

Intercomparison of different CML processing methods.

In the [cml_method_benchmarking repository](https://github.com/OpenSenseAction/cml_method_benchmarking) we carry out an intercomparison of processing methods for CML-based rainfall estimation. for the full OpenMRG dataset ([Andersson et al., 2022](https://doi.org/10.5194/essd-14-5411-2022)). This is currently work in progress and the same analysis will be added for the OpenRainER dataset. So far there are notebooks for:

**Rain event detection**, comparing the following methods:
- [Schleiss et al. (2010)](https://doi.org/10.1109/LGRS.2010.2043052)
- [Graf et al. (2020)](https://doi.org/10.5194/hess-24-2931-2020)
- [Polz et al. (2020)](https://doi.org/10.5194/amt-13-3835-2020)
- [Overeem et al. (2016)](https://doi.org/10.5194/amt-9-2425-2016)

**Wet antenna attenuation**, comparing the following methods:
- [Schleiss et al. (2013)](https://doi.org/10.1109/LGRS.2012.2236074)
- [Leijnse et al. (2008)](http://www.sciencedirect.com/science/article/pii/S0309170808000535)
- [Pastorek et al. (2021)](https://doi.org/10.1109/TGRS.2021.3110004) (the model denoted "KR-alt" in this study is used here)

Additional notebooks are available that can be used to explore the reference data from openMRG and to derive radar data along the CMLs' paths.

## Radar Merging Method Intercomparison

Intercomparison of different methods for merging radar rainfall data with CMLs using `mergeplg`.

In [Øydvin et al. (2025)](https://doi.org/10.5194/egusphere-2025-6371), we assessed the impact of merging commercial microwave link (CML) data with weather radar for quantitative precipitation estimation (QPE) using two openly available datasets (OpenMRG and OpenRainER) with contrasting observational densities. Multiple merging methods are compared, including kriging with external drift (KED) and a block kriging interpolation method that accounts for the line-average nature of CMLs.

Merging CML data improves radar QPE, with reductions in mean absolute error (MAE) of up to 38% on average for KED, though performance varies with rainfall intensity, distance to observations, and network density.

The merging framework and intercomparison study are openly available at https://github.com/OpenSenseAction/radar_adjustment_intercomparison, enabling reproducibility and further exploration.

```{figure} assets/merging_intercomparison_fig2_from_preprint.png
:width: 600px
:align: center

Figure taken from [Øydvin et al. (2025)](https://doi.org/10.5194/egusphere-2025-6371); more details are available in the paper.
```
