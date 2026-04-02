# Stolt-Nielsen inspired theme - Can change as per compnay's logo

Prompt : Have a look at the visualizations of this notebook and standardize the style of the outputs as per the example below:
BG_COLOR   = "#ffffff"   # White background
FG_COLOR   = "#000000"   # Black text
PRIMARY    = "#d71920"   # Stolt red (logo color)
SECONDARY  = "#4d4d4d"   # Neutral dark gray
ACCENT1    = "#1f78b4"   # Blue (for clarity in charts)
ACCENT2    = "#33a02c"   # Green (for positive metrics)

plt.rcParams.update({
    "figure.facecolor": BG_COLOR,
    "axes.facecolor": BG_COLOR,
    "axes.edgecolor": FG_COLOR,
    "axes.labelcolor": FG_COLOR,
    "xtick.color": FG_COLOR,
    "ytick.color": FG_COLOR,
    "text.color": FG_COLOR,
    "axes.prop_cycle": plt.cycler(color=[PRIMARY, SECONDARY, ACCENT1, ACCENT2]),
    "grid.color": SECONDARY,
    "grid.alpha": 0.2,
    "grid.linestyle": "--",
})

def style_axes(ax, edgecolor=FG_COLOR, linewidth=1.2):
    ax.set_facecolor(BG_COLOR)
    ax.tick_params(colors=FG_COLOR)
    for spine in ax.spines.values():
        spine.set_color(FG_COLOR)
    for patch in ax.patches:
        if hasattr(patch, "get_facecolor"):
            face = patch.get_facecolor()
            patch.set_edgecolor(edgecolor or face)
