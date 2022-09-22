# DeepCNN-ImageClassifier
This project used sample of happy and sad images to predict one is happy or sad

## Installations
> The saved model can be used to predict new images not trained with and this can happen locally after a set of installations and instructions:
install and import these packages:
* `!pip install tensorflow tensorflow-gpu opencv-python`
* `from tensorflow.keras.models import load_model`
* Downoad the saved model [Here](https://drive.google.com/file/d/1qkpHQ2DO7Y6ihtfP3GrSBcs7U_Go_yzs/view?usp=sharing)
* load the Model `new_model = load_model('/path/MkHappySadModel.h5')`
* Dowload two samples of pictures [Sad and happy]
run the following:
* `img = cv2.imread('/content/test.jpeg')`
 * `resize = tf.image.resize(img, (256,256))`
 * `np.expand_dims(resize, 0).shape`
 * `yhat = model.predict(np.expand_dims(resize/255, 0))`
 * `if yhat > 0.5:
      print("predicted class is sad" else: "predicted class is happy`
      
## Content
Repo comtains jupyter notebook that has all the code used in creating this model

## Recommendation
Use jupyterlab or google colab
