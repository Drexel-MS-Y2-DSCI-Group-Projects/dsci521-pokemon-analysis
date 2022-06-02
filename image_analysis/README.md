## Image Analysis

### Dependencies

This notebook uses cv2 to read image information in-memory and tqdm to help with identifying preprocessing progress.

### Running

`merged.json` is a prerequisite for running this notebook. Image urls in the sprites array is converted into hash values containing information about the image. It is a lengthy process to fetch all of the images so their information is cached in a `post_transformation.json`. Otherwise, simply execute the steps to get the related info. Adding array slices to the ndex and sprite loops can help fetching subsets of the data.
