This example is based on the [CLEVR dataset](https://github.com/facebookresearch/clevr-dataset-gen)

1. Download and install blender from [here](https://www.blender.org/download/)
2. Add paths to your `.bashrc` or `.zshrc` for handy shortcuts
```bash
# Suppose /Applications/ is the directory where it is installed (e.g. on MacOS)
export BLENDER=/Applications/Blender.app/Contents/Resources/
export BLENDER_VERSION=3.1
export BLENDER_HOME=$BLENDER/$BLENDER_VERSION/
export BLENDER_PYTHON=${BLENDER_HOME}/python/bin/python3.10
export BLENDER_SITE_PACKAGES=${BLENDER_HOME}/python/lib/python3.10/site-packages/
```
3. Add image generation folder to Blender python's path:
```
echo $PWD/image_generation >> $BLENDER_SITE_PACKAGES/clevr.pth
```
