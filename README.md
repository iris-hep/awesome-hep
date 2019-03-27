# awesome-hep

A curated list of awesome high energy and particle physics software.

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

The focus of this page is on:

   * Software for doing high energy/particle physics _analysis_, since this is the area most in need of the discoverability that an awesome list provides.
   * Software that can be used _right now_, not development projects or unmaintained projects.
   * Software that can be used independently of any collaboration framework (except for the collaboration-specific sections at the end).

See the [curated list of awesome lists](https://github.com/sindresorhus/awesome) for an idea of what an awesome list is all about: lists of links to projects, arranged by topic, so that users can find what they need. If you want to add anything to this list (or remove something that doesn't satisfy the criteria above), submit a [pull request](https://github.com/iris-hep/awesome-hep/pulls).

Links to other lists of packages are in **bold**.

## C++

   * [ROOT](https://root.cern/): If you're working in particle physics and you don't know about ROOT— you need to know about ROOT. It would fit into every category below.

### Distributed processing

   * [Thread Building Blocks (TBB)](https://www.threadingbuildingblocks.org/)

### Aggregation/histogram filling

   * [Boost.Histogram](https://github.com/HDembinski/histogram)
   * [YODA](https://yoda.hepforge.org/)

### Fitting

   * [RooFit](http://roofit.sourceforge.net): The classic, powerful symbolic fitting library built into ROOT (and therefore PyROOT).
   * [GooFit](https://github.com/GooFit/GooFit): A OpenMP/CUDA binned and unbinned fitting package for C++ and Python, similar to RooFit, more limited but up to 1000x faster.

_(FIXME: something in the Combiner/HistFactory category?)_

### Reproducibility, reinterpretation

   * [Rivet](https://rivet.hepforge.org)

### C++/Python interoperability

   * [pybind11](https://pybind11.readthedocs.io/en/stable/)

## Python

   * **[PyHEP-resources](https://github.com/hsf-training/PyHEP-resources): detailed list of Python tutorials and useful libraries in Python.**
   * [PyROOT](https://root.cern.ch/pyroot): built into ROOT; access to 100% of ROOT functions in Python.
   * [rootpy](http://www.rootpy.org/): _Pythonic_ interface to PyROOT.

### Pure physics

   * [particle](https://github.com/scikit-hep/particle): particle data, such as masses and PDG properties
   * [decaylanguage](https://github.com/scikit-hep/decaylanguage)

### Data access

   * [uproot](https://github.com/scikit-hep/uproot)
   * [root_numpy](http://scikit-hep.org/root_numpy/)
   * [root_pandas](https://github.com/scikit-hep/root_pandas)
   * [pyhepmc](https://pypi.org/project/pyhepmc/)
   * [pylhe](https://pypi.org/project/pylhe/)
   * [PySLHA](https://pypi.org/project/pyslha/): read, write, and plot SUSY Les Houches Accord (SLHA) supersymmetric spectrum/decay files

### Distributed processing

   * [Parsl](http://parsl-project.org/)
   * [Joblib](https://joblib.readthedocs.io/en/latest/)
   * [Dask](http://dask.pydata.org)
   * [yadage](https://github.com/yadage/yadage)
   * [PySpark](https://spark.apache.org/docs/latest/)

### Event generation

   * [numpythia](https://github.com/scikit-hep/numpythia)
   * [pyjet](https://github.com/scikit-hep/pyjet)

### Data processing

   * [awkward-array](https://github.com/scikit-hep/awkward-array)
   * [formulate](https://github.com/scikit-hep/formulate): translate TTree::Draw syntax to NumExpr

### Data bookkeeping

   * [Pandas](https://pandas.pydata.org/)

### Plotting (exploratory and publication)

   * [Matplotlib](https://matplotlib.org/)
   * [seaborn](https://seaborn.pydata.org/)

### Other visualization

   * [mcviz](https://github.com/mcviz/mcviz)
   
### Minimization

   * [iminuit](https://iminuit.readthedocs.io/en/latest/): A Cython powered wrapper around Minuit extracted from ROOT.

### Fitting

   * [probfit](https://probfit.readthedocs.io/en/latest/): A fitting tool for Python built on top of iMinuit, can be slow but supports unbinned fits.
   * [pyhf](https://diana-hep.org/pyhf/)
   * [zfit](https://github.com/zfit/zfit): A new TenserFlow fitting package under development.

### Statistics

_(FIXME: there's a lot of these...)_

### Machine learning

   * **[awesome machine learning](https://github.com/josephmisiti/awesome-machine-learning)**
   
### Error propagation

   * [uncertainties](https://uncertainties-python-package.readthedocs.io/en/latest/)

## Go

### Data access

   * [Go-HEP/groot](https://go-hep.org/x/hep/groot): read, write ROOT files in pure-[Go](https://golang.org)
   * [Go-HEP/hepevt](https://go-hep.org/x/hep/hepmc): provide read access to `HEPEVT` `F77` common blocks
   * [Go-HEP/hepmc](https://go-hep.org/x/hep/hepmc): read, write HepMC files in pure-[Go](https://golang.org)
   * [Go-HEP/heppdt](https://go-hep.org/x/hep/heppdt): provide read access to HepPDT data tables
   * [Go-HEP/lcio](https://go-hep.org/x/hep/lcio): provide read/write access to the LCIO data model
   * [Go-HEP/lhef](https://go-hep.org/x/hep/lhef): implement the "Les Houches Event File" data format
   * [Go-HEP/slha](https://go-hep.org/x/hep/slha): implement encoding and decoding of SUSY Les Houches Accords (SLHA) data format
   * [Go-HEP/xrootd](https://go-hep.org/x/hep/xrootd): implement the XRootD protocol
   * [Go-HEP/hbook/yodacnv](https://go-hep.org/x/hep/hbook/yodacnv): implement read/write access to YODA files

### Event generation

   * [Go-HEP/fads](https://go-hep.org/x/hep/fads): `fads` exposes building blocks for a fast simulation of a HEP detector.

### Data processing

   * [Go-HEP/fwk](https://go-hep.org/x/hep/fwk): `fwk` provides a set of tools to process High Energy Physics events data, in a multithread-friendly fashion

### Aggregation/histogram filling

   * [Go-HEP/hbook](https://go-hep.org/x/hep/hbook): hbook is a set of data analysis tools for HEP (histograms (1D, 2D, 3D), profiles and ntuples), with interoperability with ROOT (read/write) TH{1,2}x.

### Plotting (exploratory and publication)

   * [Go-HEP/hplot](https://go-hep.org/x/hep/hplot): a plotting package built on top of [Gonum/plot](https://github.com/gonum/plot) to provide HEP-oriented primitives
   * [Go-HEP/pawgo](https://go-hep.org/x/hep/pawgo): a simple interactive shell to quickly plot hbook histograms from Go
   * [Go-HEP/groot/root-srv](https://go-hep.org/x/hep/groot/cmd/root-srv): a (local) web server able to plot TH{1,2}x, TGraphs and TTrees from a ROOT file
   * [Gophernotes](https://github.com/gopherdata/gophernotes): a Go kernel for the Jupyter notebooks and nteract

### Fitting

   * [Gonum/optimize](https://godoc.org/gonum.org/v1/gonum/optimize): implements algorithms for finding the optimum value of functions
   * [Go-HEP/fit](https://go-hep.org/x/hep/fit): `fit` provides functions to fit data (histograms, data set), using `gonum/optimize`.

### Statistics

   * [Gonum/stat](https://godoc.org/gonum.org/v1/gonum/stat): `stat` provides generalized statistical functions.
   * [Gonum/stat/distuv](https://godoc.org/gonum.org/v1/gonum/stat/distuv): `distuv` provides univariate random distribution types.
   * [Gonum/stat/distmv](https://godoc.org/gonum.org/v1/gonum/stat/distmv): `distmv` provides multivariate random distribution types.

## Publishing

   * [Overleaf](https://www.overleaf.com/): write collaboratively on your web browser with a built-in LaTeX editor; many templates are available for beginners

## Reproducibility, reinterpretation

   * [reana](http://reanahub.io/)

## Data preservation

   * [CERN Open Data Portal](http://opendata.cern.ch/)
   * [HEPData](https://www.hepdata.net/)

## Collaboration-framework specific

### ???
