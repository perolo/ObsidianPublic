# ObsidianPublic
Evaluating public export from Obsidian


- [Testing formats](doc/Testing%20formats.md)
- [Testing formats](Testing%20formats.md)
- [[Export Obsidian]]
- [[Adding plugins - PlantUML, Svg, Draw]]


## Obsidian-export
```bash
$ nix-shell -p obsidian-export

$ rm -rf doc/

$ obsidian-export ../yocreo/Public/ doc

```
## mkdocs
```bash
$ nix-shell -p mkdocs

$ rm -rf doc/
$ mkdir doc

$ obsidian-export ../yocreo/Public/ doc

$ mkdocs serve

```

```bash
#once
$ mkdocs new .
INFO    -  Writing config file: ./mkdocs.yml
INFO    -  Writing initial docs: ./docs/index.md
```




## Evaluation of obsidian-export
- Does not understand PlantUML
- Does not follow move - requires a clean directory

