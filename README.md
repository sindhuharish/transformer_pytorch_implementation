### README ####

pip install -r requirements.txt with pyton = 3.6
if spacy doesnot load en and fr then explicity install 
* python -m spacy download en
* python -m spacy download fr

After training is complete the location to save weights is asked.

train script arguments - 
* python train.py -src_data
data/english.txt
-trg_data
data/french.txt
-src_lang
en
-trg_lang
fr

* python test.py -load_weights weight -src_lang en -trg_lang fr

if not using gpu and to train on cpu set - ('-no_cuda', action='store_false')
