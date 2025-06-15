# ObsidianPublic
Evaluating public export from Obsidian


- [Testing formats](docs/Testing%20formats.md)
- [Testing formats](blob/main/docs/Testing%20formats.md)
- [Index](blob/main/index.md)
- [Index](https://github.com/perolo/ObsidianPublic/blob/main/docs/Testing%20formats.md)
- https://perolo.github.io/ObsidianPublic/


## Obsidian-export
```bash
$ nix-shell -p obsidian-export

$ rm -rf doc/

$ obsidian-export ../yocreo/Public/ doc

```
## mkdocs
```bash
$ nix-shell -p mkdocs

$ rm -rf docs/*

$ obsidian-export ../yocreo/Public/ doc

$ mkdocs serve

$ mkdocs gh-deploy

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


## Evaluation of obsidian-export + mkdocs
- Does not understand PlantUML
- Does not follow move - requires a clean directory
- Pages available on https://perolo.github.io/ObsidianPublic/
- Problem found: https://github.com/zoni/obsidian-export/issues/87
```bash
$ obsidian-export ../yocreo/Public/ doc
Error: Failed to export '../yocreo/Public/Resources/Global Consequences of Helicopter Money.md'

Caused by:
   0: Failed to decode YAML frontmatter in '../yocreo/Public/Resources/Global Consequences of Helicopter Money.md'
   1: invalid type: string "Excellent follow-up. Let’s explore the **global consequences**, implications for **trust in the monetary system and currency value**, and examine **historical examples (real and theoretical)** of **helicopter money** in action.", expected a YAML mapping
```