# Banco_de_dados.3
## Selects Simples

<img width="437" height="360" alt="image" src="https://github.com/user-attachments/assets/b431fd45-6869-4b2d-b99e-b60ac6c23070" />

Criar as tabelas da forma que foram diagramadas, obedecendo as seguintes restrições:

 - A coluna users_id da tabela associativa é FK da coluna id, tabela users
 - A coluna projects_id da tabela associativa é FK da coluna id, tabela projects
 - A coluna date da tabela projects deve verificar se a data é posterior que 01/09/2014.
 - Caso contrário, o registro não deve ser inserido
 - A PK de projects deve ser de auto incremento, iniciando em 10001, com incremento de 1
 - A PK de users deve ser de auto incremento, iniciando em 1, com incremento de 1
 - O valor padrão da coluna password da tabela users, deverá ser 123mudar
 - A coluna username da tabela users deve ter restrição de unicidade.
   
Modificar a coluna username da tabela Users para varchar(10)

Modificar a coluna password da tabela Users para varchar(8)

Inserir os dados abaixo:
Users
Id    Name     Username Password Email
1     Maria    Rh_maria 123mudar maria@empresa.com
2     Paulo    Ti_paulo 123@456 paulo@empresa.com
3     Ana      Rh_ana 123mudar ana@empresa.com
4     Clara    Ti_clara 123mudar clara@empresa.com
5     Aparecido    Rh_apareci 55@!cido aparecido@empresa.com

Projects
Id Name Description Date
10001 Re-folha Refatoração das
Folhas
05/09/2014
10002 Manutenção PC´s Manutenção PC´s 06/09/2014
10003 Auditoria NULL 07/09/2014
Users_has_projects
Users_id Projects_id
1 10001
5 10001
3 10003
4 10002
2 10002
