# pyGIMLi - Open-source Research & Teaching Software
## A tutorial for the SEG Near Surface Webinar series

**Instructors:**
[Florian Wagner][florian]<sup>1</sup>,
[Thomas Günther][halbmy]<sup>2</sup>
and
[Carsten Rücker][carsten]<sup>3</sup>

> <sup>1</sup>
> Geophysical Imaging and Monitoring, RWTH Aachen University, Germany
> <br>
> <sup>2</sup>
> Leibniz Institute for Applied Geophysics, Hannover, Germany
> <br>
> <sup>3</sup>
> Institut für Angewandte Geowissenschaften, Technische Universität Berlin, Germany

## About

In this webinar, we introduce you to pyGIMLi, an open-source software for Geophysical
Inversion and Modelling. After giving some general information on pyGIMLi, we will
demonstrate its potential by inverting field ERT data through adding increasing
complexity.

##
Date: March 19, 2023

Recorded video: https://youtu.be/qbLGbSEWOSw

## Installation

We recommend installing a Python distribution locally.
In case of installation problems, one can alternatively use Google Colab.

### Local Python installation using conda

We recommend installing a Python distribution like [miniforge][miniforge] or [Anaconda][anaconda].
- Install miniforge: https://github.com/conda-forge/miniforge#install
- follow the installation instructions on https://www.pygimli.org/installation.html
- open a terminal (on Windows Powershell prompt)

```
conda create -n pg -c gimli -c conda-forge pygimli=1.5 jupyter
```

or download the file https://github.com/gimli-org/SEGwebinar/environment.yml

```
mamba env create --file environment.yml
```

Activate the environment and call Jupyter Notebook:

```
conda activate pg
jupyter notebook
```

### Google colab

1. Login to [colab][colab] using your Google account.
2. Open new Notebook and choose the GitHub option
3. Paste the [webinar] URL https://github.com/gimli-org/SEGwebinar
4. Select the template or full notebook
5. Create your own notebook, starting with `!pip install pygimli`

## License

This work is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0.html)

## Further reading
* [pyGIMLi website][pygimli] with API reference and lots of tutorials and examples
* [pyGIMLi tutorial][transform2021] given on Transform 2021 (with 2h Youtube tutorial)
* [pyGIMLi tutorial][transform2022] given on Transform 2022 (with 2h Youtube tutorial)
* Jupyter [Notebook collection][notebooks] using pyGIMLi
* Collection of [Example data][exampledata] used here and on [website][pygimli]

## References
* Rücker, C., Günther, T., Wagner, F.M. (2017): pyGIMLi: An open-source library for modelling and inversion in geophysics, Computers & Geosciences 109, 106-123, [doi:10.1016/j.cageo.2017.07.011](https://doi.org/10.1016/j.cageo.2017.07.011).
* Hübner, R., Günther, T., Heller, K., Noell, U. & Kleber, A. (2017): Impacts of a capillary barrier on infiltration and subsurface stormflow in layered slope deposits monitored with 3-D ERT and hydrometric measurements. Hydrol. Earth Syst. Sci. 21, 5181-5199, [doi:10.5194/hess-21-5181-2017](https://doi.org/10.5194/hess-21-5181-2017).
* Jordi, C., Doetsch, J., Günther, T., Schmelzbach, C. & Robertsson, J.O.A. (2018): Geostatistical regularisation operators for geophysical inverse problems on irregular meshes. Geophysical Journal International 213, 1374-1386, [doi:10.1093/gji/ggy055](https://doi.org/10.1093/gji/ggy055).
* Grünenbaum, N., Günther, T., Greskowiak, J., Vienken, T., Müller-Petke, M. & Massmann, G. (2023): Salinity distribution in the subterranean estuary of a meso-tidal high-energy beach characterized by Electrical Resistivity Tomography and Direct Push technology. J. of Hydrol. 617, 129074, [doi:10.1016/j.jhydrol.2023.129074](https://doi.org/10.1016/j.jhydrol.2023.129074).
* Wunderlich, T., Fischer, P., Wilken, D., Hadler, H., Erkul, E., Mecking, R., Günther, T., Heinzelmann, M., Vött, A. & Rabbel, W. (2018): Constraining Electric Resistivity Tomography by Direct Push Electric Conductivity logs and vibracores: An exemplary study of the Fiume Morto silted riverbed (Ostia Antica, Western Italy). Geophysics 83(3), B87-B103, [doi:10.1190/geo2016-0660.1](https://doi.org/10.1190/geo2016-0660.1).
* Wagner, F.M., Mollaret, C., Günther, T., Kemna, A., Hauck, A. (2019): Quantitative imaging of water, ice, and air in permafrost systems through petrophysical joint inversion of seismic refraction and electrical resistivity data. Geophys. J. Int. 219, 1866-1875. [doi:10.1093/gji/ggz402](https://doi.org/10.1093/gji/ggz402).
* Ronczka, M., Günther, T., Grinat, M. & Wiederhold, H. (2020): Monitoring freshwater-saltwater interfaces with SAMOS - installation effects on data and inversion. Near Surf. Geophys. 18(4), 369-383, [doi:10.1002/nsg.12115](https://doi.org/10.1002/nsg.12115).
* Hübner, R., Heller, K., Günther, T. & Kleber, A. (2015): Monitoring hillslope moisture dynamics with surface ERT for enhancing spatial significance of hydrometric point measurements. Hydrology and Earth System Sciences 19(1), 225-240, [doi:10.5194/hess-19-225-2015](https://doi.org/10.5194/hess-19-225-2015).
* Jiang, C., Igel, J., Dlugosch, R., Müller-Petke, M., Günther, T., Helms, J., Lang, J. & Winsemann (2020): Magnetic resonance tomography constrained by ground-penetrating radar for improved hydrogeophysical characterisation, Geophysics 85(6), JM13-JM26, [doi:10.1190/geo2020-0052.1](https://doi.org/10.1190/geo2020-0052.1).
* Skibbe, N., Günther, T. & Müller-Petke, M. (2021): Improved hydrogeophysical imaging by structural coupling of two-dimensional magnetic resonance and electrical resistivity tomography. Geophysics 86 (5), WB135-WB146, [doi:10.1190/geo2020-0593.1](https://doi.org/10.1190/geo2020-0593.1).
* Rochlitz, R., Becken, M. & Günther, T. (2023): Three-dimensional inversion of semi-airborne electromagnetic data with a second-order finite-element forward solver. Geophys. J. Int. 234(1), 528-545, [doi:10.1093/gji/ggad056](https://doi.org/10.1093/gji/ggad056).

[florian]: https://www.gim.rwth-aachen.de/
[halbmy]: https://www.liag-hannover.de/
[carsten]: https://www.tu.berlin/geophysik/
[pygimli]: https://www.pygimli.org
[gimli]: https://github.com/gimli-org/gimli
[webinar]: https://github.com/gimli-org/SEGwebinar
[notebooks]: https://github.com/gimli-org/notebooks
[exampledata]: https://github.com/gimli-org/example-data
[transform2021]: https://github.com/gimli-org/transform2021
[transform2022]: https://github.com/gimli-org/transform2022
[jupyter]: https://jupyter.org/
[colab]: https://colab.research.google.com
[anaconda]: https://www.anaconda.com/download
[jupyterlab]: https://jupyterlab.readthedocs.io
[miniforge]: https://github.com/conda-forge/miniforge
[conda-environ]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
[environment_yml]: https://github.com/gimli-org/SEGwebinar/environment.yml
