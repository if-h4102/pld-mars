# MARS

## Guide de style

[Guide de style](./guide de style.md)

## PlantUML

Les diagrammes UML sont générés à partir de déclarations
[_PlantUML_][plantuml].

### Installation

1. From [the download page][plantuml-download], download the
   `PlantUML compiled Jar`.

2. Add it as a command-line program.

   - Windows
     
     1. Save `plantuml.jar` in `C:/Program Files/PlantUML/plantuml.jar`
     
     2. Create a file `plantuml.cmd` in the same directory with this content:
     
        ```batch
        @echo off
        java -jar "%~dp0plantuml.jar" -charset UTF-8 %*
        ```
     
     3. Add the directory to your `PATH` environment variable.

   - Linux: Check `alias` and send a PR to add instructions here.

### Utilisation

[Documentation](http://plantuml.com/command-line)

Generate all as SVG (default: PNG):

```shell
plantuml -tsvg **/*.puml
```

### Éditeurs

#### Planttext

[Planttext](http://www.planttext.com/planttext)

#### Plugin IntelliJ Idea

Open the plugin repositories: **File | Settings.. | Plugins | Browse
Repositories...**.
 
Install `PlantUML Integration` and restart your IDE.


[plantuml]: http://plantuml.com/
[plantuml-download]: http://plantuml.com/download
