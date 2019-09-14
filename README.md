Training of model happens in the jupyter notebook under training folder. The output of training file is a model file named roses-model.pkl, this file should be copied to the model serving module.

The model serving module is available inside the model-serving-docker directory. Inside this directory, there is an app foler, the roses-model.pkl should be available there.

For building docker image, go to the directory where Dockerfile resides, and issued command docker build .  This will build the docker image.

For running the image, run the commmand - docker run -p 5000:5000 "image-name"
