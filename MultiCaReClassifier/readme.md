# MultiCaReClassifier for Medical Image Classification

The MultiCaReClassifier is a model ensemble used for multilabel medical image classification. It includes classes such as:
- image_type: 'radiology', 'pathology', 'endoscopy', 'ophthalmic_imaging', 'medical_photograph', 'electrography', 'chart'.
- image_subtype: 'ultrasound', 'x_ray', 'ct', 'mri', 'h&e', 'immunostaining', 'fundus_photograph', 'ekg', 'eeg', etc.
- radiology_region: 'thorax', 'head', 'abdomen', 'upper_limb', 'lower_limb', etc.
- radiology_view: 'frontal', 'sagittal', 'axial', 'oblique', etc.


1. Clone the HuggingFace repo:
```
!git clone https://huggingface.co/mauro-nievoff/MultiCaReClassifier
```

2. Change the directory:
```
%cd /content/MultiCaReClassifier
```

3. Import the MultiCaReClassifier class:
```
from MultiCaReClassifier.pipeline import *
```

4. Get the predictions for a given image folder:
```
predictions = MultiCaReClassifier(image_folder = '/content/img')
predictions.data.head()
```


**Model Training by:** Facundo Roffet

**Data Curation and Postprocessing by:** Mauro Nievas Offidani
