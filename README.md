# Humpback-whale-identification</br>
After centuries of intense whaling, recovering whale populations still have a hard time adapting to warming oceans and struggle to compete every day with the industrial fishing industry for food.

To aid whale conservation efforts, scientists use photo surveillance systems to monitor ocean activity. They use the shape of whales’ tails and unique markings found in footage to identify what species of whale they’re analyzing and meticulously log whale pod dynamics and movements. For the past 40 years, most of this work has been done manually by individual scientists, leaving a huge trove of data untapped and underutilized.

This code was of the past Kaggle competiton https://www.kaggle.com/c/humpback-whale-identification , where you’re challenged to build an algorithm to identify individual whales in images. You’ll analyze Happywhale’s database of over 25,000 images, gathered from research institutions and public contributors. By contributing, you’ll help to open rich fields of understanding for marine mammal population dynamics around the globe.

For this problem Siamese network was implemeted. Siamese network inputs two images- reference image, image to be tested. Then the model returns
the similarity between the two images. The inner network is CNN used for images. For more info , visit https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=11&cad=rja&uact=8&ved=2ahUKEwikxJmSoIrjAhXNinAKHRpoDKoQFjAKegQIABAC&url=https%3A%2F%2Fwww.cs.cmu.edu%2F~rsalakhu%2Fpapers%2Foneshot1.pdf&usg=AOvVaw0gKET0McCdIoco9UX2KcsE

To improve the accuracy, bounding boxes were used to remove the unneccessary environment and foxus on the whale tail. 

For bounding boxes trained model by Martin Piotte is used. Her's the link- https://www.kaggle.com/martinpiotte/bounding-box-model

The accuracy on the test set for the above model was 78%. The model was trained by breaking it into several pieces and saving each piece for resung it as computation time required by the code exceeded the alloted time on Google colab i.e 12hrs if it was run at once.
