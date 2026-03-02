# 📚 Base de Conhecimento: Data Science

## 01. Primeiros Passos em Python

### 1.1 O que é Python? <a name="python-intro"></a>

Python é uma linguagem de **<span style="color:#2E86C1">alto nível</span>**, **<span style="color:#2E86C1">interpretada</span>** e **<span style="color:#2E86C1">orientada a objetos</span>**. Criada em 1989 por *Guido van Rossum*, consolidou-se como a ferramenta principal para Ciência de Dados devido à sua legibilidade e ao vasto ecossistema de bibliotecas.

#### 💡 Características Principais
* **Sintaxe Simples:** Curva de aprendizado suave, focada na produtividade.
* **Versatilidade:** Utilizada desde automação simples até modelos complexos de *Machine Learning*.
* **Multiplataforma:** Compatível com Windows, Linux e macOS.
* **Comunidade Ativa:** Grande disponibilidade de frameworks e suporte técnico.

#### 🧪 Por que para Data Science?
A linguagem é o padrão da indústria por sua eficiência em lidar com:
1.  **Grandes volumes de dados** (Big Data).
2.  **Operações matemáticas complexas.**
3.  **Integração facilitada** com ferramentas de visualização e bancos de dados.

> [!TIP]
> **Documentação Oficial:** [python.org](https://www.python.org/)

---

### 🎨 Identidade Visual
O nome foi inspirado no grupo de comédia *Monty Python*. Abaixo, o símbolo oficial da linguagem:

![Logo Python](https://www.python.org/static/community_logos/python-logo-master-v3-TM.png)

## 1.2 Ambiente de Desenvolvimento: Google Colab

Para praticar Ciência de Dados, utilizamos o **Google Colaboratory (Colab)**. Ele é um ambiente baseado em nuvem que permite a execução de código Python diretamente no navegador, sem necessidade de configuração local.

### 💡 Por que usar o Colab?
* **Zero Instalação:** Tudo roda nos servidores do Google.
* **Recursos Gratuitos:** Acesso a RAM e GPU (essencial para modelos pesados).
* **Colaboração:** Funciona como um "Google Docs", mas para código.
* **Requisito:** Basta ter uma conta **Gmail**.

---

### 📓 O que é um Notebook (`.ipynb`)?
Diferente de scripts Python comuns (`.py`), um **Notebook** é um documento interativo que intercala:
1.  **Células de Código:** Onde o Python é executado.
2.  **Células de Texto:** Formatadas em Markdown (como esta que você lê).
3.  **Visualizações:** Gráficos e tabelas gerados pelo código.

> [!IMPORTANT]
> A extensão padrão de um notebook é **`.ipynb`** (Interactive Python Notebook). Eles podem ser abertos no Colab, Jupyter Notebook ou VS Code.

---

### ⌨️ Comandos e Execução
A execução ocorre em tempo real. Ao rodar uma célula, o Colab aloca uma **Máquina Virtual** para você.

* **Executar Célula:** `Shift` + `Enter` ou clique no botão ▶️ ao lado da célula.
* **Status do Ambiente:** No canto superior direito, você pode monitorar o uso de **RAM** e **Disco**.
* **Movimentação:** Use as setas (🔼/🔽) no menu da célula para reorganizar a ordem dos blocos.

### 1.3 Saída de Dados: A Função `print()`

A função `print()` é utilizada para exibir informações no console ou na saída de uma célula do notebook. É a ferramenta básica para depuração e visualização de estados do código.

#### Exemplo de Uso
```python
# Exibindo uma mensagem de texto (string)
print("Olá, Data Science!")

# Exibindo um valor numérico
print(10)
```

#### Retorno esperado:
~~~python
Olá, Data Science!
10
~~~

### 1.4 Comentários e Documentação

Comentários são anotações inseridas no código que o interpretador Python ignora. Eles são essenciais para documentar a lógica e aumentar a manutenibilidade do projeto.

#### 1.4.1 Comentários de Linha Única
Utiliza-se o símbolo `#`. Tudo o que estiver à direita dele na mesma linha é ignorado.

~~~python
# Este é um comentário de linha única
print(10) # Comentário inserido após uma instrução de código
~~~

#### Retorno esperado:
~~~python
10
~~~

#### 1.4.2 Comentários de Múltiplas Linhas
Utilizam-se aspas triplas (`'''` ou `"""`). São úteis para explicações extensas.

~~~python
'''
Este é um comentário
de várias linhas, ignorado
pelo interpretador.
'''
print("Python para Dados")
~~~

#### Retorno esperado:
~~~python
Python para Dados
~~~

## 02. Variáveis e Tipos de Dados

Nesta etapa, assumimos o papel de auxiliares de uma equipe de Ciência de Dados em uma instituição de ensino. O objetivo é utilizar Python para resolver problemas cotidianos da escola, começando pela manipulação de informações básicas.

---

### 2.1 O que são Variáveis?

Variáveis funcionam como nomes associados a valores ou informações armazenadas na memória do computador. Em Data Science, elas são essenciais para rotular dados que serão processados por algoritmos.

#### 2.1.1 Atribuição e Atualização
Para criar uma variável, utiliza-se o operador de atribuição `=`. O valor à direita é vinculado ao nome à esquerda. 

Uma característica fundamental é a **mutabilidade**: o valor de uma variável pode ser alterado ao longo da execução do código.

~~~python
# Atribuição inicial
idade = 5
print(idade)

# Atualizando o valor (o valor antigo é sobrescrito)
idade = 10
print(idade)
~~~

#### Retorno esperado:
~~~python
5
10
~~~

#### 2.1.2 Exibição de Valores em Notebooks
Além da função `print()`, os notebooks (como o Google Colab) exibem automaticamente o valor de uma variável se ela for escrita sozinha na **última linha** de uma célula.

~~~python
idade = 15
idade
~~~

#### Retorno esperado:
~~~python
15
~~~

---

### 2.2 Armazenando Textos (Strings)

Variáveis podem armazenar diferentes tipos de dados. Para textos, utilizamos aspas simples (`' '`) ou duplas (`" "`).

~~~python
nome = 'Gabriel'
nome
~~~

#### Retorno esperado:
~~~python
'Gabriel'
~~~



---

### 2.3 Regras de Nomeação e Boas Práticas

Para garantir que o código seja interpretável e profissional, existem regras rígidas e convenções para nomear variáveis:

#### 🚫 O que NÃO é permitido:
1.  **Iniciar com números:** Ex: `10_notas`, `2_nomes`.
2.  **Espaços vazios:** Ex: `nome aluno`. Utilize `nome_aluno` (padrão *Snake Case*).
3.  **Palavras Reservadas:** Não use nomes de funções nativas como `print` ou `type`.

#### ⚠️ Case Sensitivity (Sensibilidade a maiúsculas)
O Python diferencia letras maiúsculas de minúsculas. Portanto, as variáveis abaixo são tratadas como entidades distintas na memória:

~~~python
idade = 1
Idade = 2
IDADE = 3
_idade = 4

print(idade, Idade, IDADE, _idade)
~~~

#### Retorno esperado:
~~~python
1 2 3 4
~~~

> [!TIP]
> **Dica de Profissional:** Utilize sempre nomes descritivos. Prefira `media_notas_estudante` em vez de apenas `m` ou `n`, para que seu código seja autodocumentado.

### 2.4 Tipos de Variáveis (Classes)

O trabalho com Data Science exige a manipulação de diferentes formatos de dados. No Python, os dados são organizados em classes, sendo quatro delas os pilares fundamentais:

| CLASSE | DESCRIÇÃO | EXEMPLO |
| :--- | :--- | :--- |
| **int** | Números inteiros (positivos ou negativos). | `3`, `100`, `-5` |
| **float** | Números decimais ou fracionários (ponto flutuante). | `3.14`, `100.0`, `-0.5` |
| **str** | *Strings*: sequências de caracteres (textos) entre aspas. | `'Olá!'`, `"1234"` |
| **bool** | Valores lógicos: verdadeiro ou falso. | `True`, `False` |



---

#### 2.4.1 Identificando Tipos com `type()`

Cada variável referencia uma classe específica baseada no dado atribuído. Para verificar essa classificação, utilizamos a função nativa `type()`.

~~~python
i = 5
f = 9.8
s = 'Mirla'
b = True

print(type(i))
print(type(f))
print(type(s))
print(type(b))
~~~

#### Retorno esperado:
~~~python
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
~~~

> [!IMPORTANT]
> **Observações técnicas:**
> * **Floats:** A presença do ponto (`.`) é suficiente para classificar o dado como float, mesmo que a parte decimal seja zero (ex: `10.0`).
> * **Strings:** Números entre aspas (ex: `"1234"`) são tratados como texto e não permitem cálculos matemáticos diretos.
> * **Booleans:** A primeira letra deve ser sempre maiúscula (`True` ou `False`).

---

#### 2.4.2 Aplicação Prática: Ficha de Aluno

Consolidando os tipos de dados para criar um registro no sistema da instituição de ensino:

~~~python
# Atribuição de dados de diferentes tipos
nome_aluno = 'Fabricio Daniel' # str
idade_aluno = 15               # int
media_aluno = 8.45             # float
situacao_aprovado = True       # bool

# Exibição dos dados salvos na memória
print(nome_aluno, idade_aluno, media_aluno, situacao_aprovado)
~~~

#### Retorno esperado:
~~~python
Fabricio Daniel 15 8.45 True
~~~

### 2.5 Variáveis Numéricas e Operações Aritméticas

As variáveis do tipo `int` e `float` podem ser manipuladas através de operadores aritméticos para realizar cálculos complexos. Para exemplificar, utilizaremos os dados de recursos humanos da nossa instituição de ensino:

| Cargo | Quantidade (`int`) | Salário (`int`/`float`) |
| :--- | :--- | :--- |
| Segurança | 5 | 3000 |
| Docente | 16 | 6000 |
| Diretoria | 1 | 12500 |

#### 2.5.1 Declaração das Variáveis
Primeiro, armazenamos os dados brutos em variáveis descritivas:

~~~python
# Dados de Segurança
q_seguranca = 5
s_seguranca = 3000

# Dados de Docentes
q_docente = 16
s_docente = 6000

# Dados de Diretoria
q_diretoria = 1
s_diretoria = 12500
~~~

#### Retorno esperado:
~~~python
# (Sem saída visual, os valores foram apenas armazenados na memória)
~~~

---

#### 2.5.2 Operadores Aritméticos na Prática

Podemos resolver problemas de negócio utilizando os operadores padrão do Python:

| Operação | Operador |
| :--- | :---: |
| Soma | `+` |
| Subtração | `-` |
| Multiplicação | `*` |
| Divisão | `/` |



**1. Soma: Total de empregados**
~~~python
total_empregados = q_seguranca + q_docente + q_diretoria
total_empregados
~~~

#### Retorno esperado:
~~~python
22
~~~

**2. Subtração: Diferença salarial entre cargos**
~~~python
diferenca_salario = s_diretoria - s_seguranca
diferenca_salario
~~~

#### Retorno esperado:
~~~python
9500
~~~

**3. Multiplicação e Divisão: Média salarial ponderada**
Para calcular a média ponderada, multiplicamos a quantidade pelo salário de cada categoria e dividimos pelo total. O uso de **parênteses** é obrigatório para definir a ordem de precedência.

~~~python
media_salarial = (q_seguranca*s_seguranca + q_docente*s_docente + q_diretoria*s_diretoria) / total_empregados
media_salarial
~~~

#### Retorno esperado:
~~~python
5613.636363636364
~~~

> [!NOTE]
> **Precedência Matemática:** Assim como na matemática tradicional, o Python executa primeiro a multiplicação (`*`) e a divisão (`/`) antes da soma (`+`) e subtração (`-`). Use parênteses para garantir que as somas do numerador sejam realizadas antes da divisão final.

