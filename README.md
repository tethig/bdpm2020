# Guidance
* [Excellent article](https://medium.com/learning-machine-learning/present-your-data-science-projects-with-jupyter-slides-75f20735eb0f).
* [Guidance on nbconvert](https://nbconvert.readthedocs.io/en/latest/usage.html)

## Dynamic Rendering
```
jupyter nbconvert index.ipynb --to slides --post serve \
--SlidesExporter.reveal_theme=solarized --SlidesExporter.reveal_scroll=True --SlidesExporter.reveal_transition=none
```

## Conversion
Setup:
```
git clone https://github.com/hakimel/reveal.js.git
cd reveal.js
git checkout 3.5.0
cd ..
```
Conversion:
```
jupyter nbconvert index.ipynb --to slides --reveal-prefix reveal.js \
--SlidesExporter.reveal_theme=solarized --SlidesExporter.reveal_scroll=True --SlidesExporter.reveal_transition=none
mv index.slides.html index.html
```
