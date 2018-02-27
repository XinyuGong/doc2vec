# doc2vec
A simple example code in python:

    import gensim
    
    model_path = 'model.bin'    #directory of the model
    model = gensim.models.Doc2Vec.load(model_path)    #load the model
    
    #text that you want to convert to vector, each element is one sentence, not case-sensitive
    text = 'please write down your name'
    vector = model.infer_vector(gensim.utils.simple_preprocess(text))    #convert
    
    print(vector)

Since [GitHub accept files less than 100 MB to get pushed](https://help.github.com/articles/working-with-large-files/), I uploaded the model to [Mega]()

To use this, download the model from Mega and decompress it. There are several files and they are all necessary. But you only need to cover the directory of `model.bin` in your program, the model can find other files in the same folder.
