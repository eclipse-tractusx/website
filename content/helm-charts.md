---
title: Helm Chart Repository
sidebar: true # or false to display the sidebar
sidebarlogo: fresh-white-alt # From (static/images/logo/)
include_footer: true # or false to display the footer
---

The Eclipse IoT Packages™ project decided to host a Helm chart repository in order to share the
effort of validating and publishing charts. Eclipse IoT projects are welcome to re-use that
infrastructure to publish their charts, whether they are part of an IoT package or not. Of course
projects can still host their own repositories and charts.

This repository is intended to work with Helm version 2 and 3. Features which work only with Helm 3
are labeled explicitly.

## Adding the repository

You can add the repository with a simple command:

``
helm repo add tractus-x https://eclipse.org/tractusx/charts
``

This will add the repository, using the name `tractusx`.

After you have added the repository you should tell helm to download the index for its contents:

``
helm repo update
``

## See the content <small><span class="badge badge-secondary">Helm v3</span></small>

You can browse through the content using:

`` 
helm search repo
``   

If you also want the search to include charts that are still under development, e.g. *alpha*, *beta* and *pre-release* versions:

`` 
helm search repo --devel
``

If you want to search for *charts* only, then you can use

``
helm search repo tractus-chart
``

and if you want to search for *packages* only

``
helm search repo tractus-x
``

## How chart publishing works

# !!! This needs to be adjusted when the actions are acutally defined

All chart changes will be verified by a [Github action](https://github.com/eclipse/packages/actions), this is done on every pull request.

Once a pull request is merged, the updated chart will be deployed by a [Jenkins job](https://ci.eclipse.org/packages/job/Website/job/master/).
This job takes care of publishing the resources and generating an updated `index.yaml`.

*The content of this page is adapted from the [Eclipse IoT Packages](https://github.com/eclipse/packages) project.*
