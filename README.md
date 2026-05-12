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

<img width="664" height="568" alt="image" src="https://github.com/user-attachments/assets/f4de0d86-632c-4b42-a7ed-de3534f58bd8" />

Considerar as situações:
- O projeto de Manutenção atrasou, mudar a data para 12/09/2014
- O username de aparecido (usar o nome como condição de mudança) está feio, mudar para Rh_cido
- Mudar o password do username Rh_maria (usar o username como condição de mudança) para 888@*, mas a condição deve verificar se o password dela ainda é 123mudar
- O user de id 2 não participa mais do projeto 10002, removê-lo da associativa
