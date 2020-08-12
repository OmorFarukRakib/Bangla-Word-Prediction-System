In this folder we have all the codes to build our system.

We have divided our work into three part.

# Part_ONE

In the part ONE we loaded and cleaned our dataset to remove all the unwanted words and characters. Then we determined and gathered all the unique words and gave each of them a unique value which we called token. So each of the unique words now has a unique token value. 
There are 5 Part_One file. In the Part_One_1_1 we broke-down our whole dataset into 1-Gram language model. which means there are 2 words in one line where the first one is input and the last one is output thus predicted next word.
We also repeated the process for Part_One_2_1 for 2-Gram (2 inputs and 1 output), Part_One_3_1 (3 inputs and 1 output) upto Part_One_5_1 for 5-Gram data model.
We then saved the n-gram dataset and the corresponding tokenizer.

# Part_TWO

In this part we loaded the tokenizer and N-gram dataset from the previous code and tried to implement our algorithm. First we tried to detect if there were any errors in the dataset that we created. For example if there were any lines where the n-gram didnt constructed. If we had found any line that had problems, we simply deleted that line. When our data was ready to train we used our created model **(see our paper to better understand of our model)** and trained our datasets.

***N.B: In some Part_two code, you may find memory error while running and even in my codes have memory error. Its because my machine wasn't able to train/split this huge dataset. I then train my model into google colab. Its free and super fast with a lot of memory and GPU support. I created my models through Google colab and then save these models for further usage.***

Part_Two has 5 files for each of the n-Grams.

# Part_THREE

In this part I loaded my tokenizer and the model that i have created earlier using google colab or locally, and then constructed a function which takes a word and generate/predict the next word using my model.
I only have one Part_Three and i have loaded all the model from 1-Gram to 5-Gram and through checking the length i have passed the input value to the function and use corresponding models to generate next word.

# Part_THREE_GUI

This was used to create a GUI to see our work in action. You can see the created and working interface in the main README file.
