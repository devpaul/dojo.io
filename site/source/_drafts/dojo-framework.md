---
title: The New Framework
authorId: paul
---

## The New Dojo Framework

A number of changes are happening with Dojo. As the project continues to stabilize around a set of modules and APIs we 
constantly evaluating feedback from the community as well as our own processes.

During the Dojo 2 cycle, we have identified pain points that have the potential to become bottlenecks or affect the 
momentum of the project. Central to these issues is the complexity of managing the seven projects that make up the basis
for the dojo framework: core, has, i18n, routing, shim, stores, and widget-core. These projects have separate
repositories, separate issues trackers, and separate versioning. We have found that managing these projects individually
requires a great deal of coordination when publishing and managing inter-dependencies.

## Why are we making this change?

When the Dojo Framework was undergoing rapid iterations during development and beta phases, multiple
projects allowed for decisions to be made quickly in small compartmentalized packages. After releasing Dojo 2, the core
APIs in the project have stabilized considerably and the focus of the project has changed to long-term support of the
framework and adding functionality and features beyond the core. What this means is the advantages of multiple packages
that existed during our rapid iteration phases have given way to greater upkeep and release costs.

Now that the core Dojo packages are stable, we have decided it best to consolidate these seven packages into a single 
[@dojo/framework](https://github.com/dojo/framework) package. By doing this we will make a number of improvements to 
the project for both the team and our end-users.

* Improve the publish process
* Reduce the number of repositories so issues are in one place
* Reduce the number of packages needed by developers
* Maintain the 2.0 release w/ patches
* Keep the history from the original framework repositories

These changes will improve the overall development experience for our end users are they have to manage fewer core Dojo
packages. It will also simplify the release process and management of Dojo for us and our contributors. We expect this
to result in better and more frequent releases that are easier for Dojo users to update in their individual projects.

## Support and Migration

The [Dojo Toolkit](https://dojotoolkit.org) has a long history of support and patches. Dojo 2 will continue to see
patches backported to all of the projects that make up the foundation of @dojo/framework. We are also planning to add
a CLI migration tool to help update your Dojo 2 project's imports and usage. If you want to take a look at
the changes being made take a look at the [@dojo/framework](https://github.com/dojo/framework) repository. We'd also
love to hear your feedback on [Gitter](https://gitter.im/dojo/dojo2).
