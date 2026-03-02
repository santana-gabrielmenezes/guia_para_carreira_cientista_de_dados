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

#### Exemplo Prático: Média Ponderada
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

### 1.7.1 Operadores Aritméticos Complementares

Além das operações básicas, o Python dispõe de operadores para cálculos específicos como potência, resto e divisões inteiras.

| Operação | Operador | Descrição |
| :--- | :---: | :--- |
| **Exponenciação** | `**` | Eleva um número à potência definida. |
| **Módulo** | `%` | Retorna o resto de uma divisão entre dois números. |
| **Divisão Inteira** | `//` | Retorna apenas a parte inteira do resultado de uma divisão. |



---

#### 1. Exponenciação (`**`)
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

#### 2. Módulo (`%`)
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

#### 3. Divisão Inteira (`//`)
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

