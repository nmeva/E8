# Assignment 1 (100 points):
### * Change the languages from german<>english to french<>german *or* change g<>e to english<> german
The following code has been changed.
 * French Raw Data is not availabe in Git, Hence Interchanging German to English to English to German as below
``` python
# SRC is changed to en and TRG to de
SRC = Field(tokenize = tokenize_en, 
            init_token = '<sos>', 
            eos_token = '<eos>', 
            lower = True)

TRG = Field(tokenize = tokenize_de, 
            init_token = '<sos>', 
            eos_token = '<eos>', 
            lower = True)
            
# exts are interchanged as below
train_data, valid_data, test_data = Multi30k.splits(exts = ('.en', '.de'), 
                                                    fields = (SRC, TRG))
                                                    
                                                    
```
### * Change the model such that it has 3 layers instead of 2

The variable N_LAYERS is updated to 3.

``` python
N_LAYERS = 3
```
### * Train the model on Colab, upload to Github and share the link

Kindly refer to this [file](https://github.com/nmeva/E8/blob/main/END_S8_Assignment_PartA.ipynb)



# Assignment 2 (900 points):

### Write 100 Python programs and upload the file to github and share another link on the LMS.

Kindly refer to this [file](https://github.com/nmeva/E8/blob/main/S8_100_python.ipynb)
