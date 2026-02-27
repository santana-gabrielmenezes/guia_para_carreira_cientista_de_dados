# 📚 Base de Conhecimento: Data Science

## 01. Primeiros Passos em Dados

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
