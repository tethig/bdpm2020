# Guidance
[Excellent article](https://medium.com/learning-machine-learning/present-your-data-science-projects-with-jupyter-slides-75f20735eb0f).

## Dynamic Rendering
```
jupyter nbconvert index.ipynb --to slides --post serve \
--SlidesExporter.reveal_theme=solarized --SlidesExporter.reveal_scroll=True --SlidesExporter.reveal_transition=none
```

## Conversion
```
jupyter nbconvert index.ipynb --to slides --reveal-prefix=../reveal.js \
--SlidesExporter.reveal_theme=solarized --SlidesExporter.reveal_scroll=True --SlidesExporter.reveal_transition=none
mv index.slides.html index.html
```
