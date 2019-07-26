# TenorFlow-Image-Classifiation
A version of the image classifier built with transfer learning through ResNet50.

Requirements:
Needs a h5 file with weights named model_weights.h5, a model file named model.json and a json file with the classes named class_names.json. keras documentation on saving model to json and weights to h5: https://keras.io/getting-started/faq/#savingloading-only-a-models-architecture You can generate the class_names json file with this code:

import json

class_names = json.dumps(<TRAINING_GEN_NAME>.class_indices)
with open("class_names.json", "w") as json_file:
    json_file.write(class_names)

Directions:
  Run at least one training sesion before making any prediction. This wil generate weights needed to make accurate predictions.
