# README: POC - Media Queries

## O que são Media Queries?

Media queries são uma técnica fundamental no desenvolvimento web responsivo, permitindo que os estilos CSS se adaptem a diferentes tamanhos de tela e condições de exibição. Elas permitem que você escreva regras de estilo que se aplicam apenas quando determinadas condições são atendidas, como a largura da tela, a altura, a orientação e a resolução.

## Por que usar Media Queries?

1. **Responsividade**: Garantem que seu site funcione bem em dispositivos de diferentes tamanhos, como smartphones, tablets e desktops.
2. **Experiência do Usuário**: Proporcionam uma melhor experiência ao usuário, ajustando o layout e o design para cada dispositivo.
3. **Melhorias de Performance**: Permitem carregar estilos específicos apenas quando necessário, otimizando o desempenho.

## Sintaxe Básica

A sintaxe de uma media query é simples. Aqui está um exemplo básico:

```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

Neste exemplo, a regra de estilo será aplicada quando a largura da tela for igual ou inferior a 600 pixels.

## Tipos Comuns de Media Queries

- **Largura e Altura da Tela**:
  - `max-width`: aplica estilos quando a largura é menor ou igual ao valor especificado.
  - `min-width`: aplica estilos quando a largura é maior ou igual ao valor especificado.

- **Orientação**:
  - `orientation: portrait`: para dispositivos em modo retrato.
  - `orientation: landscape`: para dispositivos em modo paisagem.

- **Resolução**:
  - `resolution`: para aplicar estilos dependendo da resolução da tela (por exemplo, telas de alta definição).

## Exemplos Práticos

### Exemplo 1: Estilos para Múltiplos Dispositivos

```css
/* Estilos padrão para desktops */
body {
  font-size: 16px;
}

/* Estilos para tablets */
@media (max-width: 900px) {
  body {
    font-size: 14px;
  }
}

/* Estilos para smartphones */
@media (max-width: 600px) {
  body {
    font-size: 12px;
  }
}
```

### Exemplo 2: Alterando Layout com Base na Orientação

```css
@media (orientation: portrait) {
  .container {
    flex-direction: column;
  }
}

@media (orientation: landscape) {
  .container {
    flex-direction: row;
  }
}
```

## Dicas para Uso Eficiente

1. **Mobile First**: Comece com estilos para dispositivos móveis e use media queries para aumentar a complexidade em telas maiores.
2. **Organização**: Mantenha suas media queries organizadas e próximas às regras de estilo que elas afetam.
3. **Teste em Vários Dispositivos**: Verifique como seu site se comporta em diferentes dispositivos e tamanhos de tela.

## Conclusão

Media queries são essenciais para criar layouts responsivos e adaptáveis. Ao utilizá-las corretamente, você melhora a experiência do usuário e garante que seu site funcione bem em uma variedade de dispositivos. Para mais informações, consulte a documentação oficial do CSS.
