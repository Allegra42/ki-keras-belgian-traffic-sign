# ki-keras-belgian-traffic-sign

This project was created for the AI course at the University of Pforzheim in the Master's class Embedded Systems.
It's goal was to get in touch with artifical intelligence and neural networks based on the Belgian Traffic Sign Dataset.
Therefore, the [project report](https://github.com/Allegra42/ki-keras-belgian-traffic-sign/blob/master/report/Ausarbeitung_Anna-Lena_Marx.pdf)
as TeX and PDF is also a part of this repository.

## Setup project
The following instruction is based on using virtualenv.
All paths, used in the source code and documentation, are just written and tested for Linux. May you have to adjust them.

### Install requirements
```python
pip install -r requirements.txt
```

### Start training
It is assumed, the data is already downloaded and unpacked in `data`. If this is not the case, you can comment in the
call `download_data()` at the methode `setup_data()`. Do not forget to check if the paths are ok for your setup.
```python
python3 Keras.py
```

### Use the trained models
```python
python3 ClassifyImages.py -m <path/to/model> -i <path/to/pic>
```
Bear the format of the trainings pictures in mind. All models will just predict correct, if the image sections are simmilar 
to the ones, used for training.
