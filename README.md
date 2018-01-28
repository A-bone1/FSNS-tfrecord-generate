# FSNS-tfrecord-generate


Recently I would like to build a Chinese OCR based on Google Attention ocr and found that if you want to train your own model, you need to generate FSNS format tfrecord yourself, but Google officials did not say in this part carefully, only to a [stackoverflow link](https://stackoverflow.com/a/44461910/743658), but This link is also not clear,and have  some mistakes, so I wrote a code to generate FSNS format (JPG / PNG) tfrecord .
The format of FSNS said in this [paper](https://arxiv.org/pdf/1702.03970.pdf)

## We only need to care about this figure.
![image](https://github.com/A-bone1/FSNS-tfrecord-generate/blob/master/images/FSNS_format.jpg)



## How to generate your own FSNS tfrecord data

You need to do three steps:

The first step is to create a dictionary that matches your own text label, such as [dic.txt](https://github.com/A-bone1/FSNS-tfrecord-generate/blob/master/dic.txt). 

The second step is to place the pictures and text you need to generate under / data,

The third step is to generate your tfrecord by
```
python generate_tfrecord_JPG.py

```
or

```
python generate_tfrecord_PNG.py
```
