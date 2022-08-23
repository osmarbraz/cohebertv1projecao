# Visualização de Embeddings

Visualização de embeddings gerados pelo BERTimbau utilizando a ferramenta Embedding Projector (https://projector.tensorflow.org/).

Os arquivos utilizados pelo visualizador estão divididos em quatro pastas: **"compooling"** e **"sempooling"** para os arquivos do **Cohebert**. As pastas indicam se foi utilizado o pooling dos embeddings dos tokens das palavras fora do vocabulário ou não. E as pastas **faquad** e **squad2** para os arquivos da visualização dos embeddings do **FaQuAD** e **SQuAD 2.0.**.

As projeções podem utilizar os seguintes **metadados**:
- Token
- POS-Tag (Somente para pooling)
- OOV (0 - Existe no vocabulário do BERT, 1 - Não existe no vocabulário do BERT e combinado os embeddings tokens)
- Sentence

## A pasta **"compooling"** possui 4 versões dos DOs do Cohebert com pooling dos embeddings dos tokens de palavras fora do vocabulário(com PoS-Tag):
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 4 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_pool.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_pool.json

## A pasta **"sempooling"** possui 4 versões dos DOs do Cohebert sem pooling(sem PoS-Tag):
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 5 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config.json

## A pasta **"compooling"** possui 1 versão dos DOs e 1 versão perturbada(pertDO) rotulados do Cohebert e com pooling dos embeddings de tokens de palavras fora do vocabulário do BERT:
- 1 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_pool_classe.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_pool_classe.json

## A pasta **"sentenca"** possui 3 versões dos DOs e suas 20 versões perturbadas(pertDOs):
- 1 - Média dos embeddings dos tokens da senteça da última camada do BERTimbau large
- 2 - Média dos embeddings dos tokens da sentença da 4 últimas camadas do BERTimbau large
- 3 - Embeddings do token [CLS] da última camada do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_sentenca.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_sentenca.json


## Notebook para geração dos arquivos tsv
Os arquivos utilizados pelo Embedding Projector foram gerados pelo notebook: https://github.com/osmarbraz/exemplos_BERT/blob/main/ExemplosVisualizacaoEmbeddingBERT_pt_br.ipynb.

## Arquivos tsv grandes
Os arquivo tsv maiores que 50Gb devem usar o *Git Large File Storage* **(Git LFS)**. O caminho de arquivos armazenados com Git LFS são diferentes dos armazenados no Git.
