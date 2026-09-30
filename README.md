# Computação Visual

## 1. Expectativa vs. Realidade na Disciplina

Minha ideia inicial sobre Computação Visual era de que focaríamos principalmente no estudo de recursos visuais digitais, renderização de imagens e criação de animações — semelhantes às utilizadas no desenvolvimento de jogos. 

---

## 2. A História e o Funcionamento do Sistema de Cores RGB

O **modelo de cores RGB** (*Red, Green, Blue*) é a base fundamental para a exibição de imagens em meios eletrônicos, como monitores, TVs e telas de smartphones. Trata-se de um sistema **aditivo**, no qual a junção das três luzes primárias em suas intensidades máximas resulta na cor branca.

* 📖 **Leitura:** [Artigo sobre o Modelo de Cores RGB (Wikipédia)](https://pt.wikipedia.org/wiki/RGB)
* 🎥 **Vídeo explicativo:** [Vídeo no YouTube](https://youtu.be/N1D6Lv6RYys)

---

## 3. A História e o Funcionamento do Algoritmo de Detecção de Bordas de Canny

Criado por John F. Canny em 1986, o detector de bordas de Canny é um dos algoritmos mais fundamentais e amplamente utilizados em computação visual. Ele identifica descontinuidades acentuadas de brilho em uma imagem para isolar contornos e estruturas relevantes, servindo como etapa inicial indispensável para tarefas como detecção de objetos, rastreamento e reconstrução 3D.

* 📖 **Leitura:** [Artigo sobre o Detector de Bordas de Canny (Wikipédia)](https://pt.wikipedia.org/wiki/Detector_de_bordas_de_Canny)
* 🎥 **Vídeo explicativo:** [Segmentação por bordas - Canny (YouTube)](https://www.youtube.com/watch?v=OsKz8YJ2jqE)

---

## 4. A História e o Funcionamento das Redes Neurais Convolucionais (CNNs)

As **Redes Neurais Convolucionais** (CNNs, do inglês *Convolutional Neural Networks*) são inspiradas no funcionamento do córtex visual dos animais, onde neurônios individuais respondem apenas a estímulos em regiões restritas do campo de visão — os chamados campos receptivos. É uma classe de rede neural artificial do tipo feed-forward, aplicada com sucesso no processamento e análise de imagens digitais, e hoje é um dos pilares da computação visual moderna, usada em tarefas como reconhecimento facial, classificação de objetos e segmentação de imagens.

Diferente das redes neurais tradicionais totalmente conectadas, a CNN usa a operação de **convolução** — filtros que percorrem a imagem capturando padrões locais (bordas, texturas, formas) — o que reduz drasticamente a quantidade de parâmetros a serem treinados e torna o processamento de imagens muito mais viável computacionalmente.

* 📖 **Leitura:** [Artigo sobre Rede Neural Convolucional (Wikipédia)](https://pt.wikipedia.org/wiki/Rede_neural_convolucional)
* 🎥 **Vídeo explicativo:** [O que são Redes Neurais Convolucionais? (YouTube)](https://www.youtube.com/watch?v=sgt_67zNDrI)

---

## 5. A História e o Funcionamento do Ray Tracing (Traçado de Raios)

O **Ray Tracing** é uma técnica de renderização que gera imagens simulando o caminho físico da luz em uma cena 3D. A ideia surgiu em 1968, quando Arthur Appel propôs lançar raios a partir do observador para determinar quais objetos são visíveis (*ray casting*). Em 1980, Turner Whitted ampliou o método com o **ray tracing recursivo**, permitindo calcular reflexos, refrações e sombras de forma realista. Por décadas, o custo computacional restringiu a técnica a filmes e animações renderizados offline, até que a Nvidia lançou em 2018 a família GeForce RTX 20, com núcleos dedicados (RT Cores), levando a técnica aos jogos em tempo real.

O funcionamento básico é o inverso do que ocorre na natureza: em vez de seguir a luz da fonte até o olho, o algoritmo lança um raio **da câmera através de cada pixel** da tela. Ao atingir um objeto, calcula-se a cor naquele ponto considerando as fontes de luz; se a superfície for reflexiva ou transparente, novos raios são disparados recursivamente. Diferente da **rasterização** — que projeta polígonos na tela e usa "truques" para simular iluminação —, o ray tracing produz naturalmente efeitos como reflexos de objetos fora da tela e sombras suaves, ao custo de muito mais processamento.

* 📖 **Leitura:** [Artigo sobre Ray Tracing (Wikipédia)](https://pt.wikipedia.org/wiki/Ray_tracing)
* 🎥 **Vídeo explicativo:** [O que é Ray Tracing? (YouTube)](https://www.youtube.com/results?search_query=o+que+%C3%A9+ray+tracing+como+funciona)

---