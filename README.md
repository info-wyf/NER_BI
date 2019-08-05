# NER_BI
BiLSTM-IDCNN-CRF model

## Requrements

* Python (>=3.5)

* TensorFlow (>=r1.0)

* jieba (>=0.37)


## Usage


### * Training:

1. Prepare data at data/, including training data (example.train), validation data (example.dev), testing data (example.test), and Chinese character embedding data (vec.txt).

```
Current sample data includes 3 types of Named Entities, including ORG, PER and LOC
```

2. Training, models with best F1 score on validation data will be saved at ckpt/


To train with BILSTM+IDCNN+CRF (default), run:

```
#python3 main.py --train=True --clean=True --model_type=BI
```



### * Inference with command line input:

Following command will run your trained model at /ckpt

```
#python3 main.py
```
