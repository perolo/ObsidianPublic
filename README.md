# ObsidianPublic

Evaluating public export from Obsidian

* \[Testing formats.md\]
* [Testing formats](Testing%20formats.md)

````bash
$ nix-shell -p obsidian-export

$ rm *.md
$ rm *.png
$ rm -rf Resources/

$ obsidian-export ../yocreo/Public/ .
````

## Evaluation of obsidian-export

* Does not understand PlantUML
* Does not follow move - requires a clean directory
