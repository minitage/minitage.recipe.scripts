******************************************************************************
Recipe for compiling and installing software with or without minitage
******************************************************************************

.. contents::

=======================
Introduction
=======================

This is a collection of recipe which can be use inside or outside a minitage environment.
What is interresting in using them in minitage is that you ll have all your system dependencies in
the build environment automaticly.

The egg has those entry point:
    - *cmmi*: install configure/make/make install softwares
    - *fetch*: fetch something, somewhere, with git, http, frp, static, hg, svn or bzr.
    - *egg*: install python eggs / packages 'setuptoolisables'
    - *printer*: print or dump to a file all versions needed to achieve eggs
      requirements (versions.cfg made easy)
    - *scripts*: install scripts from an egg and install egg dependencies if they
      are not already in the cache
    - *wsgi*: Make a Python paste configuration file eatable by mod_wsgi with
      all the eggs dependencies you need.

The reasons why i have rewrite yet another buildout recipes builder are:
    - Support for downloading stuff
    - Do not rely on easy_install dependency system
    - Support on the fly patchs for eggs and other distribution.
    - Support multiple hooks at each stage of the build system.
    - Support for distutils
    - Robust offline mode
    - We like pypi, but offer a mode to scan for eggs without need to check
      the index,
    - Support malformed or not indexed distributions.
      In other terms, we provide an url, and the recipe builds it, that's all.
    - All recipes must support automaticly minitage dependencies and rpath linking.

You can browse the code on minitage's following resources:

    - http://git.minitage.org/git/minitage/eggs/minitage.recipe/
    - http://www.minitage.org/trac/browser/minitage/eggs/minitage.recipe

You can migrate your buldouts without any effort with buildout.minitagificator:

    * http://pypi.python.org/pypi/buildout.minitagificator

======================================
Makina Corpus sponsored software
======================================
|makinacom|_

* `Planet Makina Corpus <http://www.makina-corpus.org>`_
* `Contact us <mailto:python@makina-corpus.org>`_

  .. |makinacom| image:: http://depot.makina-corpus.org/public/logo.gif
  .. _makinacom:  http://www.makina-corpus.com



DISCLAIMER - ABANDONED/UNMAINTAINED CODE / DO NOT USE
=======================================================
minitage project was terminated in 2013. Consequently, this repository and all associated resources (including related projects, code, documentation, and distributed packages such as Docker images, PyPI packages, etc.) are now explicitly declared **unmaintained** and **abandoned**.

I would like to remind everyone that this project’s free license has always been based on the principle that the software is provided "AS-IS", without any warranty or expectation of liability or maintenance from the maintainer.
As such, it is used solely at the user's own risk, with no warranty or liability from the maintainer, including but not limited to any damages arising from its use.

Due to the enactment of the Cyber Resilience Act (EU Regulation 2024/2847), which significantly alters the regulatory framework, including penalties of up to €15M, combined with its demands for **unpaid** and **indefinite** liability, it has become untenable for me to continue maintaining all my Open Source Projects as a natural person.
The new regulations impose personal liability risks and create an unacceptable burden, regardless of my personal situation now or in the future, particularly when the work is done voluntarily and without compensation.

**No further technical support, updates (including security patches), or maintenance, of any kind, will be provided.**

These resources may remain online, but solely for public archiving, documentation, and educational purposes.

Users are strongly advised not to use these resources in any active or production-related projects, and to seek alternative solutions that comply with the new legal requirements (EU CRA).

**Using these resources outside of these contexts is strictly prohibited and is done at your own risk.**

Regarding the potential transfer of the project to another entity, discussions are ongoing, but no final decision has been made yet. As a last resort, if the project and its associated resources are not transferred, I may begin removing any published resources related to this project (e.g., from PyPI, Docker Hub, GitHub, etc.) starting **March 15, 2025**, especially if the CRA’s risks remain disproportionate.

