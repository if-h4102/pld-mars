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

   - Linux: 
      1. Create a file named plantuml in /bin
      2. Put this line in your file :`java -jar PATH/plantuml.jar -charset UTF-8 $@`, with PATH the path to the download     plantuml.jar
      3. Add the execution permission on the file /bin/plantuml (the file you have just created).
      4. Now, you use the command `plantuml`, with any arguments.

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
