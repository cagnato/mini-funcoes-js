# mini-funcoes-js

Objetivo

Esta aplicação demonstra o uso de funções em JavaScript — nomeadas, anônimas e arrow functions — em operações matemáticas e manipulação de arrays.
Foi desenvolvida para a entrega do tde 1 de Desenvolvimento Web, evidenciando também o uso de funções de callback e integração com HTML e CSS.

-----------------------------------------------------------------------------------------------------------------

***1. Funções Nomeadas***

Funções clássicas que realizam as quatro operações básicas:

function soma(a, b){ return a + b }
function subtracao(a, b){ return a - b }
function multiplicacao(a, b){ return a * b }
function divisao(a, b){ return b === 0 ? "Erro: divisão por zero!" : a / b }


Uso: chamadas diretamente pelos botões da seção “Operações Matemáticas”.

***2. Funções Arrow (Anônimas)***

Usadas para manipular arrays:

const filtrarPares = arr => arr.filter(n => n % 2 === 0)
const media = arr => arr.length ? arr.reduce((acc, v) => acc + v, 0) / arr.length : NaN
const transformar = arr => arr.map(x => x*x + 1)


Uso:

filtrarPares() retorna apenas números pares.

media() calcula a média dos números filtrados.

transformar() aplica uma transformação a cada elemento (x² + 1).

Essas funções são chamadas pelos botões da seção “Manipulação de Array”.

***3. Função com Callback***

Demonstra a passagem de uma função como parâmetro:

function calcularComCallback(a, b, operacao){
  return operacao(a, b)
}


Uso:
Permite que qualquer função (por exemplo, soma, subtracao, ou mesmo uma função anônima inline, como (x, y) => x ** y para potenciação) seja passada como argumento.

---------------------------------------------------------------------------------------------------------------------

***Tecnologias Utilizadas***

HTML5: estrutura e interface.

CSS3: estilização e layout responsivo.

JavaScript (ES6): lógica, manipulação de eventos e funções.

---------------------------------------------------------------------------------------------------------------------

***Conceitos Demonstrados***

Funções nomeadas e reutilizáveis.

Arrow functions (funções anônimas).

Passagem de funções como parâmetros (callback).

Manipulação de arrays com filter, reduce e map.

Interação com DOM e eventos (addEventListener).

---------------------------------------------------------------------------------------------------------------------

***Execução***

Clonar ou baixar o repositório.

Abrir o arquivo index.html no navegador.

Testar as operações matemáticas e manipulação de arrays diretamente na interface.
