# doc2vec
A simple example code in python:

    import gensim
    
    model_path = 'model.bin'    #directory of the model
    model = gensim.models.Doc2Vec.load(model_path)    #load the model
    
    text = 'please write down your name'    #text that you want to convert to vector, each element is one sentence, not case-sensitive
    vector = model.infer_vector(gensim.utils.simple_preprocess(text))    #convert
    
    print(vector)

Since [GitHub only accept files less than 100 MB to get pushed](https://help.github.com/articles/working-with-large-files/), I uploaded the model to [Mega](https://mega.nz/#!z8VwxCAY!0e_2lqRMjKQwGkqdE1jH130TZkspN9o_m1IHFWWkFJ8)

To use this, download the model from Mega and decompress it. There are several files and they are all necessary. But you only need to cover the directory of `model.bin` in your program, the model can find other files in the same folder.
