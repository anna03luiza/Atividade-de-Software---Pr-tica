import sqlite3 = importa o módulo 'sqlite3', que vai permitir interagir com bancos de dados SQLite em Python;

sqlite3.connect('squad.db') = conecta ao banco de dados SQLite com o mesmo nome, ou seja, 

'squad.db'. Se o banco de dados não existir, ele será criado;

conn.cursor() = Cria um cursor para executar comandos SQL no banco de dados;

conectar = função que irá retornar uma conexão com o banco de dados 'squad.db'

conn.commit() = Salva as alterações feitas no banco de dados;

commit = encerra a unidade de trabalho em que é excutada e inicia uma nova unidade;

conn.close() = fecha a conexão com o banco de dados;

cursor.fetchall() = Obtém todos os registros selecionados;

CREAT TABLE IF NOR EXISTS squad = Cria uma tabela chamada 'squad' se ela ainda não existir;

id INTEGER PRIMARY KEY AUTOINCREMENT = Define uma coluna 'id' que é uma chave primária e será automaticamente colocada em cada novo registro;

conectar = função que irá retornar uma conexão com o banco de dados 'squad.db'

INSERT INTO squad = comando SQL para inserir um novo registro;

SELECT * FROM squad = comando SQL para selecionar todos os registros da tabela 'squad';

UPTADE squad SET = comando SQL para atualizar um registro específico;

DELETE FROM squad WHERE id = comando SQL para deletar um registro específico;

Menu = função que exibe um menu interativo para o usuário e executa ações com base na escolha do usuário;

IF = É utilizado para verificar uma condição e executar um bloco de código se essa condição for verdadeira;

ELIF = Permite verificar múltiplas condições em sequência. Se a condição do if for falsa, o código irá verificar a condição do elif subsequente, e assim sucessivamente.

ELSE = Caso o usuário escolha uma opção inválida , exibe uma mensagem de erro;

if __name__ == '__main__'
  menu()
  
Verifica se o script está sendo executado diretamente(não importado como um módulo) e, se for o caso, chama a função 'menu' para iniciar o programa.

FOR integrante IN integrantes = inicia um loop que se repetirá sobre cada registro(ou tupla) na lista 'integrantes'

print(integrante) = imprime o registro atual (a tupla atual) no console.

Integrante = variável que será usada para armazenar o item atual da sequência durante cada iteração do loop.

Integrantes = sequência sobre a qual o loop 'FOR' irá iterar. Essa sequência é o valor retornado pela função 'listar_integrantes()' que irá conter todos os usuários registrados. 

FOR integrante in integrante = ele faz parte do loop 'FOR', que é usado para iterar sobre uma coleção de itens, ou seja, o loop FOR é usado para iterar uma sequência, que no caso mostrado é uma lista.

Já o IN é usado para verificar a presença de um item em uma sequência.

registros = cursor.fetchall() = esse comando retorna todos os registros da tabela 'squad', que criamos, como uma lista de tuplas e armazena essa lista na variável "registros".

o método de inserir '?' nos comando SQL são viáveis, pois eles ajudam a não haver ataques de SQL injection e corromper o código, além de ser muito claro.

placeholders garantem que os valores fornecidos sejam tratados como dados e não como parte da consulta SQL. Isso impede que um atacante injete código SQL malicioso nos valores.

fetchall() = se a consulta retornar um grande número de linhas, ele pode consumir muita memória, pois todos os dados são carregados de uma vez. Em casos assim, tem outra ferramenta que mostra melhores resultados.
