# Embedding Visualization documentation

This is a project for visualizing word embeddings based on the work of [Andrei Kashcha (@anvaka)](https://github.com/anvaka/pm).

Visualization links:
- [FastText Embedding (FR)](https://helboukkouri.github.io/embedding-visualization/#/galaxy/fasttext)

Other links:
- [Data repository](https://github.com/helboukkouri/embedding-visualization-data/tree/gh-pages)
- [Website repository](https://github.com/helboukkouri/embedding-visualization/tree/gh-pages)


## What do I see here?

Every dot here is a word. Position of a package is determined by
force-based graph layout algorithm and usually clusters together words
that depend on each other.

## Navigating in the space

The primary focus of these visualizations is exploratory discovery. It works
best on large monitor, but also works on mobile devices. Use `one finger touch`
to fly forward, `two fingers touch` to fly backward. Rotate your device
to look around.

If you are on the desktop, you can use the `mouse wheel` to bring up a keyboard map:

|    |    |    |   |
|---:|:---|---:|---|
| `W`  | Move forward  | `Up` |Rotate up|
| `S`  | Move backward  | `Down`  |Rotate down |
| `A`  | Move left  |`Left`|Rotate left|
| `D`  | Move right  |`Right` | Rotate right|
| `Q`  | Roll right  |`R` | Fly up|
| `E`  | Roll left  |`F` | Fly down|
| `L`  | Toggle links  | `Space` | Toggle steering |
| `Shift`  | Fly faster  |  |  |

I personally prefer to fly with steering mode on (`spacebar` activates it). In
this mode the spaceship will follow the mouse cursor.

## About connections

You can toggle the links display (using `L` key).

But then we could loose sight of smaller communities. Thus, by default only links whose length is shorter than 150 pixels are shown.

The minimal length of visible links is controlled by `ml` query string argument
(need to open in new tab with updated value to see the result).

# Searching

A search box can be used to locate a particular word in the graph. The input box accepts
regular expressions: If you type `.` it will match all names, and show all results.

Unfortunately for larger graphs (with more than 1,000,000 nodes) this may result
in terrible performance and should be improved in the future.

# Found a bug? Have a suggestion? Feature Requests?

This work is based on [Andrei Kashcha's (@anvaka)](https://github.com/anvaka/pm) Code Galaxies who I'm sure would love to get your feedback. So please, [open a new issue](https://github.com/anvaka/pm/issues/new)
if you have a suggestion, feature request or have found a bug.

For anything related to this particular project, you can open an issue on [the project's repository](https://github.com/helboukkouri/embedding-visualization-data/issues/new).
