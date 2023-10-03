# Degraph

Dependencies graph visualization tool

```mermaid
---
title: DeGraph
---
classDiagram
    class DeGraph

    class FileStructureLoader
    <<interface>> FileStructureLoader

    class LangParser
    <<interface>> LangParser

    LangParser --> DeGraph
    LangParser --> FileStructureLoader

    class DeGraphDrawer
    <<interface>> DeGraphDrawer

    class DeGraphExporter
    <<interface>> DeGraphExporter

    DeGraphExporter --> DeGraph
    DeGraphDrawer --> DeGraph
```
