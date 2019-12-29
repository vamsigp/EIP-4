### Assignment 5 

#### Final Accuracy for submission

- age_output_acc: 0.4068
- bag_output_acc: 0.622
- emotion_output_acc: 0.6986
- footwear_output_acc: 0.6522
- gender_output_acc: 0.8145
- image_quality_output_acc: 0.5554
- pose_output_acc: 0.7898
- weight_output_acc: 0.63

#### Strategy

1. Tried with VGG-16, VGG-19, Resnet50 as base models with NoWeights
	- Observation: Among all 3, Resnet50 has better accuracy; so went on further experiments with the same model.
	- Google colab is giving frequent disconnections, so saved the <b>best model </b> with <b>ModelCheckPoint</b> callback and loading the model and continued with the experiments.
2. Following the above strategy for about <b>~180 epochs</b> achieved below accuracy(attached excel file)
	- Run Model
	- Save Model
	- Rerun Model (Modifying ImageAugmentation and LEarning rate)
		- age_output_acc	: 0.5464
		- bag_output_acc	:	0.7303
		- emotion_output_acc	:	0.749
		- footwear_output_acc	:	0.7843
		- gender_output_acc	:	0.877
		- image_quality_output_acc	:	0.6633
		- pose_output_acc	: 0.8634
		- weight_output_acc	: 0.7122
3. Refactored the file for readability and applied the same strategy but by applying oncycleLR policy, achieved accuracy (accuracy for submission)

#### Modifications to the source file
1. Datagenerator
	- Applied ImageAugmentation with cutout
2. Train Test Split with random state for consistent training and validation sets
3. Applied BatchNormalization for the Head layers
4. Applied Resnet50 istead of VGG-16
5. Modified loss functions (used categoorical_crossentropy for all the classes - for consistency; not sure if it is right way)


##### Could have been improved
1. Applied class balancing strategy
2. Tried with Inception	