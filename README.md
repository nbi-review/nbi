[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) ![PyPI](https://img.shields.io/pypi/v/nbi)

## nbi: neural bayesian inference

Do you have challanging inference problems that are difficult to solve with the standard MCMC or Nested Sampling codes?
Are you looking to fit the same forward model to thousands or millions of observed datasets?
`nbi` may be your solution. 

`nbi` is a simulation-based inference engine designed as a straightforward substitution for your favorite MCMC or Nested
Sampling packages. It is great for solving challanging inference problems as well as batch inference problems.
It implements a custom neural posterior estimation algorithm that integrates importance sampling, which allows for
efficient, asymptotically exact results.

## Installation

To install this package, we recommend that you create a dedicated `conda` environment with Python 3.7 or higher

```bash
conda create -n nbi python=3.10
conda activate nbi
```

Then `pip` install this package

```bash
pip install nbi
```

or directly from GitHub for the latest version:

```bash
git clone https://github.com/nbi-review/nbi && cd nbi
pip install .
```

## Usage

See the `examples/` directory for Jupyter notebooks showing the basic functionality of the package.

## Contributing

nbi is released under the BSD license. We encourage you to modify it, reuse it, and contribute changes back for the benefit of others. We follow standard open source development practices: changes are submitted as pull requests and, once they pass the test suite, reviewed by the team before inclusion. 

To contribute back via pull requests, please first fork this report and make sure that you add the original repo as the `upstream` remote:

```bash
git remote add upstream https://github.com/nbi-review/nbi.git
```
When you are ready to submit a PR push to your fork:

```bash
git push -u origin <your_local_branch_with_changes_name>
```

Then create a PR back to `upstream`:

```
https://github.com/<your_username>/nbi/pull/new/<your_local_branch_with_changes_name>
```
