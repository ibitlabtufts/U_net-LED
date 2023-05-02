# U_net-LED
Run Denoising-Unet.ipynb in google colab.
Create two folders under /sample_data in the name of "image" (for training inputs) and "label" (for corresponding labels).
Create another folder in the name of "test" to save the predictions.
results = model.predict_generator(testGene,X,verbose=1): X is the number of test samples.
To save the test results: 
  !zip -r zip_file_name.zip test_folder
  from google.colab import files
  files.download(zip_file_name.zip)
To save the model in hdf5 format:
  files.download(model.hdf5)
  
# Non-learning methods in Tensorflow:
1. BM3D
2. NLM
