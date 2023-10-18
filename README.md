# ShipGen #
Generate Parametric Ship Hull with a Guided Tabular Diffusion Model. The following sections detail train a guided diffusion model to generate parametric ship hull designs

## Data Set ##
This project uses the ShipD Dataset. The ShipD Dataset is a dataset of 30,000 parametric ship hull designs. Included in the dataset performance metrics, meshes, and images of each hull.  
Sample code for the dataset is found here: https://github.com/noahbagz/ShipD
The dataset, code, and documentation: https://www.dropbox.com/sh/jg98r425v7ly89l/AAA49uMr7_mhaVmRDrPq0NU_a?dl=0

## Running the Code ##
After you download the ShipD Dataset, run the jupyter notebooks in this order:
1) "SetUp_Diffusion_TrainingData.ipynb" This will format the hull data and the performance data to prepare it for Machine Learning.
2) "Generate_negative_samples.ipynb" This creates a set of hulls that violate at least one constraint for classification purposes.
3) "Run_guidedDiffusion_Notebook.ipynb" This notebook trains the diffusion model, constriant classifier, and regression models. It also generates samples.

## Other Resources ##
Check out MIT's DeCoDE Lab for more machine learning tools and datasets for engineering design:
decode.mit.edu

The ShipGen Porject Page is found at:
decode.mit.edu/projects/shipgen/
