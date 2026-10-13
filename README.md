## 6. Fotogrametria: Transformando Fotos em Modelos 3D

A **fotogrametria** é a técnica de reconstruir objetos e ambientes tridimensionais a partir de um conjunto de fotografias comuns. Basta fotografar um objeto (uma estátua, um prédio, até uma pessoa) de vários ângulos diferentes, e o computador consegue "deduzir" sua forma e textura, gerando um modelo 3D digital. Hoje ela é usada em jogos, efeitos visuais de filmes, preservação de patrimônio histórico, arqueologia, mapeamento com drones e até em aplicativos de celular que escaneiam objetos.

O processo combina várias ideias de computação visual:

1. **Detecção de pontos de interesse:** o algoritmo encontra pontos marcantes em cada foto (cantos, manchas, detalhes de textura), usando métodos como o **SIFT**.
2. **Correspondência entre imagens:** esses pontos são comparados entre as fotos para descobrir quais deles representam o mesmo ponto do objeto real.
3. **Structure from Motion (SfM):** com as correspondências, o sistema calcula ao mesmo tempo a posição de cada câmera e a posição 3D dos pontos, por triangulação — o mesmo princípio que nossos dois olhos usam para perceber profundidade.
4. **Nuvem de pontos e malha:** os pontos formam uma nuvem densa, que é convertida em uma malha de polígonos e recebe a textura extraída das próprias fotos.

Um detalhe curioso é que a técnica tem limitações bem visíveis: superfícies **transparentes, espelhadas ou sem textura** (como vidro, metal polido ou uma parede branca lisa) confundem o algoritmo, pois não há pontos distintos para comparar entre as imagens. Mais recentemente, técnicas baseadas em redes neurais, como **NeRF** (*Neural Radiance Fields*) e **Gaussian Splatting**, surgiram como evolução dessa ideia, conseguindo representar até reflexos e transparências com realismo impressionante.

* 📖 **Leitura:** [Artigo sobre Fotogrametria (Wikipédia)](https://pt.wikipedia.org/wiki/Fotogrametria)
* 🎥 **Vídeo explicativo:** [O que é Fotogrametria? (YouTube)](https://www.youtube.com/results?search_query=fotogrametria+como+funciona+modelo+3D)

---
