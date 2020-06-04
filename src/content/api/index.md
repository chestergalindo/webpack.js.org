---
title: Introducción
sort: 1
contribuidores:
  - tbroadley
---

Una cantidad de interfaces estan disponibles para personalizar los procesos de compilazación.
Algunas carateristicas se sobreponen entre las diferentes interfaces, e.g. una opción de configuración puede estar
disponible via un CLI flag, mientas otras existen mediante una sola interfas.
Para obtener un rendimiento de alto nivel deberias iniciar.


## CLI

The Command Line Interface (CLI) to configure and interact with your build. It
is especially useful in the case of early prototyping and profiling. For the
most part, the CLI is simply used to kick off the process using a configuration
file and a few flags (e.g. `--env`).

[Learn more about the CLI!](/api/cli)


## Module

When processing modules with webpack, it is important to understand the
different module syntaxes -- specifically the [methods](/api/module-methods)
and [variables](/api/module-variables) -- that are supported.

[Learn more about modules!](/api/module-methods)


## Node

While most users can get away with just using the CLI along with a
configuration file, more fine-grained control of the compilation can be
achieved via the Node interface. This includes passing multiple configurations,
programmatically running or watching, and collecting stats.

[Learn more about the Node API!](/api/node)


## Loaders

Loaders are transformations that are applied to the source code of a module.
They are written as functions that accept source code as a parameter and return
a new version of that code with transformations applied.

[Learn more about loaders!](/api/loaders)


## Plugins

The plugin interface allows users to tap directly into the compilation process.
Plugins can register handlers on lifecycle hooks that run at different points
throughout a compilation. When each hook is executed, the plugin will have full
access to the current state of the compilation.

[Learn more about plugins!](/api/plugins)
