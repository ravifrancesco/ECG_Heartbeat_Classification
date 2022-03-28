# ECG Hearthbeat Classification

## Database

The notebooks are supposed to work on the PTB and MIT_BIH databases.

## Setup

The notebooks are supposed to run on Google Colab (it is possible to run it locally by changing the file paths and removing the drive mount for Google drive.

### Packages
On Colab, it may be required to install the PyWavelets library using for running the DBLSTM-WS models. The package may be installed by running the following command:

```bash
$ pip install PyWavelets
```

### File paths
In the notebooks some filepaths may be found (for the .h5 files for the models and the .csv files for the databases). They have to be changed to match the file paths of the environment where the models are run.

## Contributors

* [@Matteo-Omenetti](https://github.com/Matteo-Omenetti)
* [@ravifrancesco](https://github.com/ravifrancesco)
