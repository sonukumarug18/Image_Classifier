# Image Classifier 

built a powerful image classifier, using only very few training examples --just a few hundred or thousand pictures from each class you want to be able to recognize.

More information about this Project.

1. Problem Statement-
    To built a classification model to correctly classify the images to their respective class(Cats Vs Dogs).

2. Sources:
   (a) Date:    27th feb 2023. (Project Date)

3. Dataset_folder-

    data that can be downloaded at:
https://www.kaggle.com/c/dogs-vs-cats/data

    Folder structure:
    - created a data/ folder
    - created train/ and validation/ subfolders inside data/
    - created cats/ and dogs/ subfolders inside train/ and validation/
    - put the cat pictures index 0-999 in data/train/cats
    - put the cat pictures index 1000-1400 in data/validation/cats
    - put the dogs pictures index 0-999 in data/train/dogs
    - put the dog pictures index 1000-1400 in data/validation/dogs
    So that we have 1000 training examples for each class, and 400 validation examples for each class.
    In summary, this is our directory structure:
    ```
    data/
        train/
            dogs/
                dog001.jpg
                dog002.jpg
                ...
            cats/
                cat001.jpg
                cat002.jpg
                ...
        validation/
            dogs/
                dog001.jpg
                dog002.jpg
                ...
            cats/
                cat001.jpg
                cat002.jpg
                ...


4. Techniques and Algorithms used -

     1. Model_1 - Trained a small Network from scratch using CNN.
     2. Model_2 - Used a bottleneck feature of pretrained VGG-16 Network with Fully Connected layers and initialized all the weights with Imagenet trained weights

5. Conclusions-
    1. Model_1:
        1. Got validation accuracy of 0.77 after 50 epochs.
        2. the variance of the validation accuracy is fairly high, because accuracy is a high-variance metric and because we only use 800 validation 3. samples.
        4. A good validation strategy in such cases would be to do k-fold cross-validation, but this would require training k models for every evaluation round.

    2. Model_2:
        1. Reached validation accuracy of 0.88 after 50 epoch,not bad at all.



         

