# ECG Hearthbeat Classification

## Database

The notebooks are supposed to work on the [PTB](https://physionet.org/content/ptbdb/1.0.0/) and [MIT_BIH](https://physionet.org/content/mitdb/1.0.0/) datasets.

## Setup

The notebooks are supposed to run on Google Colab (it is possible to run it locally by changing the file paths and removing the drive mount for Google drive.

### Packages
It may be required to install the PyWavelets library using for running the DBLSTM-WS and the ensemble models. The package may be installed by running the following command:

```bash
$ pip install PyWavelets
```

### Train
In the first cells of each notebook you can find the following line:

```python
train = False
```

This indiates that the model will be loaded from the specified .h5 file. and no training will be performed. To train the model simply change the previous cell to:

```python
train = True
```

### File paths
In the first cells of each notebook you can find 2 (in the case of transfer learning 3) paths:

```python
data_path = "../input/"
model_path = "../../H5/<database name>/<model name>.h5"
```

The first path indicates the directory of the datasets, the second path indicates the file from which the model will be loaded (or saved if training is enabled). For the ensemble models, the ```model_path``` variable should point to the folder which contains the .h5 files:

```python
model_path = "../../H5/<PTB || MIT>/"
```

## Contributors

* [@Matteo-Omenetti](https://github.com/Matteo-Omenetti)
* [@ravifrancesco](https://github.com/ravifrancesco)
