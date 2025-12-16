# XARA: a python package for eXtreme Angular Resolution Astronomy

**XARA** is a python module that was initially designed to create, extract and manipulate Fourier-phase out of diffraction-dominated astronomical images, using the theory introduced by several journal papers:

- [Martinache (2010), ApJ, 724, 464](https://ui.adsabs.harvard.edu/abs/2010ApJ...724..464M)
- [Martinache (2013), PASP, 125, 422](https://ui.adsabs.harvard.edu/abs/2013PASP..125..422M)
- [Martinache et al (2020), A&A, 636, A72](https://doi.org/10.1051/0004-6361/201936981)

Over the years, the package has been used by several graduate students, motivated by obsevring projects using a wide range of instruments (ground based adaptive optics assisted cameras as well as space borne instruments). The same students  have often made their own fork of the project.

## Tutorial/documentation

A documentation featuring several tutorial examples and a fair amount of howto explanation is available here: <https://frantzmartinache.eu/xara_doc/>

## Acknowledgement

From 2016 to 2022, the development of XARA was supported by the ERC KERNEL project is a development carried out in the context of the KERNEL project. KERNEL has received funding from the European Research Council (ERC) under the European Union's Horizon 2020 research and innovation program (grant agreement CoG - 683029).

## Installation

Xara can be installed from PyPI as `xara-astro`:

```bash
pip install xara-astro
```

### For development

To install Xara for development, first clone this repository:

```bash
git clone https://github.com/fmartinache/xara.git
```

It is generally a good idea to install each package in a separate virtual environment.
You can create one with

```bash
conda create -n xara python
conda activate xara
```

or

```bash
python -m venv venv
source venv/bin/activate
```

Then, install Xara in editable mode, and with the test dependencies.

```bash
python -m pip install -U -e ".[test]"
```

You can then run the tests with


```bash
python -m pytest
```
