def im2patch(img, nseg=4):
  """
  Image to patch conversion fn.
  :param img: Image to convert.
  :param nseg: number of segments.
  :return: A list of image patches.
  """
  # find the step sizes in height and width directions.
  y_slide = img.shape[0] // nseg
  x_slide = img.shape[1] // nseg
  # initiate patches.
  patches = []
  # loop through the image.
  for h in range(nseg):
    for w in range(nseg):
      # extract the patches.
      patches.append(img[(y_slide*h):(y_slide*(h+1)), (x_slide*w):(x_slide*(w+1))])
  return patches
