<center>
  
---

🌳 **Sobre o Amazon Bark** 🌳

---
Amazon Bark é um conjunto de imagens de cascas (ritidoma) de árvores exploradas comercialmente para fins madeireiros na Amazônia brasileira. No total, o conjunto é constituido por 2.803 imagens de 16 espécies. Foram obtidas imagens de 10 árvores por espécie, com dois dispositivos: CANON e iOS iPhone 11, com resolução de 3024 x 4032 e 4000 x 5328, respectivamente. As imagens foram coletadas em 3 Áreas de Manejo Florestal (AMF), situados nos municípios de Nova Maringá, Feliz Natal e Cotriguaçu, Estado do Mato Grosso. Coletas botânicas foram realizadas em 5 árvores por espécie, com posterior montagem de exsicatas e envio para o Herbário Felisberto Camargo (HFC) da Universidade Federal Rural da Amazônia. 
---
|                 Espécies                  |  n   |
|:-----------------------------------------:|------|
|Apuleia leiocarpa (Vogel) J. F. Macbr.     | 01   |
|Astronium lecointei Ducke                  | 02   |
|Bagassa guianensis Aubl.                   | 03   |
|Bowdichia nitida Spruce ex Benth.          | 04   |
|Cedrela odorata L.                         | 05   |
|Dipteryx odorata (Aubl.) Forsyth f.        | 06   |
|Erisma uncinatum Warm.                     | 07   |
|Goupia glabra Aubl.                        | 08   |
|Hymenolobium petraueum Ducke               | 09   |
|Mezilaurus itauba (Meisn.) Taub. ex Mez    | 10   |
|Parkia pendula (Willd.) Benth. ex Walp.    | 11   |
|Protium acrense Daly                       | 12   |
|Qualea paraensis Ducke                     | 13   |
|Simarouba amara Aubl.                      | 14   |
|Trattinnickia burserifolia Mart.           | 15   |
|Vatairea sericea (Ducke) Ducke             | 16   |

</center>

---

Divisão de dados

Uma divisão estratificada foi realizada destinando 80% e 20% das imagens para treino e teste, respectivamente. A divisão matém a mesma proporção das classes (80% e 20%) dentro de cada conjunto. Para tanto, foi usada a biblioteca splitfolders. As divisões são construídas e salvas automaticamente no drive. Na sequência, foi realizada a extração de 50 patches de cada imagem, com dimensão de 256 x 256. Portanto, a quantidade de patches foi de 111.850 (treino) e 28.300 (teste), totalizando 140.150 patches extraídos das 2.803 imagens originais.

Extração de características

- Foram utilizadas variações do operador Padrão Binário Local (PBL) Uniforme, Invariante a Rotação e Não Invariante a Rotação;

- Quatro Redes Neurais Convolucionais pré-treinadas foram carregadas com pesos ImageNet: ResNet50, VGG16, InceptionV3 e MobileNetV2.

Classificação

- Quatro algoritmos de Machine Learning foram utilizados: Máquinas de Vetores de Suporte, Redes Neurais Artificiais, Floresta Aleatória e Análise Discriminante Linear.
---
