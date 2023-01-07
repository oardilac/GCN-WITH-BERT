# Shakespeare GCN
This project uses a Graph Convolutional Network (GCN) to analyze and understand the relationships between characters and events in Shakespeare's plays. The GCN is trained on the full texts of the plays, and uses BERT to generate word embeddings as input. We implement and train the GCN using PyTorch Geometric or DGL, and once trained, the model is able to accurately predict character interactions and plot developments in new texts.

## Requirements
To run this project, you will need to install the following dependencies:

* PyTorch
* PyTorch Geometric or DGL
* BERT
* spaCy (for preprocessing)

## Usage
To train the GCN, run the following command:
```
python train.py --data-dir DATA_DIR --output-dir OUTPUT_DIR
```

Replace ***DATA_DIR*** with the directory containing the training data, and ***OUTPUT_DIR*** with the directory where the model and training logs should be saved.

To make predictions with the trained model, run the following command:

```
python predict.py --model-path MODEL_PATH --input-text INPUT_TEXT
```

Replace ***MODEL_PATH*** with the path to the trained model, and ***INPUT_TEXT*** with the text to be analyzed. The predictions will be printed to the console.

## Credits
This project was developed by Oliver Ardila.
