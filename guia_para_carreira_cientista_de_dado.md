# 📚 Base de Conhecimento: Data Science

## 01. Python

Nesta seção, consolidamos os fundamentos da linguagem Python, desde sua definição e ambiente de desenvolvimento até a manipulação de variáveis, tipos de dados e operações matemáticas.

---

### 1.1 O que é Python? <a name="python-intro"></a>

Python é uma linguagem de **<span style="color:#2E86C1">alto nível</span>**, **<span style="color:#2E86C1">interpretada</span>** e **<span style="color:#2E86C1">orientada a objetos</span>**. Criada em 1989 por *Guido van Rossum*, consolidou-se como a ferramenta principal para Ciência de Dados devido à sua legibilidade e ao vasto ecossistema de bibliotecas.

##### 💡 Características Principais
* **Sintaxe Simples:** Curva de aprendizado suave, focada na produtividade.
* **Versatilidade:** Utilizada desde automação simples até modelos complexos de *Machine Learning*.
* **Multiplataforma:** Compatível com Windows, Linux e macOS.
* **Comunidade Ativa:** Grande disponibilidade de frameworks e suporte técnico.

##### 🧪 Por que para Data Science?
A linguagem é o padrão da indústria por sua eficiência em lidar com:
1.  **Grandes volumes de dados** (Big Data).
2.  **Operações matemáticas complexas.**
3.  **Integração facilitada** com ferramentas de visualização e bancos de dados.


> [!TIP]
> **Documentação Oficial:** [python.org](https://www.python.org/)

---

### 1.2 Ambiente de Desenvolvimento: Google Colab

Para praticar Ciência de Dados, utilizamos o **Google Colaboratory (Colab)**. Ele é um ambiente baseado em nuvem que permite a execução de código Python diretamente no navegador.

* **Zero Instalação:** Tudo roda nos servidores do Google.
* **Recursos Gratuitos:** Acesso a RAM e GPU.
* **Notebooks (`.ipynb`):** Documentos interativos que intercalam células de código, texto (Markdown) e visualizações.

##### ⌨️ Comandos e Execução
* **Executar Célula:** `Shift` + `Enter`.
* **Status do Ambiente:** Monitore o uso de **RAM** e **Disco** no canto superior direito.


---

### 1.3 Função `print()`

A função `print()` é utilizada para exibir informações no console ou na saída de uma célula. É a ferramenta básica para depuração e visualização de dados.

##### Exemplo de Uso
~~~python
# Exibindo uma mensagem de texto e um valor numérico
print("Olá, Data Science!")
print(10)
~~~

##### Retorno esperado:
~~~python
Olá, Data Science!
10
~~~

---

### 1.4 Comentários e Documentação

Comentários são anotações ignoradas pelo interpretador, essenciais para documentar a lógica do projeto.

* **Linha Única:** Utiliza-se o símbolo `#`.
* **Múltiplas Linhas:** Utilizam-se aspas triplas (`'''` ou `"""`).

##### Exemplo de Uso
~~~python
# Comentário de uma linha
print(10)

'''
Este é um comentário
de várias linhas.
'''
print("Python para Dados")
~~~

##### Retorno esperado:
~~~python
10
Python para Dados
~~~

---

### 1.5 Variáveis: Conceitos e Atribuição

Variáveis são nomes associados a valores armazenados na memória. Em Ciência de Dados, rotulam os dados que serão processados.

* **Atribuição:** Utiliza-se o operador `=`.
* **Mutabilidade:** O valor de uma variável pode ser alterado durante a execução.

##### Exemplo de Uso
~~~python
idade = 5
print(idade)

# Atualizando o valor
idade = 10
print(idade)
~~~

##### Retorno esperado:
~~~python
5
10
~~~

---

#### 1.5.1 Regras de Nomeação e Boas Práticas

* **Case Sensitivity:** Python diferencia maiúsculas de minúsculas (`idade` ≠ `IDADE`).
* **Snake Case:** Utilize underline para nomes compostos (ex: `nome_aluno`).
* **Restrições:** Não iniciar com números ou usar palavras reservadas (ex: `print`, `type`).

---

### 1.6 Tipos de Dados (Classes)

O Python organiza os dados em classes fundamentais. A função `type()` identifica a classe de uma variável.

| CLASSE | DESCRIÇÃO | EXEMPLO |
| :--- | :--- | :--- |
| **int** | Números inteiros. | `3`, `-5` |
| **float** | Números decimais (ponto flutuante). | `3.14`, `10.0` |
| **str** | Textos (*Strings*) entre aspas. | `'Olá'`, `"123"` |
| **bool** | Valores lógicos. | `True`, `False` |

##### Exemplo de Uso
~~~python
# Identificando tipos
media = 8.45
print(type(media))
~~~

##### Retorno esperado:
~~~python
<class 'float'>
~~~

---

### 1.7 Operações Aritméticas

Variáveis numéricas (`int` e `float`) podem ser manipuladas para cálculos aritméticos.

| Operação | Operador |
| :--- | :---: |
| Soma | `+` |
| Subtração | `-` |
| Multiplicação | `*` |
| Divisão | `/` |

##### Exemplo Prático: Média Ponderada
~~~python
# Cálculo utilizando precedência com parênteses
total_empregados = 5 + 16 + 1
media_salarial = (5*3000 + 16*6000 + 1*12500) / total_empregados
print(media_salarial)
~~~

##### Retorno esperado:
~~~python
5613.636363636364
~~~


> [!NOTE]
> **Precedência:** Multiplicação e divisão são executadas antes de soma e subtração. Utilize parênteses para forçar a ordem desejada.

#### 1.7.1 Operadores Aritméticos Complementares

Além das operações básicas, o Python dispõe de operadores para cálculos específicos como potência, resto e divisões inteiras.

| Operação | Operador | Descrição |
| :--- | :---: | :--- |
| **Exponenciação** | `**` | Eleva um número à potência definida. |
| **Módulo** | `%` | Retorna o resto de uma divisão entre dois números. |
| **Divisão Inteira** | `//` | Retorna apenas a parte inteira do resultado de uma divisão. |



---

1. Exponenciação (`**`)
Para realizar o cálculo, define-se a base à esquerda e o expoente à direita do operador.

##### Exemplo de Uso
~~~python
# Exemplo: 2 elevado a 3 (2 * 2 * 2)
operador = 2
potencia = 3
resultado = operador ** potencia
print(resultado)
~~~

##### Retorno esperado:
~~~python
8
~~~

---

2. Módulo (`%`)
Útil para identificar se um número é par ou ímpar, ou para encontrar o que sobra de uma divisão não exata.

##### Exemplo de Uso
~~~python
# Exemplo: Resto da divisão de 7 por 3
dividendo = 7
divisor = 3
print(dividendo % divisor)
~~~

##### Retorno esperado:
~~~python
1
~~~

---

3. Divisão Inteira (`//`)
Diferente da divisão comum (`/`), este operador descarta as casas decimais e retorna apenas o quociente inteiro.

##### Exemplo de Uso
~~~python
# Exemplo: Parte inteira de 7 dividido por 3
numerador = 7
denominador = 3
print(numerador // denominador)
~~~

##### Retorno esperado:
~~~python
2
~~~

### 1.8 Strings (Variáveis de Texto)

Além de dados numéricos, o Python permite a manipulação de textos através das **Strings**. Elas são sequências de caracteres que podem ser delimitadas tanto por aspas simples (`' '`) quanto por aspas duplas (`" "`).

##### Exemplo de Uso
~~~python
s1 = 'Alura'
s2 = "Alura"

# Verificando se os tipos são idênticos
print(type(s1), type(s2))
~~~

##### Retorno esperado:
~~~python
<class 'str'> <class 'str'>
~~~

---

### 1.9 Métodos

Métodos são funções associadas a objetos que permitem realizar ações, transformações ou obter informações sobre os dados. Em Data Science, o uso de métodos é constante para o tratamento e limpeza de dados brutos (*Data Cleaning*).

#### 1.9.1 Sintaxe de Uso
A estrutura básica consiste no nome do objeto, seguido de um ponto e o nome do método com parênteses: `objeto.metodo()`.



#### 1.9.2 Principais Métodos de Tratamento de Strings
Para exemplificar, utilizaremos o nome de uma professora que precisa de padronização para o cadastro da escola:

~~~python
texto = '  Geovana Alessandra dias Sanyos '
~~~

| Método | Descrição | Resultado Esperado |
| :--- | :--- | :--- |
| **`upper()`** | Converte todos os caracteres para maiúsculas. | `'  GEOVANA ALESSANDRA DIAS SANYOS '` |
| **`lower()`** | Converte todos os caracteres para minúsculas. | `'  geovana alessandra dias sanyos '` |
| **`strip()`** | Remove espaços em branco no início e no fim da string. | `'Geovana Alessandra dias Sanyos'` |
| **`replace(antigo, novo)`** | Substitui um caractere ou trecho por outro. | `'  Geovana Alessandra dias Santos '` |

---

#### 1.9.3 Atribuição e Acumulação de Métodos

É importante notar que os métodos de string retornam uma **cópia** do texto transformado; eles não alteram a variável original automaticamente. Para salvar as mudanças, devemos realizar uma nova atribuição.

O Python permite o **encadeamento de métodos** (acumulação), executando várias transformações em uma única linha de código.

##### Exemplo Prático: Padronização de Nome
~~~python
# Aplicando limpeza, correção de caracteres e conversão para maiúsculas
texto = '  Geovana Alessandra dias Sanyos '
texto = texto.strip().replace('y','t').upper()

print(texto)
~~~

##### Retorno esperado:
~~~python
GEOVANA ALESSANDRA DIAS SANTOS
~~~

> [!TIP]
> **Data Cleaning:** O encadeamento de métodos como `strip().replace().upper()` é uma técnica comum para garantir que nomes de categorias ou colunas em um conjunto de dados fiquem padronizados e sem erros de digitação antes da análise.

### 1.10 O Padrão Unicode e a Função `chr()`

O Python utiliza o padrão **Unicode** para codificação de caracteres, o que permite a representação consistente de textos em diversos idiomas, símbolos e emojis, independentemente da plataforma utilizada. Ao contrário do antigo padrão ASCII, limitado ao alfabeto inglês, o Unicode associa códigos numéricos a mais de 140 mil caracteres globais.



#### 1.10.1 A Função `chr()`

A função nativa `chr()` retorna a string correspondente ao código numérico especificado na tabela Unicode.

##### Exemplo de Uso
~~~python
# Imprimindo o caractere "@" (código 64)
print(chr(64))
~~~

##### Retorno esperado:
~~~python
@
~~~

---

#### 1.10.2 Concatenação de Strings

É possível unir múltiplas strings ou caracteres gerados pela função `chr()` utilizando o operador de soma `+`. Esse processo é conhecido como **concatenação**.

##### Exemplo de Uso
~~~python
# Construindo a palavra 'Olá' via códigos Unicode
palavra = chr(79) + chr(108) + chr(225) 
print(palavra)
~~~

##### Retorno esperado:
~~~python
Olá
~~~

> [!TIP]
> **Globalização de Dados:** Em Data Science, o suporte ao Unicode é fundamental para o processamento de textos (*Natural Language Processing*) de diferentes origens geográficas, garantindo que caracteres especiais como o "ç" ou o "ñ" não sejam corrompidos durante a análise.

### 1.11 Coleta e Conversão de Dados

Diferente de variáveis com valores pré-definidos, a coleta dinâmica permite que o código interaja com o usuário final para obter informações em tempo real.

#### 1.11.1 A Função `input()`

A função `input()` é a ferramenta responsável por interromper a execução do código e aguardar que o usuário insira uma informação via teclado. Ela retorna o conteúdo coletado como uma **string (texto)**.



##### Exemplo de Uso
~~~python
# Coletando e armazenando um nome
nome = input('Escreva seu nome: ')

# Exibindo o resultado
print(nome)
~~~

##### Retorno esperado:
~~~python
Escreva seu nome: Mirla
Mirla
~~~

---

#### 1.11.2 Funções de Conversão (Casting)

Como a função `input()` sempre retorna uma string, é necessário converter o dado caso queiramos realizar operações matemáticas ou lógicas. O Python oferece quatro funções principais para essa conversão:

| Função | Tipo de Destino | Descrição |
| :--- | :--- | :--- |
| **`int()`** | Inteiro | Converte para números sem casas decimais. |
| **`float()`** | Ponto Flutuante | Converte para números reais/decimais. |
| **`str()`** | String | Converte qualquer valor em texto. |
| **`bool()`** | Booleano | Converte para valores lógicos (True/False). |

##### Exemplo de Uso (Conversão Aninhada)
~~~python
# Coletando o ano de ingresso e convertendo imediatamente para inteiro
ano_entrada = int(input('Escreva o ano de ingresso do(a) estudante: '))

print(type(ano_entrada))
~~~

##### Retorno esperado:
~~~python
Escreva o ano de ingresso do(a) estudante: 2026
<class 'int'>
~~~

---

#### 1.11.3 Formatação de Saída com f-strings

As **f-strings** (formatted strings) permitem interpolar variáveis dentro de textos de forma elegante e legível, facilitando a apresentação de relatórios e resultados.



##### Exemplo Prático: Registro de Estudante
~~~python
# Coleta e conversão de dados
ano_entrada = int(input('Escreva o ano de ingresso: '))
nota_entrada = float(input('Digite a nota do teste de ingresso: '))

# Exibição formatada utilizando o prefixo 'f' antes das aspas
print(f'Ano de entrada {ano_entrada} - Nota do teste de ingresso {nota_entrada}')
~~~

##### Retorno esperado:
~~~python
Escreva o ano de ingresso: 2026
Digite a nota do teste de ingresso: 9.0
Ano de entrada 2026 - Nota do teste de ingresso 9.0
~~~

> [!IMPORTANT]
> **Boas Práticas:** Ao utilizar `input()`, sempre adicione um espaço após os "dois pontos (:)" na frase de solicitação. Isso evita que o cursor do usuário fique colado ao texto, melhorando a experiência de uso.

### 1.12 Formatação Avançada de Saída

Além das f-strings, o Python oferece métodos alternativos para interpolação de strings e o uso de caracteres especiais para controle de exibição no console. Como você tem interesse em estruturar documentações técnicas em Python, o domínio dessas formatações é essencial para a clareza dos outputs.

#### 1.12.1 Operador de Formatação (%)

Este operador funciona como um marcador (placeholder) que informa onde o valor da variável será exposto na string. Cada tipo de dado exige uma palavra-chave específica:

| Tipo de Variável | Palavra-chave |
| :--- | :---: |
| **String** | `%s` |
| **Inteiro** | `%d` |
| **Float** | `%f` |
| **Caractere** | `%c` |



##### Exemplo de Uso (Múltiplas Variáveis e Precisão)
~~~python
nome_aluno = 'Fabricio Daniel'
idade_aluno = 15
media_aluno = 8.45

# Usando %.2f para limitar a duas casas decimais
print('O aluno %s tem %d anos e média %.2f.' % (nome_aluno, idade_aluno, media_aluno))
~~~

##### Retorno esperado:
~~~python
O aluno Fabricio Daniel tem 15 anos e média 8.45.
~~~

> [!TIP]
> **Booleano com %:** Embora o `%s` aceite booleanos (convertendo-os internamente via `str()`), recomenda-se a conversão explícita para manter o código legível: `print("Valor: %s" % str(True))`.

---

#### 1.12.2 Método `.format()`

O método `.format()` é mais flexível que o operador `%`, utilizando chaves `{}` como marcadores. Ele não exige a especificação do tipo de dado (int, float, etc.) para a formatação básica.

##### Exemplo de Uso
~~~python
nome_aluno = 'Fabricio Daniel'
media_aluno = 8.45

print('Nome: {} - Média: {}'.format(nome_aluno, media_aluno))
~~~

##### Retorno esperado:
~~~python
Nome: Fabricio Daniel - Média: 8.45
~~~

---

#### 1.12.3 Caracteres Especiais (Escaping)

Caracteres especiais são sequências que representam ações (como quebras de linha) ou permitem imprimir símbolos reservados que o Python normalmente interpretaria como código.

| Caractere | Função | Descrição |
| :--- | :---: | :--- |
| **`\n`** | Nova Linha | Equivale a pressionar "Enter" no texto. |
| **`\t`** | Tabulação | Adiciona um recuo (espaço de tab) no texto. |
| **`\\`** | Barra Invertida | Permite imprimir uma barra invertida literal. |
| **`\"`** ou **`\'`** | Aspas | Permite imprimir aspas dentro de strings delimitadas pelo mesmo tipo de aspa. |



##### Exemplo de Uso (Tabulação e Quebra de Linha)
~~~python
print('Quantidade\tQualidade\n5 amostras\tAlta\n3 amostras\tBaixa')
~~~

##### Retorno esperado:
~~~python
Quantidade	Qualidade
5 amostras	Alta
3 amostras	Baixa
~~~

##### Exemplo de Uso (Aspas e Caminhos de Arquivo)
~~~python
# Imprimindo aspas internas e caminhos de diretório
print("Caminho: C:\\arquivos\\documento.csv")
print('Minha professora disse: \'Estudar é a chave do sucesso.\'')
~~~

##### Retorno esperado:
~~~python
Caminho: C:\arquivos\documento.csv
Minha professora disse: 'Estudar é a chave do sucesso.'
~~~

> [!IMPORTANT]
> **Recomendação:** Entre as três formas de formatação (f-string, `.format()` e `%`), a **f-string** é a preferida na comunidade de Ciência de Dados por ser mais legível, rápida e fácil de manter.

### 1.13 Estruturas Condicionais (if e else)

Em Ciência de Dados, as estruturas condicionais são fundamentais para resolver problemas de categorização e tomada de decisão lógica. Elas permitem que o programa execute diferentes blocos de instruções baseando-se em uma condição: se ela for verdadeira, uma instrução é rodada; se for falsa, executa-se um caminho alternativo.



#### 1.13.1 Lógica de Decisão

A estrutura condicional básica é composta por dois caminhos lógicos:
* **SE (if):** Verifica se uma condição é verdadeira para entrar no primeiro bloco de instruções.
* **SENÃO (else):** Define o que deve acontecer quando a condição inicial não é atendida (é falsa).

---

#### 1.13.2 Estudo de Caso: Categorização de Estudantes

Para automatizar a classificação de desempenho em uma instituição de ensino, utilizamos a média final (escala de 0.0 a 10.0) sob as seguintes condições:
* **Aprovação:** Média maior ou igual a 6.0.
* **Reprovação:** Média menor que 6.0.

##### Exemplo de Uso (Sintaxe Python)
~~~python
# Definindo a média para teste
media = 7.5

# Aplicando a estrutura condicional
if media >= 6.0:
    print("Estudante aprovado(a)")
else:
    print("Estudante reprovado(a)")
~~~

##### Retorno esperado:
~~~python
Estudante aprovado(a)
~~~

> [!IMPORTANT]
> **Indentação:** No Python, o espaço (recuo) antes das instruções dentro do `if` e do `else` é obrigatório. É essa organização visual que informa ao interpretador quais comandos pertencem a cada bloco de decisão.

#### 1.13.3 Sintaxe, Indentação e Fluxo de Execução

Diferente de outras linguagens que utilizam chaves, o Python utiliza a **indentação** (recuo de um "tab" ou 4 espaços) para definir o escopo de um bloco de instruções. A estrutura segue obrigatoriamente o padrão de palavra-chave (`if` ou `else`), condição e o uso de dois pontos (`:`) ao final da linha.



---

#### 1.13.4. Identificando Blocos de Instrução
Instruções identadas pertencem ao bloco condicional e só são executadas se a condição for atendida. Instruções sem recuo estão **fora do bloco** e serão executadas independentemente do resultado lógico do `if`.

##### Exemplo de Uso
~~~python
# Testando uma condição falsa
if 2 > 7:
    print('Este texto NÃO será exibido')
    
print('Fora do bloco: Este texto SEMPRE será exibido')
~~~

##### Retorno esperado:
~~~python
Fora do bloco: Este texto SEMPRE será exibido
~~~

---

#### 1.13.5. A Estrutura Complementar: `else`
O `else` (senão) atua como o caminho de saída quando a condição do `if` é falsa. Ele nunca possui uma condição própria e deve estar sempre alinhado verticalmente com o `if` correspondente.

##### Exemplo de Uso
~~~python
# Verificando se 2 é menor que 7
if 2 < 7:
    print('Condição verdadeira')
else:
    print('Condição falsa')
~~~

##### Retorno esperado:
~~~python
Condição verdadeira
~~~

> [!IMPORTANT]
> **Atenção ao Google Colab:** Ao pressionar "Enter" após os dois pontos (`:`), o ambiente realiza a indentação automática. Caso o recuo seja removido manualmente, o Python gerará um erro de sintaxe (`IndentationError`), impedindo a execução do código.

### 1.13.6 Condicionais em Cascata

Quando uma situação exige mais de duas saídas (ex: Aprovado, Recuperação e Reprovado), podemos utilizar um conjunto de `if`s em sequência para validar cada intervalo de valores separadamente. Nesta estrutura, o `else` não é obrigatório, pois cada `if` funciona como uma verificação independente.



##### Exemplo de Uso
~~~python
media = float(input('Digite a média: '))

# Condição 1: Aprovação
if media >= 6.0:
    print('Aprovado(a)')

# Condição 2: Recuperação (entre 4.0 e 6.0)
if 6.0 > media >= 4.0:
    print('Recuperação')

# Condição 3: Reprovação (abaixo de 4.0)
if media < 4.0:
    print('Reprovado(a)')
~~~

##### Retorno esperado (caso média 5.0):
~~~python
Digite a média: 5.0
Recuperação
~~~

---

### 1.13.7 O Problema da Associação do `else`

Um erro comum ao lidar com múltiplas condições é tentar finalizar uma sequência de `if`s independentes com um único `else`. No Python, o `else` se associa exclusivamente ao `if` imediatamente anterior a ele. 

Isso pode gerar resultados inconsistentes e saídas duplas, pois o programa pode validar o primeiro `if` como verdadeiro e, simultaneamente, executar o `else` do segundo bloco por este ter resultado em falso.

##### Exemplo de Erro Lógico
~~~python
media = float(input('Digite a média: '))

if media >= 6.0:
    print('Aprovado(a)') # Primeiro bloco independente

if 6.0 > media >= 4.0:
    print('Recuperação') # Segundo bloco associado ao else abaixo
else:
    print('Reprovado(a)')
~~~

##### Retorno esperado (Erro de lógica com média 7.0):
~~~python
Digite a média: 7.0
Aprovado(a)
Reprovado(a)
~~~

> [!CAUTION]
> **Risco de Saída Dupla:** No exemplo acima, como 7.0 é maior que 6.0, o primeiro `print` é executado. Porém, como 7.0 não está entre 4.0 e 6.0, a segunda condição é falsa, disparando o `else` associado e imprimindo também "Reprovado(a)". Para resolver este problema de forma elegante, utilizamos a estrutura `elif`, que será abordada na sequência.

### 1.13.8 A Estrutura `elif`

A palavra-chave `elif` é uma abreviação para "senão, se" (*else if*) e funciona como uma união entre o `else` e o `if`. Ela é utilizada para criar estruturas condicionais encadeadas, onde uma condição só é verificada se a condição superior a ela for falsa.

Diferente do `else`, o `elif` permite testar uma nova condição específica logo após um `if` que resultou em falso. A estrutura segue esta lógica:
1.  **`if`**: Verifica a primeira condição.
2.  **`elif`**: Só é avaliado se o `if` anterior for falso. Se sua própria condição for verdadeira, executa seu bloco de comando.
3.  **`else`**: Só é executado se todas as condições anteriores (`if` e todos os `elif`s) forem falsas.

> [!NOTE]
> **Escalabilidade:** É possível adicionar quantos blocos `elif` forem necessários entre o `if` e o `else`, não existindo uma limitação técnica, embora o excesso de encadeamento não seja considerado uma boa prática de programação.


Para resolver o problema das saídas duplas e do encadeamento ineficiente de múltiplos `if`s independentes, remodelamos a lógica de avaliação da instituição de ensino utilizando a estrutura `if-elif-else`.

##### Exemplo de Uso
~~~python
# Coleta da média e aplicação da estrutura integrada
media = float(input('Digite a média: '))

if media >= 6.0:
    print('Aprovado(a)')
elif 6.0 > media >= 4.0:
    print('Recuperação')
else:
    print('Reprovado(a)')
~~~

##### Retorno esperado
~~~python
Digite a média: 5.0
Recuperação
~~~

> [!TIP]
> **Eficiência Lógica:** Nesta estrutura, assim que o Python encontra uma condição verdadeira, ele executa o bloco correspondente e ignora o restante da cadeia. Isso garante que um estudante com média 7.0 receba apenas o status de "Aprovado(a)", sem disparar o bloco `else` por engano.

### 1.14 Operadores Relacionais

Uma condição no Python é fundamentada na comparação entre dados, resultando em um valor booleano (**True** ou **False**). Os operadores relacionais são as ferramentas que executam essas comparações para determinar o fluxo lógico do programa.



---

#### 1.14.1 Operadores de Magnitude (> e <)

Estes operadores verificam se um valor é estritamente maior ou menor que outro. Caso os valores sejam iguais, ambos retornarão **False**.

**1. Maior que (>)**
Retorna verdadeiro apenas se o valor à esquerda for superior ao da direita.

##### Exemplo de Uso
~~~python
idade_maria = int(input('Digite a idade da Maria: '))
idade_beatriz = int(input('Digite a idade da Beatriz: '))

if idade_maria > idade_beatriz:
    print('Maria é mais velha que Beatriz.')
~~~

##### Retorno esperado:
~~~python
Digite a idade da Maria: 12
Digite a idade da Beatriz: 10
Maria é mais velha que Beatriz
~~~

**2. Menor que (<)**
Retorna verdadeiro se o valor à esquerda for inferior ao da direita.

##### Exemplo de Uso
~~~python
idade_maria = int(input('Digite a idade da Maria: '))
idade_beatriz = int(input('Digite a idade da Beatriz: '))

if idade_maria < idade_beatriz:
    print('Maria é mais nova que Beatriz.')
~~~

##### Retorno esperado:
~~~python
Digite a idade da Maria: 30
Digite a idade da Beatriz: 34
Maria é mais nova que Beatriz
~~~

---

#### 1.14.2 Operadores de Limite (>= e <=)

Diferente dos anteriores, estes operadores incluem a igualdade na condição de verdade.

**1. Maior ou igual a (>=)**
Retorna verdadeiro se o valor à esquerda for maior ou exatamente igual ao da direita.

##### Exemplo de Uso
~~~python
emp_1 = int(input('Digite a quantidade de empregados da empresa 1: '))
emp_2 = int(input('Digite a quantidade de empregados da empresa 2: '))

if emp_1 >= emp_2:
    print('Empresa 1 tem uma quantidade de empregados maior ou igual à empresa 2.')
~~~

##### Retorno esperado:
~~~python
Digite a quantidade de empregados da empresa 1: 300
Digite a quantidade de empregados da empresa 2: 150
Empresa 1 tem uma quantidade de empregados maior ou igual à empresa 2
~~~

**2. Menor ou igual a (<=)**
Retorna verdadeiro se o valor à esquerda for menor ou igual ao da direita.

##### Exemplo de Uso
~~~python
emp_1 = int(input('Digite a quantidade de empregados da empresa 1: '))
emp_2 = int(input('Digite a quantidade de empregados da empresa 2: '))

if emp_1 <= emp_2:
    print('Empresa 1 tem uma quantidade de empregados menor ou igual à empresa 2.')
~~~

##### Retorno esperado:
~~~python
Digite a quantidade de empregados da empresa 1: 200
Digite a quantidade de empregados da empresa 2: 200
Empresa 1 tem uma quantidade de empregados menor ou igual à empresa 2
~~~

---

#### 1.14.3 Operadores de Identidade e Diferença (== e !=)

Estes operadores comparam se dois objetos são idênticos ou distintos, funcionando tanto para números quanto para strings.

**1. Igual a (==)**
Retorna verdadeiro se os valores forem idênticos.

##### Exemplo de Uso
~~~python
livro_1 = input('Digite o título do 1° livro: ')
livro_2 = input('Digite o título do 2° livro: ')

if livro_1 == livro_2:
    print('Os livros têm o mesmo título')
~~~

##### Retorno esperado:
~~~python
Digite o título do 1° livro: Verso e Código
Digite o título do 2° livro: Verso e Código
Os livros têm o mesmo título
~~~

**2. Diferente de (!=)**
É o inverso da igualdade; retorna verdadeiro se os valores não forem os mesmos.

##### Exemplo de Uso
~~~python
livro_1 = input('Digite o título do 1° livro: ')
livro_2 = input('Digite o título do 2° livro: ')

if livro_1 != livro_2:
    print('Os livros têm títulos diferentes')
~~~

##### Retorno esperado:
~~~python
Digite o título do 1° livro: Verso e Código
Digite o título do 2° livro: Programar com versos
Os livros têm títulos diferentes
~~~

> [!TIP]
> **Data Validation:** Em Ciência de Dados, o operador `!=` é amplamente usado para filtrar registros que não pertencem a uma determinada categoria ou para identificar anomalias em conjuntos de dados.

### 1.15 Operadores Lógicos e de Pertencimento

As **expressões lógicas** são construções fundamentais para solucionar problemas complexos em Ciência de Dados através da combinação de múltiplos critérios. Elas são compostas por dois elementos principais:
* **Operandos Lógicos:** Elementos comparados ou avaliados em uma expressão que resultam em `True` (verdadeiro) ou `False` (falso).
* **Operadores Lógicos:** Palavras-chave ou símbolos usados para combinar esses operandos em uma única instrução.



---

#### 1.15.1 Atribuição Múltipla

Antes de manipular expressões, é possível utilizar a **atribuição múltipla** para ligar diversas variáveis a um mesmo valor simultaneamente, o que facilita a inicialização de estados lógicos no código.

##### Exemplo de Uso
~~~python
# Atribuindo True a t1 e t2, e False a f1 e f2
t1 = t2 = True
f1 = f2 = False

print(f"t1: {t1}, f1: {f1}")
~~~

##### Retorno esperado
~~~python
t1: True, f1: False
~~~

---

#### 1.15.2 Operadores Lógicos (`and`, `or`, `not`)

Estes operadores definem como os valores booleanos interagem entre si para formar uma decisão lógica final.

| Operador | Regra de Funcionamento | Resultado |
| :--- | :--- | :--- |
| **`and`** | Exige que **todas** as entradas sejam verdadeiras. | `True` apenas se ambos os operandos forem `True`. |
| **`or`** | Exige que **pelo menos uma** entrada seja verdadeira. | `False` apenas se ambos os operandos forem `False`. |
| **`not`** | Realiza a **inversão** do resultado booleano. | Transforma `True` em `False` e vice-versa. |

**1. Operador `and` (E)**
##### Exemplo de Uso
~~~python
# O 'and' só retorna verdadeiro se ambas as entradas forem True
if t1 and f2:
    print('expressão verdadeira')
else:
    print('expressão falsa')
~~~

##### Retorno esperado
~~~python
expressão falsa
~~~

**2. Operador `or` (OU)**
##### Exemplo de Uso
~~~python
# O 'or' retorna verdadeiro se houver pelo menos uma entrada True
if t1 or f2:
    print('expressão verdadeira')
else:
    print('expressão falsa')
~~~

##### Retorno esperado
~~~python
expressão verdadeira
~~~

**3. Operador `not` (NÃO)**
##### Exemplo de Uso
~~~python
# O 'not' inverte o valor de t1 (que é True) para False
if not t1:
    print('expressão verdadeira')
else:
    print('expressão falsa')
~~~

##### Retorno esperado
~~~python
expressão falsa
~~~

---

#### 1.15.3 Operador de Pertencimento (`in`)

O operador `in` verifica se um determinado elemento está contido dentro de um conjunto ou sequência de elementos, como uma string ou uma lista. Se o elemento for encontrado, o resultado é `True`; caso contrário, é `False`.



##### Estudo de Caso: Busca em Lista de Aprovados
Na instituição de ensino, utilizamos o `in` para automatizar a verificação de nomes em listas extensas de estudantes aprovados.

##### Exemplo de Uso
~~~python
# Base de dados de estudantes
lista = 'José da Silva, Maria Oliveira, Pedro Martins, Ana Souza, Mariana Rodrigues'
nome_1 = 'Mariana Rodrigues'
nome_2 = 'Marcelo Nogueira'

# Verificando se Mariana Rodrigues está na lista
if nome_1 in lista:
    print(f'{nome_1} está na lista')
else:
    print(f'{nome_1} não está na lista')

# Verificando se Marcelo Nogueira está na lista
if nome_2 in lista:
    print(f'{nome_2} está na lista')
else:
    print(f'{nome_2} não está na lista')
~~~

##### Retorno esperado
~~~python
Mariana Rodrigues está na lista
Marcelo Nogueira não está na lista
~~~

> [!TIP]
> **Automação de Dados:** O uso do operador `in` é uma ferramenta poderosa para automatizar buscas em grandes volumes de texto, reduzindo o trabalho manual e a margem de erro em projetos de análise de dados.

#### 1.15.4 Operadores de Atribuição

Os operadores de atribuição têm como função principal definir ou atualizar o valor armazenado em uma variável. O operador mais básico e frequente no Python é o `=`, que realiza a atribuição direta e literal de um dado.



---

**1. Atribuição Composta**

Além da atribuição simples, o Python oferece operadores compostos que realizam uma operação aritmética e atualizam a variável no mesmo passo. Já utilizamos o operador de soma `+=` em nossos contadores para adicionar um valor específico ao conteúdo atual da variável.

##### Exemplo de Uso
~~~python
preco = 2.00
# Adicionando 3 ao valor atual (2.00 + 3)
preco += 3
print(preco)
~~~

##### Retorno esperado
~~~python
5.0
~~~

---

**2. Outros Operadores de Atualização**

Existem variações para todas as operações aritméticas básicas, permitindo alterar os valores das variáveis de forma concisa.

| Operador | Descrição | Exemplo | Lógica Equivalente |
| :--- | :--- | :--- | :--- |
| **`-=`** | Subtrai um valor da variável. | `preco -= 5` | $preco = preco - 5$ |
| **`*=`** | Multiplica a variável por um valor. | `preco *= 3` | $preco = preco * 3$ |
| **`/=`** | Divide a variável por um valor. | `preco /= 2` | $preco = preco / 2$ |
| **`//=`** | Realiza a divisão inteira da variável. | `preco //= 6` | $preco = preco // 6$ |
| **`%=`** | Atribui o resto da divisão à variável. | `preco %= 5` | $preco = preco \% 5$ |

##### Exemplo Prático: Desconto e Atualização
~~~python
estoque = 100
venda = 15

# Atualizando o estoque após uma venda (subtração)
estoque -= venda
print(f"Itens restantes: {estoque}")

# Aplicando um multiplicador de bônus
pontos = 10
pontos *= 2
print(f"Total de pontos: {pontos}")
~~~

##### Retorno esperado
~~~python
Itens restantes: 85
Total de pontos: 20
~~~

> [!TIP]
> **Eficiência de Código:** O uso de operadores como `+=` e `-=` torna o código mais limpo e reduz o risco de erros de digitação ao repetir o nome da variável em ambos os lados do sinal de igual.


#### 1.15.5 Tabela Verdade

Para construir expressões lógicas que resultem no comportamento esperado, é essencial compreender o funcionamento da **tabela verdade** de cada operador. Essas tabelas auxiliam na análise de algoritmos e na verificação da validade de expressões, mapeando todos os resultados possíveis para cada combinação de valores lógicos.



---

**1. Operador `and` (E)**

A lógica do operador `and` estabelece que a saída só será **Verdadeira (True)** se ambos os operandos forem simultaneamente verdadeiros. Caso qualquer uma das entradas seja falsa, o resultado final será **Falso (False)**.

| Operando 1 | Operando 2 | Resultado (`and`) |
| :--- | :--- | :--- |
| `False` | `False` | `False` |
| `False` | `True` | `False` |
| `True` | `False` | `False` |
| `True` | `True` | `True` |

---

**2. Operador `or` (OU)**

Diferente do anterior, o operador `or` retorna **Verdadeiro (True)** se pelo menos um dos operandos for verdadeiro. O resultado só será **Falso (False)** se ambas as entradas forem falsas.

| Operando 1 | Operando 2 | Resultado (`or`) |
| :--- | :--- | :--- |
| `False` | `False` | `False` |
| `False` | `True` | `True` |
| `True` | `False` | `True` |
| `True` | `True` | `True` |

---

**3. Operador `not` (NÃO)**

O operador `not` possui a tabela mais simples, pois atua sobre um único operando realizando a inversão do seu valor lógico.

| Operando | Resultado (`not`) |
| :--- | :--- |
| `True` | `False` |
| `False` | `True` |

> [!TIP]
> **Validação de Algoritmos:** Consultar a tabela verdade durante a fase de planejamento do código ajuda a evitar erros de lógica (bugs) em sistemas de decisão complexos, garantindo que todas as combinações de dados sejam tratadas corretamente.

### 1.16 Estruturas de Repetição

Até o momento, trabalhamos com execuções lineares de código. No entanto, em Ciência de Dados, frequentemente precisamos realizar a mesma tarefa para múltiplos registros (ex: processar notas de centenas de estudantes), o que torna a repetição manual inviável.

[Image comparing manual code repetition versus loop structure in programming]

---

#### 1.16.1 O Problema da Repetição Manual

Considere a tarefa de coletar duas notas de um estudante e calcular sua média. O bloco de código abaixo executa essa função com eficiência para uma única pessoa:

##### Exemplo de Uso (Um Estudante)
~~~python
# Coleta e cálculo imediato da média
nota_1 = float(input('Digite a 1° nota: '))
nota_2 = float(input('Digite a 2° nota: '))

print(f'Média: {(nota_1 + nota_2) / 2}')
~~~

##### Retorno esperado
~~~python
Digite a 1° nota: 5
Digite a 2° nota: 6
Média: 5.5
~~~

Caso precisemos realizar o mesmo cálculo para três estudantes, a solução imediata seria copiar e colar o bloco de código três vezes. Embora funcional para uma escala pequena, essa abordagem gera códigos extensos e de difícil manutenção.

##### Exemplo de Uso (Três Estudantes - Repetição Manual)
~~~python
# Repetição manual do bloco para 3 estudantes
nota_1 = float(input('Digite a 1° nota: '))
nota_2 = float(input('Digite a 2° nota: '))
print(f'Média: {(nota_1 + nota_2) / 2}')

nota_1 = float(input('Digite a 1° nota: '))
nota_2 = float(input('Digite a 2° nota: '))
print(f'Média: {(nota_1 + nota_2) / 2}')

nota_1 = float(input('Digite a 1° nota: '))
nota_2 = float(input('Digite a 2° nota: '))
print(f'Média: {(nota_1 + nota_2) / 2}')
~~~

---

#### 1.16.2 A Necessidade de Automação

Ao imaginarmos um cenário real com **100 estudantes**, a repetição manual deixaria de ser produtiva, cansativa e tornaria o código desnecessariamente gigantesco. É nesta situação que entram as **Estruturas de Repetição** (ou laços de repetição).

Estas estruturas são capazes de repetir um mesmo conjunto de comandos quantas vezes forem definidas. Em vez de escrever o código 100 vezes, colocamos o bloco dentro de um laço e instruímos o Python a executá-lo pelo número de vezes desejado, mantendo o código limpo e eficiente.



#### 1.16.3 Estruturas de Repetição no Python
Para construir laços de repetição, o Python utiliza duas palavras-chave principais:
* **`while`**: Executa a repetição enquanto uma condição específica for verdadeira.
* **`for`**: Geralmente utilizado para percorrer sequências ou repetir ações um número pré-determinado de vezes.

> [!TIP]
> **Data Science Tip:** O uso de loops é o primeiro passo para o processamento de grandes conjuntos de dados (Big Data), permitindo que um único algoritmo analise milhares de linhas de informação de forma automatizada e rápida.

#### 1.16.4 O Laço de Repetição `while`

O laço `while` (enquanto) é uma estrutura que repete um bloco de código enquanto uma determinada condição for verdadeira. Ele funciona de forma análoga a uma estrutura `if`, porém, em vez de executar o bloco apenas uma vez, ele retorna ao início da verificação após cada execução das instruções.



##### Sintaxe do `while`
~~~python
while condição:
# bloco de código que será repetido
~~~
As instruções dentro do laço devem estar obrigatoriamente tabuladas (indentadas) para que o Python compreenda que pertencem à repetição.

---

##### Exemplo Prático: Contador de 1 a 10

Para entender a execução, podemos criar um contador que exibe números sequenciais. Para isso, utilizamos uma variável de controle que é atualizada a cada ciclo.

##### Exemplo de Uso
~~~python
contador = 1
while contador <= 10:
    print(contador)
    # Incrementando a variável para atualizar o valor
    contador += 1
~~~

##### Retorno esperado
~~~python
1
2
3
4
5
6
7
8
9
10
~~~

> [!IMPORTANT]
> **Operador de Atribuição Composta:** A expressão `contador += 1` é uma forma simplificada em Python para escrever `contador = contador + 1`. Sem essa incrementação, a condição permaneceria verdadeira para sempre, gerando um **loop infinito** que travaria a execução do código.

---

##### Automação do Registro de Notas

Utilizando o `while`, podemos resolver o desafio de coletar médias para múltiplos estudantes sem duplicar linhas de código manualmente. Abaixo, o laço é configurado para rodar exatamente três vezes.

##### Exemplo de Uso
~~~python
# Inicializando o contador
contador = 1

while contador <= 3:
    nota_1 = float(input('Digite a 1° nota: '))
    nota_2 = float(input('Digite a 2° nota: '))

    print(f'Média: {(nota_1 + nota_2) / 2}')
        
    # Atualizando o contador para evitar loop infinito
    contador += 1
~~~

##### Retorno esperado (Simulação para 3 alunos)
~~~python
Digite a 1° nota: 5
Digite a 2° nota: 6
Média: 5.5
Digite a 1° nota: 7
Digite a 2° nota: 9
Média: 8.0
Digite a 1° nota: 4
Digite a 2° nota: 4
Média: 4.0
~~~

> [!TIP]
> **Fluxo de Dados:** Observe que o programa solicita as entradas sequencialmente. Assim que a média do primeiro aluno é exibida, o contador passa a valer 2, a condição `2 <= 3` é validada e o bloco reinicia automaticamente para o próximo estudante.

#### 1.16.5 O Laço de Repetição `for`

Diferente do `while`, o laço `for` não depende de uma condição lógica externa para ser executado. Ele funciona através da **iteração**, repetindo um bloco de código para cada elemento contido dentro de um conjunto de dados.



---

1. Sintaxe do `for`
A estrutura básica do `for` define uma variável temporária que assume o valor de cada item do conjunto, um por um, até que todos tenham sido processados.

~~~python
for elemento in conjunto:
    # bloco de código executado para cada elemento
~~~

* **`for`**: Traduzido como "para".
* **`elemento`**: Variável que recebe o valor do item atual da iteração.
* **`in`**: Operador que verifica a existência do elemento no conjunto.
* **Indentação**: Assim como no `while`, o bloco de código interno deve estar tabulado para ser lido corretamente.

---

##### A Função `range()`

Para criar contadores numéricos com o `for`, utilizamos a função `range()`, que gera uma sequência de números inteiros.

**Sintaxe:** `range(inicio, fim, passo)`
* **Início**: O valor onde a sequência começa.
* **Fim**: O limite da sequência (o valor definido é **exclusivo**, ou seja, a contagem para um número antes).
* **Passo**: O intervalo entre os números (o padrão é 1).

---

##### Exemplo Prático: Contador de 1 a 10

Utilizar o `for` com `range()` é mais produtivo do que o `while`, pois não exige a criação prévia da variável contadora nem a sua incrementação manual (`+= 1`), reduzindo o tamanho do código.

##### Exemplo de Uso
~~~python
# Criando uma sequência de 1 a 10 (o fim deve ser 11 pois é exclusivo)
for contador in range(1, 11):
    print(contador)
~~~

##### Retorno esperado
~~~python
1
2
3
4
5
6
7
8
9
10
~~~

---

##### Automação do Registro de Notas com `for`

Podemos remodelar o sistema de cadastro de notas da instituição de ensino para processar os dados de três alunos de forma automatizada e concisa.

##### Exemplo de Uso
~~~python
# O range(1, 4) executa o bloco para os valores 1, 2 e 3
for contador in range(1, 4):
    nota_1 = float(input('Digite a 1° nota: '))
    nota_2 = float(input('Digite a 2° nota: '))

    print(f'Média: {(nota_1 + nota_2) / 2}')
~~~

##### Retorno esperado (Simulação para 3 alunos)
~~~python
Digite a 1° nota: 4
Digite a 2° nota: 5
Média: 4.5
Digite a 1° nota: 6
Digite a 2° nota: 7
Média: 6.5
Digite a 1° nota: 5
Digite a 2° nota: 6
Média: 5.5
~~~

> [!TIP]
> **Iteração e Estruturas de Dados:** O laço `for` é a ferramenta ideal para trabalhar com conjuntos de elementos. Na próxima aula, veremos como utilizá-lo para percorrer **Estruturas de Dados**, o que permitirá análises ainda mais potentes em Ciência de Dados.

### 1.16.6 Comandos de Controle (`continue` e `break`)

Ao trabalharmos com laços de repetição (`for` e `while`), podemos controlar o fluxo de execução dentro do bloco de código, permitindo manipular como e quando as iterações devem ser processadas ou interrompidas. Os dois principais comandos para esse controle são o `continue` e o `break`.



---

1. O Comando `continue`

O comando `continue` interrompe apenas a iteração atual do laço e salta imediatamente para a próxima, retornando ao início da verificação do laço. Ele é útil para ignorar elementos específicos que não atendem a um critério sem parar o processamento dos demais.

##### Exemplo de Uso
~~~python
# Contagem de 1 a 5, pulando o número 4
for i in range(1, 6):
if i == 4:
continue
print(i)
~~~

##### Retorno esperado
~~~python
1
2
3
5
~~~

---

2. O Comando `break`

Diferente do anterior, o comando `break` interrompe a execução do laço completamente, saindo do bloco de código de repetição e seguindo para a próxima instrução fora dele. É amplamente utilizado para encerrar buscas ou parar execuções quando uma condição crítica é atingida.

##### Exemplo de Uso
~~~python
# Contagem de 1 a 5, interrompendo ao chegar no 4
for i in range(1, 6):
if i == 4:
    break
    print(i)
~~~

##### Retorno esperado
~~~python
1
2
3
~~~

---

3. Comparativo de Fluxo

A tabela abaixo resume como cada comando redireciona a execução do programa dentro de uma estrutura de repetição:

| Comando | Ação no Fluxo | Destino da Execução |
| :--- | :--- | :--- |
| **`continue`** | Interrompe a iteração atual. | Retorna ao início do laço (próxima iteração). |
| **`break`** | Interrompe o laço completamente. | Sai do bloco e vai para o código fora da estrutura. |

> [!TIP]
> **Eficiência em Dados:** O uso do `break` é essencial em Ciência de Dados ao realizar buscas em grandes volumes de informação; assim que o dado procurado é encontrado, o laço é encerrado, economizando tempo de processamento computacional.

## 02. Estruturas de Dados

Além dos tipos básicos (int, float, bool e str), o Python possui variáveis capazes de armazenar e agrupar diversos itens simultaneamente, funcionando como conjuntos de elementos. Essas variáveis são classificadas como **dados estruturados**.

---

### 2.1 Listas

As listas são um dos dados estruturados mais comuns e poderosos do Python. Elas armazenam diversos elementos em uma ordem específica e podem conter qualquer tipo de dado, inclusive misturando diferentes classes (como strings e números) em uma mesma estrutura.



#### 2.1.1 Criação de Listas
Uma lista é delimitada por **colchetes `[]`**, com seus itens separados por vírgulas.

##### Exemplo de Uso (Cadastro de Estudante)
~~~python
# Criando uma lista com: Nome, Nota 1, Nota 2, Nota 3 e Situação
lista = ['Fabricio Daniel', 9.5, 9.0, 8.0, True]

# Visualizando a lista
print(lista)
~~~

##### Retorno esperado
~~~python
['Fabricio Daniel', 9.5, 9.0, 8.0, True]
~~~

---

#### 2.1.2 Organização e Índices

Cada item em uma lista possui uma posição única chamada **índice**. O Python permite acessar esses elementos utilizando numeração positiva (do início ao fim) ou negativa (do fim para o início).

| Direção | Primeiro Item | Segundo | Terceiro | Quarto | Último |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Positiva** | `[0]` | `[1]` | `[2]` | `[3]` | `[4]` |
| **Elemento** | 'Fabricio Daniel' | 9.5 | 9.0 | 8.0 | True |
| **Negativa** | `[-5]` | `[-4]` | `[-3]` | `[-2]` | `[-1]` |



---

#### 2.1.3 Manipulação de Dados na Lista

Podemos coletar, atualizar ou realizar cálculos utilizando os índices dos elementos.

**1. Acessando Elementos**
~~~python
# Coletando o nome (índice 0) e a situação (índice -1)
print(lista[0])
print(lista[-1])
~~~

##### Retorno esperado
~~~python
Fabricio Daniel
True
~~~

**2. Atualizando Valores**
As listas são mutáveis, permitindo a substituição de valores através de uma nova atribuição ao índice desejado.

~~~python
# Atualizando a terceira nota (índice 3) de 8.0 para 10.0
lista[3] = 10.0
print(lista)
~~~

##### Retorno esperado
~~~python
['Fabricio Daniel', 9.5, 9.0, 10.0, True]
~~~

**3. Cálculos Dinâmicos**
~~~python
# Calculando a média utilizando os índices das notas
media = (lista[1] + lista[2] + lista[3]) / 3
print(media)
~~~

##### Retorno esperado
~~~python
9.5
~~~

---

#### 2.1.4 Leitura Dinâmica com `for`

Para listas extensas, utilizamos o laço `for` para percorrer (iterar) cada item de forma automática.

##### Exemplo de Uso
~~~python
# A variável 'elemento' assume o valor de cada item da lista em sequência
for elemento in lista:
    print(elemento)
~~~

##### Retorno esperado
~~~python
Fabricio Daniel
9.5
9.0
10.0
True
~~~

> [!TIP]
> **Data Science Insight:** As listas são fundamentais para organizar séries temporais ou conjuntos de variáveis independentes antes de serem processadas por modelos matemáticos. No próximo vídeo, exploraremos métodos avançados para manipulação de listas.

### 2.2 Strings

Embora as strings já tenham sido introduzidas como tipos básicos, elas funcionam como sequências ordenadas de caracteres (letras, números, espaços e símbolos). Apesar de compartilharem semelhanças com as listas, como a indexação, elas possuem comportamentos fundamentais distintos.



---

#### 2.2.1 Indexação e Imutabilidade

Cada caractere em uma string ocupa um índice que inicia em **0** e vai até a quantidade de caracteres menos 1. Assim como nas listas, é possível utilizar índices negativos para acessar elementos a partir do final.

No entanto, uma string é **imutável**: ao contrário das listas, não é possível alterar um caractere individual através de uma atribuição direta (`string[0] = 'a'`), o que resultaria em um erro de compilação.

##### Exemplo de Uso (Acesso via Índice)
~~~python
linguagem = 'Python'

# Acessando caracteres específicos
print(linguagem[0], linguagem[1], linguagem[2], linguagem[-3], linguagem[-2], linguagem[-1])
~~~

##### Retorno esperado
~~~python
P y t h o n
~~~

---

#### 2.2.2 Transformando Strings em Listas: Método `split()`

O método `split()` separa uma string em uma lista de substrings baseando-se em um delimitador especificado. Se nenhum delimitador for definido, o Python utiliza os espaços em branco como critério de separação.



##### Exemplo de Uso
~~~python
duvida = 'Quem veio antes? O ovo? Ou foi a serpente?'

# Separando pelo caractere '?'
lista_perguntas = duvida.split('?')
print(lista_perguntas)

# Separando por espaços (padrão)
lista_palavras = duvida.split()
print(lista_palavras)
~~~

##### Retorno esperado
~~~python
['Quem veio antes', ' O ovo', ' Ou foi a serpente', '']
['Quem', 'veio', 'antes?', 'O', 'ovo?', 'Ou', 'foi', 'a', 'serpente?']
~~~

---

#### 2.2.3 Transformando Listas em Strings: Método `join()`

O método `join()` realiza o processo inverso: ele une os elementos de uma lista para formar uma única string, utilizando um caractere unificador definido previamente.

##### Exemplo de Uso
~~~python
misturas = [
    'Tintas: vermelho, azul e amarelo',
    'Verde: mistura de azul e amarelo',
    'Laranja: mistura de vermelho e amarelo',
    'Roxo: mistura de vermelho e azul'
]

unificador = '. '
string_final = unificador.join(misturas)
print(string_final)
~~~

##### Retorno esperado
~~~python
Tintas: vermelho, azul e amarelo. Verde: mistura de azul e amarelo. Laranja: mistura de vermelho e amarelo. Roxo: mistura de vermelho e azul
~~~

> [!IMPORTANT]
> **Diferença Conceitual:** Uma **String** é representada por uma única variável contendo uma sequência de caracteres. Já uma **Estrutura de Dados** (como a Lista) é uma coleção que pode armazenar múltiplos itens de tipos variados em uma única variável.

### 2.3 Manipulação de Listas

As listas são ferramentas essenciais em Python pela sua capacidade de armazenar elementos de forma organizada e permitir o acesso rápido aos dados. Elas oferecem diversos métodos e funções nativas para manipular informações, como adicionar, remover e particionar dados conforme a necessidade do projeto de Ciência de Dados.



---

#### 2.3.1 Identificando a Quantidade de Elementos: `len()`

Para processar grandes volumes de informações sem a necessidade de contagem manual, utilizamos a função `len()`, que retorna o número total de itens presentes em um objeto iterável, como uma lista.

##### Exemplo de Uso
~~~python
# Utilizando a lista de cadastro: ['Fabricio Daniel', 9.5, 9.0, 10.0, True]
quantidade = len(lista)
print(quantidade)
~~~

##### Retorno esperado
~~~python
5
~~~

---

#### 2.3.2 Partição de Listas (Slicing)

A partição permite isolar fatias específicas de um conjunto de dados, o que é fundamental para dividir bancos de dados em partes menores. A sintaxe básica é `lista[inicio:fim]`, onde o índice de **início** é incluído e o índice de **fim** é o primeiro elemento a ser excluído da seleção.

| Sintaxe | Resultado |
| :--- | :--- |
| **`lista[1:4]`** | Seleciona do índice 1 até o 3 (as três notas). |
| **`lista[:3]`** | Seleciona do início até o índice 2. |
| **`lista[3:]`** | Seleciona do índice 3 até o final da lista. |
| **`lista[:]`** | Coleta todos os dados, do primeiro ao último. |

[Image explaining Python list slicing syntax with start and end parameters]

##### Exemplo de Uso
~~~python
# Extraindo apenas as três notas do estudante
notas_estudante = lista[1:4]
print(notas_estudante)
~~~

##### Retorno esperado
~~~python
[9.5, 9.0, 10.0]
~~~

---

#### 2.3.3 Adição de Elementos: `append()` vs `extend()`

Existem dois métodos principais para inserir novos dados ao final de uma lista, cada um com um comportamento específico de estruturação.

**1. Método `append()`**
Adiciona um **único elemento** ao final da lista. Se você passar uma lista para o `append()`, ela será inserida como um subelemento único (lista aninhada).

##### Exemplo de Uso
~~~python
# Adicionando a média (9.5) ao final da lista
lista.append(9.5)
print(lista)
~~~

**2. Método `extend()`**
Adiciona vários elementos de uma vez ao final da lista, desde que estejam contidos em um iterável. Diferente do `append()`, ele "desmembra" a nova lista e adiciona cada item como um elemento separado.

##### Exemplo de Uso
~~~python
# Adicionando três novas notas de uma vez
lista.extend([10.0, 8.0, 9.0])
print(lista)
~~~

##### Retorno esperado (Comparativo)
~~~python
# Com append(): [..., True, 9.5, [10.0, 8.0, 9.0]] -> Lista dentro de lista
# Com extend(): [..., True, 9.5, 10.0, 8.0, 9.0] -> Elementos individuais
~~~

---

#### 2.3.4 Remoção de Elementos: `remove()`

O método `remove()` permite excluir um item específico da lista informando o seu valor. Em Ciência de Dados, este método é útil para limpar informações indesejadas ou corrigir erros de inserção.

##### Exemplo de Uso
~~~python
# Removendo um elemento específico (ex: uma lista inserida por erro)
lista.remove([10.0, 8.0, 9.0])
print(lista)
~~~

##### Retorno esperado
~~~python
['Fabricio Daniel', 9.5, 9.0, 10.0, True, 9.5, 10.0, 8.0, 9.0]
~~~

> [!TIP]
> **Boas Práticas:** Utilize o `append()` para inclusões simples e o `extend()` para mesclar coleções de dados. Para remoções baseadas na posição (índice) em vez do valor, pesquise pelo método `pop()`.
