# doc2vec
A simple example code in python:

    import gensim
    
    model_path = 'model.bin'    #directory of the model
    model = gensim.models.Doc2Vec.load(model_path)    #load the model
    
    #text that you want to convert to vector, each element is one sentence, not case-sensitive
    text = 'please write down your name'
    vector = model.infer_vector(gensim.utils.simple_preprocess(text))    #convert
    
    print(vector)
