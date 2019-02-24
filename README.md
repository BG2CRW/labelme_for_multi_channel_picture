<img src="labelme/icons/icon.png" align="right" />

# labelme: Image Polygonal Annotation with Python

## Features

- [x] Image annotation for polygon, rectangle, circle, line and point. ([tutorial](examples/tutorial))
- [x] Image flag annotation for classification and cleaning. ([#166](https://github.com/wkentaro/labelme/pull/166))
- [x] Video annotation. ([video annotation](examples/video_annotation))
- [x] GUI customization (predefined labels / flags, auto-saving, label validation, etc). ([#144](https://github.com/wkentaro/labelme/pull/144))
- [x] Exporting VOC-format dataset for semantic/instance segmentation. ([semantic segmentation](examples/semantic_segmentation), [instance segmentation](examples/instance_segmentation))
- [x] Exporting COCO-format dataset for instance segmentation. ([instance segmentation](examples/instance_segmentation))



## Requirements

- Ubuntu / macOS / Windows
- Python2 / Python3
- [PyQt4 / PyQt5](http://www.riverbankcomputing.co.uk/software/pyqt/intro) / [PySide2](https://wiki.qt.io/PySide2_GettingStarted)


## Installation

There are options:

- Platform agonistic installation: [Anaconda](#anaconda)
- Platform specific installation: [Ubuntu](#ubuntu), [macOS](#macos), [Windows](#windows)

### Anaconda

```bash
git clone https://github.com/BG2CRW/labelme_for_multi_channel_picture.git
cd labelme_for_multi_channel_picture

# Install anaconda3 and labelme
curl -L https://github.com/wkentaro/dotfiles/raw/master/local/bin/install_anaconda3.sh | bash -s .
source .anaconda3/bin/activate
pip install -e .
```

## How to build standalone executable

Below shows how to build the standalone executable on macOS, Linux and Windows.  
Also, there are pre-built executables in
[the release section](https://github.com/wkentaro/labelme/releases).

```bash
# Setup conda
conda create --name labelme python==3.6.0
conda activate labelme

git clone https://github.com/BG2CRW/labelme_for_multi_channel_picture.git
cd labelme_for_multi_channel_picture

# Build the standalone executable
pip install .
pip install pyinstaller
pyinstaller labelme.spec
dist/labelme --version
```

## Acknowledgement

This repo is the fork of [mpitid/pylabelme](https://github.com/wkentaro/labelme)
