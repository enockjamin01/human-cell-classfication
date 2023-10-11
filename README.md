# Human Cell Classifier

A classifier to predict different human cells in a microscope image is trained on a Convolutional neural network (CNN) built to predict three human cells ['Adipose', 'Muscle', 'Red'].

The model is trained with 446 color images of all classes together and 446 greyscale images of all classes together so a total of 892 images with 50 epochs on a batch size 16.

## Modules to install

```bash
python3 -m pip install TensorFlow

pip install opencv-python

pip install matplotlib
```

## Frameworks used

* Tensorflow
* Open CV
* Matplotlib

## Training more classes :

To train the model with more classes add more subdirectories of the particular class in the function Alter the "classes" variable on both .ipynb files and add required images in the subdirectory Do one hot encoding and train the more with suitable hyperparameters.

## Usage

* You can load the model (.keras) file from the main branch and start predicting with your images
  [cell_classifier.ipynb](https://github.com/enockjamin01/human-cell-classfication/blob/main/cell_classifier.ipynb)

* Please delete (delete.txt) file from each sub directory classes in the Git repo after cloning (This was done to demonstrate only the structure of the image and dataset folders)

* You can add more classes by adding more classes directory and images to the images folder and add the classes directory to the dataset folder 

* Remember to run the data_preprocessing.ipynb file after downloading images for the required classes
  [data_preprocessing.ipynb](https://github.com/enockjamin01/human-cell-classfication/blob/main/data_preprocessing.ipynb)

## How to get images

* Google Microscope images of the required cell and fetch somewhere between 150-300 images of each class

## Sample image for download

![Sample microscope image](https://github.com/enockjamin01/human-cell-classfication/blob/main/sample/sample-muscle-2.jpg)

## Splitting of data

* Train = 90%
* Validiation = 7%
* Test = 3%

## Accuracy and Loss plot

* Accuracy

![Accuracy](https://github.com/enockjamin01/human-cell-classfication/blob/main/plots/accuracy.png)

#Loss

![Loss](https://github.com/enockjamin01/human-cell-classfication/blob/main/plots/loss-plot.png)

## License

[MIT](https://choosealicense.com/licenses/mit/)
