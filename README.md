# Visualização dos Embeddings do Cohebert v1

Visualização dos embeddings do Cohebert utilizando BERTimbau.

https://projector.tensorflow.org/

Possui 4 versões dos embeddings do cohebert sem pooling dos tokens:
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 5 - Concatenação das 4 últimas camadas do BERTimbau large

Link para o Embedding Projector sem pooling:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config.json


Possui 3 versões dos embeddings do cohebert com pooling média dos embeddings dos tokens de palavras fora do vocabulário:
- 1 - Última camada do BERTimbau base
- 2 - Última camada do BERTimbau large
- 3 - Concatenação das 4 últimas camadas do BERTimbau base
- 4 - Concatenação das 4 últimas camadas do BERTimbau large

Link para o Embedding Projector com pooling:
https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/osmarbraz/cohebertv1visualizacao/main/config_pool.json
