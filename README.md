# COVASim

COVID-19 Agent-based Simulator. A stochastic individual-based model that can be used for Covid-19 (novel coronavrius, SARS-nCoV-2) epidemic projections, scenario interventions, etc., and adapted to different contexts (e.g. the Diamond Princess cruise ship, cities, countries).


## Requirements

Python >=3.6 (64 bit).


## Installation

Standard Python package installation: `python setup.py develop`.

The module should then be importable as `import covasim`.


## Usage

Simplest usage is `python -i scripts/run_sim.py`. This will create a figure (and, by default, save it to disk). Different flavors are described below.


## Flavors

The package contains multiple different flavors of COVASim. Each flavor has its own parameters file (`parameters.py`) and slight variations to the model (`model.py`). Different versions are:
* `cova_base` -- not to be used directly, the base classes for the simulation.
* `cova_cdc` -- for intervention scenarios for the CDC, uses detailed age mixing patterns for Seattle
* `cova_cruise` -- for the Diamond Princess cruise ship, includes data on diagnoses and passengers and crew
* `cova_oregon` -- estimtaes for the Oregon Health Authority
* `cova_seattle` -- estimates for the Washington Department of Health
* `cova_webapp` -- for running an interactive webapp

More information is available in the `README.md` in each folder (coming soon).


## That's great, but I want to know more

Totally reasonable request. We are still working on the documentation.