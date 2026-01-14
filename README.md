# gsg_colorbars
Highly colorful colorbars for those who want their data to stand out.

## Available Colorbars

This repository contains a collection of vibrant colorbar definitions in text format. Each file contains RGB color values that can be used for data visualization.

### Colorbar Files

- **rainbow.txt** - A vibrant rainbow color scheme from red to violet
- **sunset.txt** - A warm sunset color scheme from deep purple to bright orange
- **ocean.txt** - A deep ocean color scheme from dark blue to cyan
- **fire.txt** - A hot fire color scheme from black to white through red and yellow
- **tropical.txt** - A vibrant tropical color scheme with bright pinks, greens, and blues
- **neon.txt** - An electric neon color scheme for maximum visibility

## File Format

Each colorbar file follows a simple text format:
- Lines starting with `#` are comments
- Each color is defined on a separate line with three values: `R G B`
- RGB values range from 0 to 255
- Colors are ordered from the start to the end of the colorbar

### Example

```
# Rainbow Colorbar
# Format: R G B (values 0-255)
255 0 0
255 127 0
255 255 0
0 255 0
0 0 255
75 0 130
148 0 211
```

## Usage

You can load these colorbar files into your data visualization software or use them programmatically. Here are some examples:

### Python (matplotlib)

```python
import numpy as np
import matplotlib.pyplot as plt
from matplotlib.colors import ListedColormap

# Read colorbar file
colors = []
with open('colorbars/rainbow.txt', 'r') as f:
    for line in f:
        line = line.strip()
        if line and not line.startswith('#'):
            r, g, b = map(int, line.split())
            colors.append([r/255.0, g/255.0, b/255.0])

# Create colormap
cmap = ListedColormap(colors)

# Use in plot
plt.imshow(data, cmap=cmap)
plt.colorbar()
plt.show()
```

### Python (generic)

```python
def load_colorbar(filename):
    """Load a colorbar from a text file."""
    colors = []
    with open(filename, 'r') as f:
        for line in f:
            line = line.strip()
            if line and not line.startswith('#'):
                r, g, b = map(int, line.split())
                colors.append((r, g, b))
    return colors

colors = load_colorbar('colorbars/sunset.txt')
```

## Contributing

Feel free to add your own colorbar definitions! Follow the existing file format and create a pull request.
