# Prova 2 - Módulo 6 💀

## Descrição

Esse repositório contém a entrega da parte prática da prova 2 do módulo 6 de Engenharia da Computação do Inteli em 2024. Nele, é possível encontrar um arquivo de Jupyter Notebook com um script para detecção de faces usando Haar Cascade, um vídeo que demonstra o output do script **E** este arquivo README.md com instruções básicas + **respostas às perguntas** que acompanham a atividade prática da prova.

## Execução

### Pré-requisitos

- Conta no Google 

### Passo a passo

1. Baixe o conteúdo desse repositório ou clone-o com o seguinte comando numa janela de terminal:

```bash
git clone https://github.com/RaiDeOliveira/p2m6.git
```

2. Abra o arquivo de Jupyter Notebook `p2m6.ipynb` no Google Colab

3. Na aba lateral esquerda do Google Colab, onde é possível fazer upload de arquivos, faça o upload do vídeo base `la_cabra.mp4`

4. Execute o Jupyter Notebook

5. Ao fim da execução, um arquivo de vídeo `video.avi` será gerado na mesma aba lateral, contando com a identificação das faces marcadas por retângulos azuis.

## Perguntas

### 2.1

**Descreva de maneira concisa (um parágrafo no máximo) o funcionamento do método de detecção escolhido.**

O método de detecção escolhido foi o Haar Cascade e ele funciona de modo que, em cascata, vários retângulos preto com partes em preto e branco são sobrepostos pela área de uma imagem para calcular a diferença de intensidade entre partes escuras e claras de diferentes regiões dos pixels. Com base nessas diferenças, é possível treinar o modelo para identificar determinados objetos.

### 2.2

**Considere as seguintes alternativas para resolver o problema de detecção de faces:**

>    HAAR Cascade
>    CNN
>    NN Linear
>    Filtros de correlação cruzada

**Classifique-os (coloque em ordem) em termos de viabilidade técnica (se é possível resolver o problema), facilidade de implementação e versatilidade da solução. Justifique sua classificação.**

Ordem (1 = mais viável, 2 = menos viável):

1 - HAAR Cascade (implementação simples e funcionamento rápido)
2 - NN Linear (implementação simples)
3 - CNN (implementação mais robusta, funcionamento menos rápido)
4 - Filtros de correlação cruzada (implementação mais robusta, funcionamento menos rápido, não compensa para o problema simples)

### 2.3

**Considerando as mesmas alternativas acima, faça uma nova classificação considerando a viabilidade técnica para detecção de emoções através da imagem de uma face.**

Ordem (1 = mais viável, 2 = menos viável):

1 - CNN (é possível criar vários nós de output para cada emoção)
2 - HAAR Cascade (implementação simples, treinamento demorado)
3 - Filtros de correlação cruzada 
4 - NN Linear (não tem a complexidade necessária para resolver o problema de maneira ótima)

### 2.4

**A solução apresentada ou qualquer outra das que foram listadas na questão 2.2. tem a capacidade de considerar variações de um frame para outro (e.g. perceber que em um frame a pessoa está feliz e isso influenciar na detecção do próximo frame)? Se não, quais alterações poderiam ser feitas para que isso seja possível?**

A solução apresentada e as demais listadas na questão 2.2 não tem capacidade de considerar essas variações. Contudo, isso pode ser possível caso os modelos sejam treinados para tal. Além disso, numa implementação usando rede neural, por exemplo, pode haver diferentes nós de output para cada emoção, permitindo essa diferenciação a cada frame. 

### 2.5

**Quem ganha a bola de ouro 2024?**

