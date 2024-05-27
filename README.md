# place-recognition

#### Step 1
* Build a panoramic dataset, using the videos dataset , there is 4 faculties, a video for each faculté
* each video we extract some frames from it (frames should not be so close nor too far)
* from these frame we make an panoramic image ( image stitching )


### Step 2
* There we extract image features from each panoramic image using SIFT ( and save them in an .npz  file)
* when the user gives an input image we extract its features using SIFT too
* And we compare with each saved features (.npz)
* Then we classify it with the one that has many simillar features

### Step 3
* for building detection we use image segmentation using a pre-trained model from facebook ( detectron2 )
