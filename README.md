About r-acs-feedstock
=====================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-acs-feedstock/blob/main/LICENSE.txt)

Home: http://dusp.mit.edu/faculty/ezra-glenn, http://eglenn.scripts.mit.edu/citystate/, http://mailman.mit.edu/mailman/listinfo/acs-r

Package license: GPL-3.0-only

Summary: Provides a general toolkit for downloading, managing, analyzing, and presenting data from the U.S. Census (<https://www.census.gov/data/developers/data-sets.html>), including SF1 (Decennial short-form), SF3 (Decennial long-form), and the American Community Survey (ACS).  Confidence intervals provided with ACS data are converted to standard errors to be bundled with estimates in complex acs objects.  Package provides new methods to conduct standard operations on acs objects and present/plot data in statistically appropriate ways.

Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13611&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-acs-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--acs-green.svg)](https://anaconda.org/conda-forge/r-acs) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-acs.svg)](https://anaconda.org/conda-forge/r-acs) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-acs.svg)](https://anaconda.org/conda-forge/r-acs) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-acs.svg)](https://anaconda.org/conda-forge/r-acs) |

Installing r-acs
================

Installing `r-acs` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-acs` can be installed with `conda`:

```
conda install r-acs
```

or with `mamba`:

```
mamba install r-acs
```

It is possible to list all of the versions of `r-acs` available on your platform with `conda`:

```
conda search r-acs --channel conda-forge
```

or with `mamba`:

```
mamba search r-acs --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search r-acs --channel conda-forge

# List packages depending on `r-acs`:
mamba repoquery whoneeds r-acs --channel conda-forge

# List dependencies of `r-acs`:
mamba repoquery depends r-acs --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [anaconda.org](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-acs-feedstock
========================

If you would like to improve the r-acs recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-acs-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@conda-forge/r](https://github.com/conda-forge/r/)
* [@izahn](https://github.com/izahn/)

