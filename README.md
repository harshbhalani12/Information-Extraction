# Information-Extraction

**Description:** We implemented Information Extraction application using NLP features and pipeline for converting unstructured data to stuctured data based on the templates.
The domain for this project is related to **Movie information**.

**Features:** It will take sentences as input and fill the appropriate templates based on the given appeared word in the sentence.

For example, our templates are : 

            - Release (product, location, date, owner, format)
            - PromotionalEvent (Movie, Event, Location, Date)
            
The input sentence is **"Black Panther premiered in Los Angeles on January 29, 2018, and
was released theatrically in the United States on February 16, in 2D, 3D, IMAX
and other premium large formats."**

Then, the output will be: 

          - Release (Black Panther, United States, Febuary 16, Owner<no-match>, [2D, 3D, IMAX])
          - PromotionalEvent (Black Pantherm, Los Angeles, January 29, 2018 , Owner<no-match>, format<no-match>)
          
**Technology used:**

           - Python
           - spacy library for Named Entity Recogntion, depeency parsing, sentence tokenization, lemmatization
