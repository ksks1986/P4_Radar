1. Implementation steps for the 2D CFAR process.
  First, to consider edge of matrix as 0.0, I made result matrix "RDM_CFAR" and is initialized 0.0.
  To get the average of training cell, I use following equation.

  Train_Cells_Average = ((Train_Cells_Sum + Guard_Cells_Sum + CUT) - (Guard_Cells_Sum + CUT)) / (the_number_of_training_cells)

  After getting training cells average, adding offset to trainng cells average, resulting as threshold value.

  Finally, compare the threshold and RDM value.


2. Selection of Training, Guard cells and offset.
  At first, the number of traing and guard cell is same as previous my 1D lesson.
  And setting offset = 2.5dB, too many false points are detected.
  So increasing the offset, set to 5.0dB, then appropriate points are detected.


3. Steps taken to suppress the non-thresholded cells at the edges.
  As mentioned abobe (1.), I initialized 0.0 at the edges.

