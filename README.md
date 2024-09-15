# Jogo do Número Secreto

Este projeto é um jogo simples em JavaScript chamado **"Jogo do Número Secreto"**, onde o objetivo é adivinhar um número aleatório entre 1 e 100. O jogador tem várias tentativas para acertar o número e o jogo fornece dicas se o número correto é maior ou menor do que o chute. Quando o jogador acerta, ele pode reiniciar o jogo.

## Estrutura do Projeto

O projeto é composto por três arquivos principais:

1. **index.html**: Contém o layout básico da página web.
2. **style.css**: Define o estilo visual da página.
3. **app.js**: Contém a lógica do jogo, como a geração de números aleatórios e o controle das tentativas.

### index.html
- Estrutura HTML principal com um formulário que permite ao jogador inserir um número.
- Inclui links para fontes do Google Fonts, uma biblioteca de voz (ResponsiveVoice.js) para feedback falado e o arquivo CSS de estilo.
- Dois botões principais:
  - **"Chutar"**: Para enviar a tentativa do número.
  - **"Novo jogo"**: Para reiniciar o jogo, desabilitado até que o jogador acerte o número.

### style.css
- Design responsivo com ajustes visuais para diferentes tamanhos de tela.
- Cores escuras de fundo com gradiente.
- Botões, fontes, e caixas de entrada estilizadas para uma interface moderna.
- Imagens de fundo com transparência e sombras para um efeito visual suave.

### app.js
- **Funções principais**:
  - `ExibirMensagemInicial()`: Exibe o título e as instruções do jogo.
  - `verificarChute()`: Verifica se o número digitado é o número correto. Se o jogador errar, uma dica é exibida (se o número é maior ou menor). Se acertar, uma mensagem de sucesso é exibida e o botão de reiniciar é habilitado.
  - `gerarNumeroAleatorio()`: Gera o número secreto aleatório e assegura que o mesmo número não seja repetido enquanto o jogo estiver ativo.
  - `limparCampo()`: Limpa o campo de entrada após cada tentativa.
  - `reiniciarJogo()`: Reseta o jogo com um novo número e desabilita o botão "Novo jogo" até que o jogador acerte o próximo número.

## Como Jogar

1. Digite um número entre 1 e 100 no campo de entrada.
2. Pressione o botão **Chutar** para verificar se acertou o número.
3. Se errar, uma dica será fornecida, indicando se o número secreto é maior ou menor.
4. Continue chutando até acertar o número.
5. Quando acertar, o botão **Novo jogo** será ativado, permitindo iniciar uma nova partida.

## Requisitos

- Um navegador moderno que suporte JavaScript, HTML5, e CSS3.
- Conexão com a internet para carregar as fontes e a biblioteca de voz.

## Personalização

- O valor do limite do número pode ser alterado modificando a variável `numeroLimite` no arquivo `app.js`.
- O design e a aparência podem ser ajustados no arquivo `style.css` conforme necessário.

## Executando o Projeto

Abra o arquivo `index.html` em um navegador para começar a jogar. O jogo funcionará localmente, sem necessidade de instalação ou dependências adicionais.

---

Este jogo é uma maneira simples e divertida de praticar JavaScript, manipulação de DOM e estilização CSS.
