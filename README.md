# img_to_patch
Image to patch conversion with python .

[![License](https://img.shields.io/github/license/KiLJ4EdeN/img_to_patch)](https://img.shields.io/github/license/KiLJ4EdeN/img_to_patch) [![Version](https://img.shields.io/github/v/tag/KiLJ4EdeN/img_to_patch)](https://img.shields.io/github/v/tag/KiLJ4EdeN/img_to_patch) [![Code size](https://img.shields.io/github/languages/code-size/KiLJ4EdeN/img_to_patch)](https://img.shields.io/github/languages/code-size/KiLJ4EdeN/img_to_patch) [![Repo size](https://img.shields.io/github/repo-size/KiLJ4EdeN/img_to_patch)](https://img.shields.io/github/repo-size/KiLJ4EdeN/img_to_patch) [![Issue open](https://img.shields.io/github/issues/KiLJ4EdeN/img_to_patch)](https://img.shields.io/github/issues/KiLJ4EdeN/img_to_patch)
![Issue closed](https://img.shields.io/github/issues-closed/KiLJ4EdeN/img_to_patch)

# usage

```python
import matplotlib.pyplot as plt
import matplotlib.image as mage
from img_to_patch import im2patch

# include the path to your desired image.
temp_image = mage.imread('image.jpg')
# perform the conversion.
patches = im2patch(temp_image, nseg=8)
# length is two times the nseg param.
print(len(patches))
# demonstrate the results.
for patch in patches:
  plt.figure()
  plt.imshow(patch)
```
