# Trabalho final 3d computação grafica

Este código cria uma cena 3D interativa com um cubo, uma esfera e um cilindro. Os objetos podem ser girados e movidos usando o mouse e o teclado. Além disso, os objetos mudam de cor ao passar o mouse sobre eles.

## Configuração Inicial

A primeira parte do código define a estrutura básica do documento HTML e carrega a biblioteca Three.js:

- O documento HTML define um elemento `<canvas>` para exibir a cena 3D.
- A biblioteca Three.js é carregada a partir de um CDN.

## Criação da Cena, Câmera e Renderizador

A próxima parte do código cria a cena, a câmera e o renderizador:

- A cena é onde os objetos 3D serão colocados.
- A câmera é usada para visualizar a cena.
- O renderizador é usado para renderizar a cena no canvas.

## Criação de Objetos 3D

A próxima parte do código cria três objetos 3D: um cubo vermelho, uma esfera verde e um cilindro azul:

- Cada objeto é criado usando uma geometria e um material diferentes.
- A geometria define a forma do objeto.
- O material define a cor e a aparência do objeto.

## Configuração de Iluminação

A próxima parte do código adiciona iluminação à cena:

- Uma luz ambiente suave é adicionada para fornecer uma luz geral à cena.
- Três luzes direcionais coloridas são adicionadas para fornecer luz mais focada.

## Configuração de Sombras

A próxima parte do código habilita a capacidade de gerar sombras no renderizador:

- O tipo de sombra é definido como THREE.PCFSoftShadowMap, que fornece sombras suaves.

## Animação

A próxima parte do código define uma função `animate()` que utiliza o `requestAnimationFrame` para criar uma animação contínua:

- A função `animate()` gira e anima em escala os objetos 3D com base no tempo.

## Interação do Mouse

A próxima parte do código registra um evento de movimento do mouse que atualiza a posição do mouse no espaço da cena:

- Um Raycaster é usado para verificar se o mouse está sobre algum dos objetos 3D.
- Quando o mouse passa sobre um objeto, a cor do material do objeto é alterada para vermelho.

## Interação do Teclado

A próxima parte do código registra um evento de pressionamento de tecla que move o objeto selecionado na direção especificada pelas setas do teclado.

## Iniciar a Animação

A função `animate()` é chamada para iniciar a animação após todas as configurações serem feitas.

