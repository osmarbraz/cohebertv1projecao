# Visualização dos Embeddings do Cohebert

Visualização dos embeddings das palavras de documentos originais **(DO)** e perturbados **(pertDO)** do **Cohebert** gerados pelo BERTimbau(Large e Base) utilizando o Embedding Projector (https://projector.tensorflow.org/).

Os arquivos utilizados pelo visualizador estão divididos em quatro pastas: **"compooling"** e **"sempooling"** para os arquivos do Cohebert. As pastas indicam se foi utilizado o pooling dos embeddings dos tokens das palavras fora do vocabulário ou não. E as pastas **faquad** e **squad2** para os arquivos do FaQuAD e SQuAD 2.0.

## A pasta **"compooling"** possui 4 versões dos DOs do Cohebert com os embeddings das palavras e sua POS-Tag:
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 4 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_pool.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_pool.json

## A pasta **"sempooling"** possui 4 versões dos DOs do Cohebert com os embeddings dos tokens:
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 5 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config.json

## A pasta **"compooling"** possui 1 versão dos DOs e pertDOs do Cohebert com os embeddings das palavras e sua POS-Tag:
- 1 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_pool_classe.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_pool_classe.json

## A pasta **"faquad"** possui 1 versão dos DOs do FaQuAD com os embeddings das palavras e sua POS-Tag:
- 1 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_faquad.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_faquad.json

## A pasta **"squad2"** possui 1 versão dos DOs do SQuAD 2.0 com os embeddings das palavras e sua POS-Tag:
- 1 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_squad2.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_squad2.json

## Notebook para geração dos arquivos tsv

Os arquivos utilizados pelo Embedding Projector foram gerados pelo notebook: https://github.com/osmarbraz/exemplos_BERT/blob/main/ExemplosVisualizacaoEmbeddingBERT_pt_br.ipynb.