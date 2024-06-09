# Ai Plugin

The *AiPlugin* is an optional engine plugin that provides functionality for doing typical game AI tasks.

To enable the plugin, use the [plugin selection](../../projects/plugin-selection.md) dialog and enable the *AiPlugin*. Some functionality will show up in the form of *components*, other functionality may only be available through C++ code.

To get access to the C++ functionality, your code needs to additionally link against the AiPlugin library.

## Navigation

The plugin provides functionality to create navmeshes on-demand at runtime. See [this chapter](runtime-navmesh.md) for details.

Additionally there is C++ functionality available for searching paths and *steering* characters along the found path.

# See Also

* [Runtime Navmesh](runtime-navmesh.md)