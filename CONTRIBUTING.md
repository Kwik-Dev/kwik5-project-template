# Contributing to the project template

## Trying a change

```bash
kwik new scratch --template https://github.com/Kwik-Dev/kwik5-project-template.git                  --branch <your-branch>
kwik run scratch
```

`kwik new` is the acceptance test: if the project it produces does not run, the template is broken.

## Rules that bite

* **`Solar2D/lua_modules` is installed, not authored.** `kwik install` populates it from a release;
  editing it in place produces a change nobody can ship.
* **This is data.** No `Scripts/` (D19), no Python, no shell helpers — `kwik` owns those.
* **A release is a tag**, not a push: `YYYYMMDD-NN`, with `version.txt` and `requires.cli`.
