# gsg_colorbars
Highly colorful colorbars for those who want their data to stand out.



<img width="803" height="313" alt="image" src="https://github.com/user-attachments/assets/7bdcc9fe-38ac-4a67-8fd3-c6f0beeaeefd" />
<img width="803" height="478" alt="image" src="https://github.com/user-attachments/assets/56937f76-0645-40c7-b1cb-9734f10469ce" />
<img width="803" height="368" alt="image" src="https://github.com/user-attachments/assets/61254edd-d285-4dd7-9e85-cafdad8e94fd" />





calling them in matlab:

  gulf = load('/path/gulf.txt');
  colormap(gulf);


calling them in python (crazy I know):

  import numpy as np
  from matplotlib.colors import ListedColormap
  
  gulf= np.loadtxt(Path(r"path\gulf.txt"))
  cmap = ListedColormap(gulf)
