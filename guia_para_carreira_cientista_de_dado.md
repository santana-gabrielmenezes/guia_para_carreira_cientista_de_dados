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