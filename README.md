# Laboratório de Computação Gráfica 3D

## 📌 Descrição

O projeto consiste no desenvolvimento de uma ferramenta interativa em **WebGL** para visualização e estudo de conceitos de Computação Gráfica, permitindo que o usuário manipule valores e observe graficamente os resultados no espaço tridimensional.

A proposta é reunir, em uma única aplicação, diferentes conteúdos abordados na disciplina, facilitando a associação entre os **cálculos matemáticos** e suas **representações gráficas em 3D**.

## 🛠️ Funcionalidades

- Visualização e manipulação de **vetores no espaço 3D**;
- Operações vetoriais:
  - Soma;
  - Subtração;
  - Multiplicação por escalar;
  - Produto escalar;
  - Produto vetorial;
- Exibição dos **cálculos e resultados** das operações;
- Explicação visual e textual de cada operação;
- Criação, edição e visualização de **matrizes**;
- Aplicação de **transformações geométricas 3D**:
  - Translação;
  - Rotação;
  - Escala;
- Criação de uma **matriz de composição** a partir de uma sequência de transformações;
- Visualização do efeito das transformações no espaço 3D;
- Controle interativo da câmera, permitindo **rotação e zoom**;
- Alteração de valores com atualização dos resultados em tempo real.

## ✅ Estado atual

O laboratório está funcional e reúne os módulos de **vetores**, **matrizes 3×3** e **transformações geométricas homogêneas 4×4** em uma única interface. Todas as visualizações geométricas são rasterizadas com WebGL nativo.

### Implementado

- [x] Visualização de vetores em 3D
- [x] Soma de vetores
- [x] Subtração de vetores
- [x] Multiplicação por escalar
- [x] Produto escalar
- [x] Produto vetorial
- [x] Visualização dos cálculos
- [x] Controle interativo da câmera
- [x] Criação e edição de matriz 3×3
- [x] Multiplicação de matriz por vetor 3D
- [x] Aba exclusiva para operações com matrizes
- [x] Soma, subtração e produto de matrizes
- [x] Matriz transposta e determinante
- [x] Visualização WebGL do efeito de uma transformação linear
- [x] Transformações de translação em X, Y e Z
- [x] Rotações configuráveis em torno dos eixos X, Y e Z
- [x] Escala independente nos três eixos
- [x] Matrizes homogêneas 4×4
- [x] Criação de sequências de transformações
- [x] Ativação, remoção e reordenação das etapas
- [x] Geração da matriz final de composição
- [x] Exibição das matrizes individuais e do cálculo resultante
- [x] Aplicação da composição a um ponto editável
- [x] Visualização WebGL do objeto original, etapas intermediárias e resultado final
- [x] Visualização dos eixos locais transformados
- [x] Atualização dos cálculos e da cena em tempo real

## 🧭 Como utilizar

Abra o arquivo `laboratorio_vetores_3d.html` em um navegador com suporte a WebGL.

- Na aba **Vetores**, escolha uma operação e altere as componentes dos vetores.
- Na aba **Matrizes**, edite as matrizes 3×3 ou utilize um dos presets disponíveis.
- Na aba **Transformações**, adicione translações, rotações e escalas à sequência.
- Use as setas para alterar a ordem, a caixa de seleção para desativar uma etapa e `×` para removê-la.
- Arraste sobre a cena para girar a câmera e use o scroll para controlar o zoom.

## 🧮 Convenção matemática

As transformações usam matrizes homogêneas 4×4 e vetores-coluna. As operações da lista são aplicadas de cima para baixo. Assim, para uma sequência escala → rotação → translação, a matriz final é:

```text
M = T × R × S
p' = M × p
```

Como a multiplicação matricial não é comutativa, alterar a ordem da lista pode alterar o resultado.

## 🎯 Objetivo

O projeto busca funcionar como um **laboratório visual e interativo**, auxiliando na compreensão prática dos conteúdos estudados em Computação Gráfica.

A ferramenta permite relacionar os conceitos matemáticos com suas representações visuais, tornando possível observar como **vetores, matrizes e transformações geométricas** se comportam no espaço tridimensional.

## 💻 Tecnologias

- **WebGL**
- **JavaScript**
- **HTML**
- **CSS**

Não são utilizadas bibliotecas gráficas externas: o canvas, os shaders e os buffers são configurados diretamente pela API WebGL.

