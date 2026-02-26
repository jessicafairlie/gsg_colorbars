# gsg_colorbars
Highly colorful colorbars for those who want their data to stand out.

<img width="610" height="313" alt="image" src="https://github.com/user-attachments/assets/c7bf069f-6cfa-4bee-9546-760d99a9d999" />
<img width="672" height="423" alt="image" src="https://github.com/user-attachments/assets/a923d5de-0d67-44ce-86d8-47b19489cd52" />
<img width="663" height="203" alt="image" src="https://github.com/user-attachments/assets/5dc0d1bf-1c9d-4845-9786-cfda1d45d36f" />




calling them in matlab:

gulf = load('/path/gulf.txt');
colormap(gulf);


calling them in python (crazy I know):

import numpy as np
from matplotlib.colors import ListedColormap

gulf= np.loadtxt(Path(r"path\gulf.txt"))
cmap = ListedColormap(gulf)
