Working :


In the initial step, the RGB images of all the leaf samples were picked up. The step-by-step procedure of the proposed system:

RGB image acquisition;
Convert the input image from RGB to HSI format;
Masking the green-pixels;
Removal of masked green pixels;
Segment the components;
Obtain useful segments;
Evaluating feature parameters for classification;
Configuring SVM for disease detection.
Colour Transformation: HSI (hue, saturation, intensity) color model is a popular color model because it is based on human perception. After transformation, only the H (hue) component of HSI colour space is taken into account since it provides us with the required information.

Masking Green Pixels: This is performed as green colour pixel represent the healthy region of a leaf. Green pixels are masked based on the specified threshold values.

Segmentation: The infected portion of the leaf is extracted by segmenting the diseased part with other similar coloured parts (say, a brown coloured branch of a leaf that may look like the disease) which have been considered in the masked out image, are filtered here. All further image processing is done over a region of interest (ROI) defined at this stage.

Classification: From the previous results we analyze and evaluate the features like the area of the leaf, percentage(%) of the leaf infected, the perimeter of the leaf, etc., for all the leaf images, and pass it to the SVM classifier.
