# Atividades Python

## Variáveis numéricas

| ---   | 
|   ---   |   
q_seguranca = 5
s_seguranca = 3000
|   ---   |
q_docente = 16
s_docente = 6000
|   ---   |
q_diretoria = 1
s_diretoria = 12500
|   ---   |
 
**1. Soma**
`total_empregados = q_seguranca + q_docente + q_diretoria
total_empregados`

**2. Subtração**
`diferenca_salario = s_diretoria - s_seguranca
diferenca_salario`

**3. media ponderada**
`media = (q_seguranca*s_seguranca + q_docente*s_docente + q_diretoria*s_diretoria) / (total_empregados)
media`

## STRINGS

### Usando os métodos
`texto = '  Geovana Alessandra dias Sanyos '`

Temos o texto, que se refere ao nome da professora e a string, com dois espaços antes do nome dela e outro espaço após. Vamos rodar essa célula e objetivo é que, ao final, o nome esteja da seguinte forma:

'GEOVANA ALESSANDRA DIAS SANTOS'

`texto.upper()`

' GEOVANA ALESSANDRA DIAS SANYOS '

Ao rodarmos o código, receberemos o mesmo texto, escrito em letras maiúsculas. Se existe um método que converte todas as letras em maiúsculas, também existe um que retorne todas as letras em minúsculas, esse método é o str.lower(). O procedimento é o mesmo: string, seguida de ponto e método `lower()`.

`texto.lower()`

' geovana alessandra dias sanyos '

O retorno é o texto todo em letras minúsculas. Precisamos remover os espaços em branco antes e depois do texto. Para isso, usaremos o método `str.strip()`.

`texto.strip()`

'Geovana Alessandra dias Sanyos'

O retorno é o texto sem caracteres de espaço. Por fim, outro método interessante é o `str.replace`. Ele vai substituir um caractere antigo por um novo, conforme o que determinarmos no nosso comando.

`texto.replace('y','t')`

' Geovana Alessandra dias Santos '

Como salvar as transformações?  Aqui realizamos apenas a consulta da visualização da transformação!

Então, faremos texto = texto. Essa é uma atribuição para dizer que texto é igual a texto. Adicionando ponto, podemos atribuir também uma transformação. Vamos começar com o strip(), para remover espaços em branco.

`texto = texto.strip()`

Também precisamos tornar o texto maiúsculo e substituir o "y" por "t". Vamos fazer uma acumulação dos métodos. Já colocamos o método strip() para remover espaços em branco. O segundo método será o replace(), para substituirmos o "y" por "t".

`texto = texto.strip().repalce('y','t')`

Por fim, o terceiro método que executaremos será o upper(), para converter o texto em letras maiúsculas. Escrevendo texto na outra linha, podemos conferir se o texto foi atualizado.

`texto = texto.strip().repalce('y','t').upper()
texto`

'GEOVANA ALESSANDRA DIAS SANTOS'

### Coletando dados
Em algumas aplicações precisamos coletar valores da pessoa usuária do nosso projeto. Em python conseguimos coletar dados de usuário através do comando input().

Para fazer essa coleta podemos atribuir essa função à uma variável.

`nome = input('Escreva seu nome: ')`
Escreva seu nome: Wellington

`nome`
'WEllington'

O retorno desse comando sempre será uma *string*. Isso quer dizer que mesmo que façamos uma coleta de algo que deva ser numérico, ele será uma string.

Então, será preciso converter o resultado caso não seja desejável obter uma string.

Existem funções para conversão de valores:

- Inteiros: _int(dado_para_conversao)_
- Float:  _float(dado_para_conversao) _
- String:  _str(dado_para_conversao) _
- Booleano:  _bool(dado_para_conversao)_

`ano_entrada = input('Escreva o ano de ingresso do(a) estudante: ')`
Escreva o ano de ingresso do(a) estudante: 2023

`type(ano_entrada)`
str

`ano_entrada = int(input('Escreva o ano de ingresso do(a) estudante: '))`
Escreva o ano de ingresso do(a) estudante: 2023

`type(ano_entrada)`
int

Buscaremos apresentar melhor agora o resultado que obtivemos da transformação. Nós conseguimos formatar e apresentar o nosso resultado misturando strings com valores não textuais.

Para fazer isso usamos a estrutura de formatação f com strings.

`nota_entrada = float(input('Digite a nota do teste de ingresso: '))
print(f'Ano de entrada {ano_entrada} - nota do teste de ingresso {nota_entrada}´)`


Digite a nota do teste de ingresso: 9.0
Ano de entrada 2023 - nota do teste de ingresso 9.0
