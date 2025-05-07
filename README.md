# Analysis for ECG Data

This repository contains Python code, primarily within a Jupyter Notebook (`paper.ipynb`), for analyzing ECG data.

## Prerequisites

To run this code, you will need Python 3 and the following libraries installed:

* `pickle` (standard library, aliased as `pkl`)
* `numpy` (aliased as `np`)
* `os` (standard library)
* `glob` (standard library)
* `matplotlib` (specifically `matplotlib.pyplot`, aliased as `plt`)

You can typically install these libraries using pip:

```bash
pip install numpy matplotlib
```
## Running the Code

1.  **Set up the Environment:** Ensure Python and the prerequisite libraries are installed.
2.  **Organize Data:** Place your `.pkl` data files in the correct directory structure as described in the "Directory Structure" and "Data Files" sections of the full README.
3.  **Open Jupyter Notebook:** Launch Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook
    # or
    jupyter lab
    ```
4.  **Run the Notebook:** Open `paper.ipynb`. You can run the cells sequentially. The notebook is divided into sections:
    * **Code Cell 1:** Defines the `get_numeric_template` function.
    * **Code Cell 2:** Defines the `plot_cam_template` function.
    * **Markdown Cell 3:** Header for "Baseline" section.
    * **Code Cell 4:** Loads data for the "Baseline" model (`file_name = 'BaselineDS_balanced_naf'`), prints metrics, calls `plot_cam_template`, and saves the figure to `Figures/Baseline.png`.
    * **Markdown Cell 5:** Header for "RR model" section.
    * **Code Cell 6:** Loads data for the "RR model" (`file_name = 'lambda_500_rr_balanced_NAF'`), prints metrics, calls `plot_cam_template`, and saves the figure to `Figures/RR.png`.
    * **Markdown Cell 7:** Header for "P-Wave" section.
    * **Code Cell 8:** Loads data for the "P-Wave model" (`file_name = 'lambda_500_pwave_naf'`), prints metrics, calls `plot_cam_template`, and saves the figure to `Figures/PWave.png`.
    * **Markdown Cell 9:** Header for "ALL" section.
    * **Code Cell 10:** Loads data for the "ALL" model (`file_name = 'lambda_500_all_naf'`), prints metrics, calls `plot_cam_template`, and saves the figure to `Figures/All.png`.

    Execute each code cell to perform the analysis and generate the plots. The plots will be displayed in the notebook and saved to the `Figures/` directory.
