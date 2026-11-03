# gsg_colorbars
Highly colorful colorbars for those who want their data to stand out.
These colorbars are perceptually uniform and sequential, meaning they increase/decrease in lightness linearly.
The non-diverging colorbars are all colorblind friendly due to the linear changes in lightness.
The diverging colorbars for the most part are color blind friendly, especially strbry_flds_frvr_div, terra, chntclr, and swmp_rnbw which retain their positive-negative contrast under colorblind filters.



<img width="803" height="313" alt="image" src="https://github.com/user-attachments/assets/d6c8e91c-c71d-4ca4-99bf-548bf9ae5589" />
<img width="803" height="478" alt="image" src="https://github.com/user-attachments/assets/cf5e32fa-b223-40e8-9a26-b85dd90ce0e1" />
<img width="803" height="368" alt="image" src="https://github.com/user-attachments/assets/b21fa8e2-203f-4453-977c-ac33d6f178b6" />






calling them in matlab:

  gulf = load('/path/gulf.txt');
  colormap(gulf);


calling them in python (crazy I know):

  import numpy as np
  from matplotlib.colors import ListedColormap
  
  gulf= np.loadtxt(Path(r"path\gulf.txt"))
  cmap = ListedColormap(gulf)
