# FilmXPro recipe drops

The manifest the app reads to find recipes published after a release.

- `drops/recipes.json` — the live list, served at
  `https://trunghai298.github.io/filmxpro-drops/drops/recipes.json`

A drop carries recipe settings and words, nothing else: no images, no film
definitions, and nothing about anyone using the app. The app fetches this file
with a plain GET when the Library is opened, at most once in six hours.

To publish a recipe, add a record and push. To take one down, delete its record
and push — a copy anyone already saved keeps working.

The field reference and the checks to run before publishing are in the app
repository, under `docs/drops/README.md`.
