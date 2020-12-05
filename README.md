# Custom-Fast-RCNN - python
This repository includes a custom object detector.
The "custom" part is basically how the data set of pictures needs to be designed. Namely The dataset needs to be a folder with the pictures in .jpeg format 
and annotations in .xml files,  so the structure of the Data Set looks like this:

Dataset
├── annots
└── images

and the annots part looks like this:


<annotation>
	<folder>Dataset</folder>
	<filename>00001.jpg</filename>
	<path>...</path>
	<source>
		<database>Unknown</database>
	</source>
	<size>
		<width>450</width>
		<height>319</height>
		<depth>3</depth>
	</size>
	<segmented>0</segmented>
	<object>
		<name>kangaroo</name>
		<pose>Unspecified</pose>
		<truncated>0</truncated>
		<difficult>0</difficult>
		<bndbox>
			<xmin>233</xmin>
			<ymin>89</ymin>
			<xmax>386</xmax>
			<ymax>262</ymax>
		</bndbox>
	</object>
	<object>
		<name>kangaroo</name>
		<pose>Unspecified</pose>
		<truncated>0</truncated>
		<difficult>0</difficult>
		<bndbox>
			<xmin>134</xmin>
			<ymin>105</ymin>
			<xmax>341</xmax>
			<ymax>253</ymax>
		</bndbox>
	</object>
</annotation>

The annotations are basically the actual mask coordinates of the bounding boxes ideally outputted by the neural network.

For a better explanaition look at this link : https://machinelearningmastery.com/how-to-train-an-object-detection-model-with-keras/

I basically took the code from this tutorial to get it and then just made it easily available for google colab.
