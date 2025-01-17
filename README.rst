.. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
   If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
   This text does not appear on pypi or github. It is a comment.

.. image:: https://github.com/collective/lineage.controlpanels/workflows/ci/badge.svg
    :target: https://github.com/collective/lineage.controlpanels/actions
    :alt: CI Status

.. image:: https://img.shields.io/pypi/v/lineage.controlpanels.svg
    :target: https://pypi.python.org/pypi/lineage.controlpanels/
    :alt: Latest Version

.. image:: https://img.shields.io/pypi/status/lineage.controlpanels.svg
    :target: https://pypi.python.org/pypi/lineage.controlpanels
    :alt: Egg Status

.. image:: https://img.shields.io/pypi/pyversions/lineage.controlpanels.svg?style=plastic   :alt: Supported - Python Versions

.. image:: https://img.shields.io/pypi/l/lineage.controlpanels.svg
    :target: https://pypi.python.org/pypi/lineage.controlpanels/
    :alt: License

=====================
lineage.controlpanels
=====================

.. warning::
    ALPHA: THIS IS STILL EXPERIMENTAL CODE!

Allows Lineage child site specific configurations for plone.registry based controlpanels.

Not available in Lineage Childsites
-----------------------------------

The following control panels change global settings. Therefore they are not available in subsites.

- content-controlpanel
- dexterity-types
- filter-controlpanel
- maintenance-controlpanel
- prefs_install_products_form
- resourceregistry-controlpanel
- security controlpanel
- usergroup-groupprefs
- usergroup-userprefs


This is also disabled, but should probably fixed to work with local registries too:
- portal_registry

This one stores it's configuration in the registry but has changes one setting in portal_actions, which would affect all sites.
Thus disabled.
- syndication-controlpanel


Installation
------------

Install lineage.controlpanels by adding it to your buildout::

    [buildout]

    ...

    eggs =
        lineage.controlpanels


and then running ``bin/buildout``

Source Code and Contributions
-----------------------------

If you want to help with the development (improvement, update, bug-fixing, ...)
of ``lineage.controlpanels`` this is a great idea!

The code is located in the
`github collective <https://github.com/collective/lineage.controlpanels>`_.

You can clone it or `get access to the github-collective
<http://collective.github.com/>`_ and work directly on the project.

Maintainer is Johannes Raggam and the BlueDynamics Alliance developer team. We
appreciate any contribution and if a release is needed to be done on pypi,
please just contact one of us
`dev@bluedynamics dot com <mailto:dev@bluedynamics.com>`_


Contributors
------------

- Jens W. Klein <jens@bluedynamics.com>
- Daniel Widerin <daniel@widerin.net>


License
-------

The project is licensed under the GPLv2.
