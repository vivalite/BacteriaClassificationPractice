# Bacteria Classification Practice
Transfer learning & fine-tune bacteria classifier on EfficientNet, InceptionV3, Xception and ResNet50 with Keras.

The dataset DIBaS was published as the main dataset of the paper Deep learning approach to bacterial colony classification (https://doi.org/10.1371/journal.pone.0184554) It was collected by the Chair of Microbiology of the Jagiellonian University in Krakow. The samples were stained using the Gramm’s method. All images were taken with an Olympus CX31 Upright Biological Microscope and an SC30 camera with a 100 times objective under oil-immersion. The DIBaS dataset is publicly available here: http://misztal.edu.pl/software/databases/dibas/ 

To run the Jupyter notebook and prepare the enveronment I suggest using Anaconda. Make sure you install Python 3.8, Tensorflow 2.3. I wasn't able to get higher Tensorflow GPU version working on my computer but the notebook should be able to run in the latest Tensorflow.

Extract all DIBaS dataset into C:\DIBaS_Dataset\Data folder. Make sure each bacteria strain in there own folder.

Copy all Jypyter notebooks to C:\DIBaS_Dataset\.

Now you should be able to use DataPrepare notebook to create croped & splited data folder with image size match the model's optimal input requirement. (For example EfficientNet-B4 calls for input size 380, you should have folder C:\DIBaS_Dataset\Data380 created)
For a list of model's optimal input requirement please refer to https://github.com/keras-team/keras-applications.

After you have created croped & splited data folder, run the training notebook. It may take few hours to complete (Or minutes if you have very strong GPU).

That's all.
