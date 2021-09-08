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

   * [Boost.Histogram](https://github.com/boostorg/histogram)
   * [YODA](https://yoda.hepforge.org/)

### Fitting

   * [RooFit](http://roofit.sourceforge.net): The classic, powerful statistical modelling language and fitting library built into ROOT (and therefore PyROOT). Provides the workspace to serialize models, which is widely used in combinations. [RooFit Tutorials](https://root.cern/doc/master/group__tutorial__roofit.html) [Quick Start](https://root.cern.ch/download/doc/roofit_quickstart_3.00.pdf) [Manual](https://root.cern.ch/download/doc/RooFit_Users_Manual_2.91-33.pdf)
   * [RooStats](https://twiki.cern.ch/twiki/bin/view/RooStats/WebHome) [RooStats tutorials](https://root.cern/doc/master/group__tutorial__roostats.html) Statistical tools built on top of RooFit's statistical modelling language. Provides statistical procedures used for Higgs discovery. Ships with ROOT.
   * [HistFactory](https://twiki.cern.ch/twiki/bin/view/RooStats/HistFactory): A C++ implementation (built on top of RooFit) of the statistical models for binned distributions based on template histograms described in [CERN-OPEN-2012-016](https://cdsweb.cern.ch/record/1456844). Also ships with ROOT.
   * [HistFitter](http://histfitter.web.cern.ch/histfitter/) a tool that integrates HistFactory, RooStats, and RooFit for common analysis use cases.
   * [Combine](https://cms-analysis.github.io/HiggsAnalysis-CombinedLimit/): Combine provides a command line interface to many different statistical techniques available inside RooFit/RooStats used widely inside CMS. [Tutorial](http://twiki.ihep.ac.cn/twiki/view/CMS/CombineTutorial)
   * [GooFit](https://github.com/GooFit/GooFit): A OpenMP/CUDA binned and unbinned fitting package for C++ and Python, similar to RooFit, more limited but up to 1000x faster.
   

### Reproducibility, reinterpretation

   * [Rivet](https://rivet.hepforge.org)
   * [RECAST](https://recast-docs.web.cern.ch) - [talk](https://indico.cern.ch/event/639314/contributions/2726367/attachments/1542484/2419628/ReinterpretationWorkshopFNAL.pdf)
   * [MadAnalysis](https://madanalysis.irmp.ucl.ac.be)
   * [CheckMate](http://checkmate.hepforge.org/)
   * [Contour](https://contur.hepforge.org)
   * [Workshops](https://twiki.cern.ch/twiki/bin/view/LHCPhysics/InterpretingLHCresults) | [Overview of tools](https://twiki.cern.ch/twiki/bin/view/LHCPhysics/RecastingTools)

### C++/Python interoperability

   * [pybind11](https://pybind11.readthedocs.io/en/stable/): Header-only, pure C++ bindings for CPython and PyPy.

## Python

   * **[PyHEP-resources](https://github.com/hsf-training/PyHEP-resources): detailed list of Python tutorials and useful libraries in Python.**
   * [PyROOT](https://root.cern.ch/pyroot): Built into ROOT; access to 100% of ROOT functions in Python. Newer versions are becoming more Pythonic.
   * [rootpy](http://www.rootpy.org/): _Pythonic_ interface to PyROOT, deprecated.

### Pure physics

   * [particle](https://github.com/scikit-hep/particle): Easy access to particle data, such as masses and PDG properties.
   * [decaylanguage](https://github.com/scikit-hep/decaylanguage): Read and process or check `.dec` files and also convert AmpGen syntax to GooFit (extendable).
   * [MadMiner](https://github.com/diana-hep/madminer): Likelihood fits to high-dimensional observables (multi-differential distributions) using Machine-learning techniques.
   * [Vector](https://github.com/scikit-hep/vector): 2D vector, 3D vector, and LorentzVectors, supporting multiple backends, including NumPy, Numba, Awkward, and Numba + Awkward.

### Data access

   * [uproot](https://uproot.readthedocs.io/): Read ROOT files in Pure Python
   * [pyhepmc](https://pypi.org/project/pyhepmc/)
   * [pylhe](https://pypi.org/project/pylhe/)
   * [PySLHA](https://pypi.org/project/pyslha/): Read, write, and plot SUSY Les Houches Accord (SLHA) supersymmetric spectrum/decay files.

### Distributed processing

   * [Parsl](http://parsl-project.org/)
   * [Joblib](https://joblib.readthedocs.io/en/latest/)
   * [Dask](http://dask.pydata.org)
   * [yadage](https://github.com/yadage/yadage)
   * [PySpark](https://spark.apache.org/docs/latest/)
   * [REANA](http://reanahub.io/)

### Aggregation/histogram filling

   * [Hist](https://github.com/scikit-hep/hist): Powerful histogramming package, extends boost-histogram with analysis shortcuts and plotting.
   * [boost-histogram](https://github.com/scikit-hep/boost-histogram): Pybind11 powered interface to Boost.Histogram, intended as a basis for other tools.

### Event generation

   * [numpythia](https://github.com/scikit-hep/numpythia)
   * [fastjet](https://github.com/scikit-hep/fastjet) (replaces [pyjet](https://github.com/scikit-hep/pyjet))

### Data processing

   * [Awkward Array](https://github.com/scikit-hep/awkward-1.0): Manipulate JSON-like data with NumPy-like idioms.
   * [formulate](https://github.com/scikit-hep/formulate): translate TTree::Draw syntax to NumExpr
   * [numba](https://numba.pydata.org): Convert pure Python functions to LLVM bytecode, for speed and easy loop acceleration. Supported by many Scikit-HEP projects, like Awkward and Vector.

### Data bookkeeping

   * [Pandas](https://pandas.pydata.org/): General purpose tabular (1D and 2D labeled mostly) data.
   * [xarray](https://xarray.pydata.org): General purpose ND labeled rectangular data.

### Plotting (exploratory and publication)

   * [Matplotlib](https://matplotlib.org/) (MPL): General purpose plotting library for Python.
   * [seaborn](https://seaborn.pydata.org/): General purpose statistics plotting adaptor for MPL.
   * [mplhep](https://github.com/scikit-hep/mplhep): Adaptor for common HEP needs and experiment styles for MPL.

### Other visualization

   * [mcviz](https://github.com/mcviz/mcviz)
   * [histoprint](https://github.com/scikit-hep/histoprint): Plotting histograms inside the terminal.
   
### Minimization

   * [scipy.optimize](https://docs.scipy.org/doc/scipy/reference/tutorial/optimize.html): General purpose optimization.
   * [iminuit](https://iminuit.readthedocs.io/en/latest/): A pybind11 powered wrapper around Minuit2 extracted from ROOT.

### Statistics and Fitting

   * [pyhf](https://diana-hep.org/pyhf/): implements HistFactory schema supports numpy, TensorFlow, pytorch, MXNet backends
   * [probfit](https://probfit.readthedocs.io/en/latest/): A fitting tool for Python built on top of iMinuit, can be slow but supports unbinned fits.
   * [zfit](https://github.com/zfit/zfit): A new TensorFlow fitting package under development.
   * [TensorFlow Probability](https://www.tensorflow.org/probability/)

### Machine learning

   * [HEPML Resources](https://github.com/iml-wg/HEP-ML-Resources/blob/master/README.md#papers): a general purpose curated list
   * **[awesome machine learning](https://github.com/josephmisiti/awesome-machine-learning)**
   * [JAX](https://github.com/google/jax): General purpose JAX is Autograd and XLA, brought together for high-performance machine learning research.
   * [EnergyFlow](https://energyflow.network): a set of tools aimed at jet physics.
   
### Gaussian Processes
   * [GPy](https://github.com/SheffieldML/GPy)
   * [GPFlow](https://github.com/GPflow/GPflow)
   * [GPyTorch](https://gpytorch.ai)
   
### Blackbox Optimization / Bayesian Optimization / Hyperparameter Optimization
   * [Scikit-Optimize](https://scikit-optimize.github.io)
   * [Spearmint](https://github.com/HIPS/Spearmint)
   * [GPyOpt](https://github.com/SheffieldML/GPyOpt)
   * [A review](https://medium.com/@mikkokotila/a-comprehensive-list-of-hyperparameter-optimization-tuning-solutions-88e067f19d9)

### Error propagation

   * [uncertainties](https://uncertainties-python-package.readthedocs.io/en/latest/): General purpose uncertainty propogation.

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
   * [CERN Analysis Preservation Portal](http://analysispreservation.cern.ch)
   * [HEPData](https://www.hepdata.net/)

## Collaboration-framework specific

### ???
