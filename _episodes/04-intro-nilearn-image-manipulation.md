--- 
title: "Introduction to Nilearn and Image Manipulation"
teaching: 30
exercises: 15
questions:
- "How can I perform basic arithmetic operations on full MR images"
objectives:
- "Use Nilearn's nibabel wrappers to handle image loading and inspection"
- "Learn how to perform basic image operations and masking" 
- "Resampling data to work across MR modalities"
keypoints:
- "MR images can be treated as if they were 3D arrays!"
---

# Warming up with Nilearn

Moving forward, we'll be using Nilearn which is an analysis/visualization library meant for neuroimaging. Nilearn is a convenient tool for us since it *wraps* nibabel; meaning that under the hood nibabel is being used. This means that if we wanted to perform more advanced operations, we can jump down to using nibabel instead of using the high level operations provided for by nilearn. 

~~~
import os
import matplotlib.pyplot as plt
from nilearn import image as img
from nilearn import plotting as plot
~~~
{: .python}

