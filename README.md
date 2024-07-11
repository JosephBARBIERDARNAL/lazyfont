# lazyfont

A simple way to load fonts for matplotlib.

<br>

## Installation

```
pip install git+https://github.com/JosephBARBIERDARNAL/lazyfont.git
```

<br>

## Usage

#### Load a font for a matplotlib chart:

```python
from lazyfont import load_font
import matplotlib.pyplot as plt

# load font
font = load_font(family="Sarabun", style='italic', weight='bold')

# check how the font looks on a minimalist example
fig, ax = plt.subplots(figsize=(10, 6), dpi=200)
ax.text(
   x=0.15, y=0.5,
   s=f"What an easy way to load fonts, isn't it?",
   font=font,
   fontsize=20
)
plt.show()
```

![output of quick start](img/quickstart.png)

<br>

#### Download a font locally:

```python
from lazyfont import download_font
download_font(family="Sarabun", style='normal', weight='thin')
```

`Font installed at: /Users/josephbarbier/Desktop/lazyfont/Sarabun_Thin.ttf`