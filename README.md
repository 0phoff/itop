<div align="center">

<img alt="Logo" src="https://raw.githubusercontent.com/0phoff/ibb/master/docs/source/_static/logo.svg" width="60%"/>

[![PyPi][pypi-badge]][pypi-url]
[![NPM][npm-badge]][npm-url]
[![Documentation][docs-badge]][docs-url]

</div>

Interactive BramBox
===================
IPython widgets for visualizing [brambox](http://eavise.gitlab.io/brambox/) annotation and detection dataframes on their images.
These widgets help with doing computer vision research in IPython Notebooks.


## Widget List
You can find more information about each widget by checking its doc-string:
```python
import ibb

# Python
help(ibb.<WIDGET_NAME>)

# Alternative in Notebook
?ibb.<WIDGET_NAME>
```

- **ImageCanvas**: Barebones widget to draw numpy arrays as images and rectangles. Use this to create your own widgets.
- **ImageViewer**: Image list browser.
- **BramboxViewer**: Brambox dataset browser. Browse through your annotations or detections for visual inspection.
- **PatchViewer**: Brambox dataset browser, but cut images in smaller patches (with overlap) for easier visualisation.
- **CutoutViewer**: Brambox dataset browser, but view individual annotations or detections as cutouts of the image.


## Installation

To install use pip:

```bash
> pip install ibb
> jupyter nbextension enable --py --sys-prefix ibb
```


For a development installation (requires npm),

```bash
> git clone https://github.com/0phoff/ibb.git
> cd ibb 
> pip install -e .
> jupyter nbextension install --py --symlink --sys-prefix ibb
> jupyter nbextension enable --py --sys-prefix ibb
```

[pypi-badge]: https://img.shields.io/pypi/v/ibb?logo=pypi
[pypi-url]: https://pypi.org/project/ibb
[npm-badge]: https://img.shields.io/npm/v/ibb?logo=npm
[npm-url]: https://npmjs.com/package/ibb
[docs-badge]: https://img.shields.io/readthedocs/ibb?logo=readthedocs
[docs-url]: https://ibb.readthedocs.io
