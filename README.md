# Maturitni-prace

Prvni verze.

## Python environment

The notebooks use CERN ROOT's Python bindings, pandas, and a Jupyter kernel. Create the project environment and install its dependencies with:

```bash
python3 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt
.venv/bin/python -m ipykernel install --user --name maturitni-prace --display-name "Maturitni-prace (.venv)"
```

Select **Maturitni-prace (.venv)** as the notebook kernel in VS Code.

## Interactive ROOT plots

The ROOT plotting cells use interactive JSROOT output. Open the project notebook in JupyterLab to use zooming and other interactive plot controls:

```bash
.venv/bin/jupyter lab
```

Open `rekonstrukce_Z-boson.ipynb` in the JupyterLab tab and run the notebook. JSROOT is loaded from the ROOT project’s online servers, so an internet connection is needed. VS Code's notebook output does not render ROOT's embedded JavaScript; to display static plots there, change `%jsroot on` to `%jsroot off` in the plotting cell.