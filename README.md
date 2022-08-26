# Visualização de Embeddings

Visualização de embeddings gerados pelo BERTimbau utilizando a ferramenta Embedding Projector (https://projector.tensorflow.org/).

Os arquivos utilizados pelo visualizador estão divididos em duas pastas: **"token"** e **"sentence"** para os arquivos do **Cohebert**. As pastas indicam se foi utilizado o embeddings de tokens das sentenças ou embeddings consolidados das sentenças. 
A pasta **"token"** contêm os arquivos para a visualização dos embeddings dos tokens das sentenças.
A pasta **"sentence"** contêm os arquivos para a visualização dos embeddings consolidados dos tokens das sentenças.

## Projeção dos embeddings de tokens

As projeções dos embeddings de tokens podem se relacionar os seguintes **metadados**:
- Token
- POS-Tag (Somente para pooling)
- OOV (0 - Existe no vocabulário do BERT, 1 - Não existe no vocabulário do BERT e combinado os embeddings tokens)
- Sentence

Os arquivos dos embeddings de tokens estão divididos em duas pastas **"compooling"**, **"sempooling"** e **"do_pertdo_pooling"** .

### A pasta **"compooling"** possui 4 versões dos DOs do Cohebert com pooling dos embeddings dos tokens de palavras fora do vocabulário(com PoS-Tag):
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 4 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_token_pool.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_token_pool.json

### A pasta **"sempooling"** possui 4 versões dos DOs do Cohebert sem pooling(sem PoS-Tag):
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 4 - Concatenação das 4 últimas camadas do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_token.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_token.json

### Notebook para geração dos arquivos tsv para visualização dos embeddings de tokens
 
Os arquivos utilizados pelo Embedding Projector foram gerados pelo notebook: https://github.com/osmarbraz/exemplos_BERT/blob/main/ExemplosVisualizacaoEmbeddingTokenBERT_pt_br.ipynb.

## Projeção dos embeddings de sentenças

As projeções dos embeddings de sentenças podem se relacionar com os seguintes **metadados**:
- Sentença
- Classe (0 - Original e 1 - Perturbado)

### A pasta **"sentence"** possui 4 versões dos DOs do Cohebert:
- 1 - Média dos embeddings dos tokens da sentença das 4 últimas camadas do BERTimbau base
- 2 - Média dos embeddings dos tokens da sentença das 4 últimas camadas do BERTimbau large
- 3 - Embeddings do token [CLS] da última camada do BERTimbau base
- 4 - Embeddings do token [CLS] da última camada do BERTimbau large

**Link** para o Embedding Projector com o arquivo *config_sentenca.json* e as referências aos dados:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_sentence.json

### Notebook para geração dos arquivos tsv para visualização dos embeddings de sentenças
 
Os arquivos utilizados pelo Embedding Projector foram gerados pelo notebook: https://github.com/osmarbraz/exemplos_BERT/blob/main/ExemplosVisualizacaoEmbeddingSentencaBERT_pt_br.ipynb.

## Arquivos tsv grandes
Os arquivo tsv maiores que 50Gb devem usar o *Git Large File Storage* **(Git LFS)**. O caminho de arquivos armazenados com Git LFS são diferentes dos armazenados no Git.
