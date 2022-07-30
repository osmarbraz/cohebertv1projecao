# Visualização dos Embeddings do Cohebert

Visualização dos embeddings do Cohebert gerados pelo BERTimbau utilizando o Embedding Projector.
https://projector.tensorflow.org/

Os arquivos utilizados pelo visualizados estão divididos em duas pastas: **"compooling"** e **"sempooling"**. Quem indicam se foi utilizado o pooling dos embeddings dos tokens das palavras fora do vocabulário.

## A pasta **"sempooling"** possui 4 versões dos cohebert com os embeddings dos tokens:
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 5 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector sem pooling através do arquivo config.json:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config.json

## A pasta **"compooling"** possui 4 versões do cohebert com os embeddings das palavras e sua POS-Tag:
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 4 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com pooling através do arquivo config_pool.json:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_pool.json

## Geração dos arquivos

Os arquivos utilizados pelo Embedding Projector foram gerados pelo notebook: https://github.com/osmarbraz/exemplos_BERT/blob/main/ExemplosVisualizacaoEmbeddingBERT_pt_br.ipynb.