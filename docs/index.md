<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
# eDucation
</center></font>

**Conteúdo**

- [Autores](#autores)
- [Descrição do projeto](#descrição-do-projeto)
- [Diagrama de casos de uso](#diagrama-de-casos-de-uso)
- [Descrição dos casos de uso](#descrição-dos-casos-de-uso)
- [Protótipos de tela](#protótipos-de-tela)
- [Modelo de domínio](#modelo-de-domínio)
- [Decisões de arquitetura](#decisões-de-arquitetura)
- [Diagrama de implantação](#diagrama-de-implantação)
- [Referências](#referências)


# Autores

* Eduardo Pereira
* Rafael Guerino
* Davi Pena
* Lucas Juan



# Descrição do projeto

Nosso projeto tem como objetivo ajudar os professores e a escola controlar a presença dos alunos. Será um sistema para realizar o controle dos professores, alunos, disciplinas, turmas e faltas dos alunos.
Terá um Administrador (diretor da escola), Secretaria e o Professor que lançará as faltas, cada um tem sua função.
Diretor/Administrador poderá editar e adicionar dados dos professores, disciplinas e turmas para deixar salvo no sistema, o Professor pode adicionar faltas aos alunos quando não responderem a chamada na sala.
Secretária poderá adicionar e editar os alunos da escola.


# Diagrama de casos de uso

![Diagrama Caso de Uso Alunos](https://github.com/codeByEdu/ppads-2023s1/blob/master/docs/Diagrama%20de%20Caso%20de%20Uso.png)

*&lt;Diagrama de casos de uso&gt;*

# Descrição dos casos de uso

| **Especificação de caso de uso** |                                                                                            |
|----------------------------------|--------------------------------------------------------------------------------------------|
| **Nome**                         | Manter Alunos                                                                              |
| **Atores**                       | Secretaria                                                                                 |
| **Sumário**                      | Este caso de uso permite que o   secretária inclua, exclua ou consulte os dados dos alunos |
| **Pré-condição**                 | Entrar no sistema                                                                          |
| **Pós-condição**                 | Alunos terão seus dados   incluídos no sistema, assim poderão ser atribuídas as faltas.    |

| **Fluxo Principal**                   |                                                                                     |
|---------------------------------------|-------------------------------------------------------------------------------------|
| **Ações do   Ator**                   | **Ações do Sistema**                                                                |
| 1.   Seleciona a opção Manter Alunos. |                                                                                     |
|                                       |  2. Apresenta uma lista com   os Alunos que estiverem cadastrados.                  |
|                                       | 3. O sistema apresenta opções de   Incluir (FA1), Excluir (FA2) ou Consultar (FA3). |
|  4.   Seleciona a opção desejada.     |                                                                                     |

| **Fluxo Alternativo 1 (FA1) – Incluir Aluno**        |                                                                  |
|------------------------------------------------------|------------------------------------------------------------------|
| **Ações do   Ator**                                  | **Ações do Sistema**                                             |
| 1.   Seleciona a opção incluir Aluno.                |                                                                  |
|                                                      |  2. O sistema apresenta os   dados que precisam ser preenchidos. |
| 3.   Preenche os dados solicitados e clica em salvar |                                                                  |
|                                                      |  4. Salva   os dados do Aluno.                                   |

| **Fluxo Alternativo 2 (FA2) – Excluir Aluno** |                                                              |
|-----------------------------------------------|--------------------------------------------------------------|
| **Ações do Ator**                             | **Ações do Sistema**                                         |
| 1. Seleciona a opção Excluir Aluno.           |                                                              |
|                                               |  2. O sistema apresenta os dados do aluno que será excluído. |
| 3. Confirma Exclusão                          |                                                              |
|                                               |  4. Exclui o Aluno.                                          |

| **Fluxo Alternativo 3 (FA3) – Alterar Aluno** |                                                                |
|-----------------------------------------------|----------------------------------------------------------------|
| **Ações do   Ator**                           | **Ações do Sistema**                                           |
| 1. Seleciona o Aluno                          |                                                                |
|                                               |  2. O sistema apresenta os   dados do Aluno que será alterado. |
| 3.   Altera os dados do locatário             |                                                                |
| 4.   Seleciona a opção Confirmar Alterações   |                                                                |
|                                               |  5.   Atualiza os dados do Aluno.                              |

| **Fluxo Alternativo 4 (FA4) – Consultar Aluno** |                                                                              |
|-------------------------------------------------|------------------------------------------------------------------------------|
| **Ações do   Ator**                             | **Ações do Sistema**                                                         |
| 1. Seleciona a opção Consultar Aluno.           |                                                                              |
|                                                 |  2. O sistema apresenta um   filtro com nome dos alunos em ordem alfabética. |
| 3.   Preenche os dados no filtro.               |                                                                              |
|                                                 | 4. O sistema apresenta os Alunos   filtrados.                                |
|  5.   Seleciona Aluno desejado.                 |                                                                              |
|                                                 | 6. Apresenta os   dados do Aluno selecionado.                                |

| **Especificação de caso de uso** |                                                                                                                                                  |
|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| **Nome**                         | Manter Professores                                                                                                                               |
| **Atores**                       | Diretor (ADM)                                                                                                                                    |
| **Sumário**                      | Este caso de uso permite que o   diretor (administrador do sistema) inclua, exclua ou consulte os dados dos   professores.                       |
| **Pré-condição**                 | O diretor deve estar autenticado   no sistema      O sistema deve ter registrado pelo menos um professor                                         |
| **Pós-condição**                 | O sistema registra as   informações do novo professor ou atualiza os dados do professor existente, de   acordo com a ação executada pelo diretor |

| **Fluxo Principal**                                                     |                                                                                                                                                                 |
|-------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Ações do   Ator**                                                     | **Ações do Sistema**                                                                                                                                            |
| 1. O   diretor acessa a funcionalidade de manter professores no sistema |                                                                                                                                                                 |
|                                                                         | 2. O sistema exibe uma lista com   os professores já registrados                                                                                                |
| 3. O   diretor seleciona a opção de adicionar novo professor            |                                                                                                                                                                 |
|                                                                         | 4. O sistema exibe um formulário   para o diretor preencher as informações do novo professor (nome, sobrenome,   matrícula, disciplina, e-mail, telefone, etc.) |
| 5. O   diretor preenche as informações e clica em "Salvar"              |                                                                                                                                                                 |
|                                                                         | 6. O sistema valida as   informações e registra o novo professor no sistema                                                                                     |
|                                                                         | 7. O sistema   exibe uma mensagem de confirmação para o diretor                                                                                                 |

| **Fluxo Alternativo 1 (FA1) – Editar Professor**                        |                                                                                           |
|-------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
| **Ações   do Ator**                                                     | **Ações do Sistema**                                                                      |
| 1.   O diretor seleciona a opção de editar um professor existente       |                                                                                           |
|                                                                         | 2. O sistema   exibe um formulário preenchido com as informações do professor selecionado |
| 3. O   diretor modifica as informações desejadas e clica em "Salvar"    |                                                                                           |
|                                                                         | 4. O sistema valida as   informações e atualiza os dados do professor no sistema          |
| 5. O   sistema exibe uma mensagem de confirmação para o diretor         |                                                                                           |
|                                                                         | 6. O sistema valida as   informações e registra o novo professor no sistema               |
|                                                                         | 7. O sistema   exibe uma mensagem de confirmação para o diretor                           |

| **Fluxo Alternativo 2 (FA2) – Excluir Professor**                              |                                                                             |
|--------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| 4b. O diretor seleciona a opção de excluir um   professor existente:           |                                                                             |
| **Ações do   Ator**                                                            | **Ações do Sistema**                                                        |
|                                                                                | 1. O sistema   exibe uma lista com os professores já registrados            |
| 2. O   diretor seleciona o professor que deseja excluir e clica em   "Excluir" |                                                                             |
|                                                                                | 3. O sistema exibe uma mensagem   de confirmação para o diretor             |
|                                                                                | 4. O sistema   remove o professor do sistema                                |
|                                                                                | 6. O sistema valida as   informações e registra o novo professor no sistema |
|                                                                                | 7. O sistema   exibe uma mensagem de confirmação para o diretor             |

| **Especificação de caso de uso** |                                                                                                    |
|----------------------------------|----------------------------------------------------------------------------------------------------|
| **Nome**                         | Manter Disciplina                                                                                  |
| **Atores**                       | Diretor (Administrador)                                                                            |
| **Sumário**                      | Este caso de uso permite que o   administrador inclua, exclua ou consulte os dados das disciplinas |
| **Pré-condição**                 | Entrar no sistema                                                                                  |
| **Pós-condição**                 | Disciplinas terão que estar   incluidas para ser atribuidas nos horários ou turmas.                |

| **Fluxo Principal**                        |                                                                                     |
|--------------------------------------------|-------------------------------------------------------------------------------------|
| **Ações   do Ator**                        | **Ações do Sistema**                                                                |
| 1.   Seleciona a opção Manter Disciplinas. |                                                                                     |
|                                            |  2. Apresenta uma lista com   as Disciplinas que estiverem cadastradas.             |
|                                            | 3. O sistema apresenta opções de   Incluir (FA1), Excluir (FA2) ou Consultar (FA3). |
|  4.   Seleciona a opção desejada.          |                                                                                     |

| **Fluxo Alternativo 1 (FA1) – Incluir Disciplinas**  |                                                                  |
|------------------------------------------------------|------------------------------------------------------------------|
| **Ações   do Ator**                                  | **Ações do Sistema**                                             |
| 1.   Seleciona a opção incluir Disciplina.           |                                                                  |
|                                                      |  2. O sistema apresenta os   dados que precisam ser preenchidos. |
| 3.   Preenche os dados solicitados e clica em salvar |                                                                  |
|                                                      |  4. Salva   os dados da Disciplina.                              |

| **Fluxo Alternativo 2 (FA2) – Excluir Disciplina** |                                                                     |
|----------------------------------------------------|---------------------------------------------------------------------|
| **Ações   do Ator**                                | **Ações do Sistema**                                                |
| 1. Seleciona a opção Excluir Disciplina.           |                                                                     |
|                                                    |  2. O sistema apresenta os   dados da Disciplina que será excluído. |
| 3.   Confirma Exclusão                             |                                                                     |
|                                                    |  4. Exclui   a Disciplina.                                          |

| **Fluxo Alternativo 3 (FA3) – Alterar Disciplina** |                                                                     |
|----------------------------------------------------|---------------------------------------------------------------------|
| **Ações do   Ator**                                | **Ações do Sistema**                                                |
| 1. Seleciona a Disciplina                          |                                                                     |
|                                                    |  2. O sistema apresenta os   dados da Disciplina que será alterado. |
| 3.   Altera os dados do Disciplina                 |                                                                     |
| 4.   Seleciona a opção Confirmar Alterações        |                                                                     |
|                                                    |  5.   Atualiza os dados da Disciplina.                              |

| **Fluxo Alternativo 4 (FA4) – Consultar Disciplina** |                                                                                  |
|------------------------------------------------------|----------------------------------------------------------------------------------|
| **Ações do   Ator**                                  | **Ações do Sistema**                                                             |
| 1. Seleciona a opção Consultar Disciplina.           |                                                                                  |
|                                                      |  2. O sistema apresenta um   filtro com nome das Disciplina em ordem alfabética. |
| 3.   Preenche os dados no filtro.                    |                                                                                  |
|                                                      | 4. O sistema apresenta as   Disciplina filtradas.                                |
|  5.   Seleciona Disciplina desejada.                 |                                                                                  |
|                                                      | 6. Apresenta os   dados da Disciplina selecionada.                               |

| **Especificação de caso de uso** |                                                                                               |
|----------------------------------|-----------------------------------------------------------------------------------------------|
| **Nome**                         | Manter Turmas                                                                                 |
| **Atores**                       | Diretor (Administrador)                                                                       |
| **Sumário**                      | Este caso de uso permite que o   administrador inclua, exclua ou consulte os dados das Turmas |
| **Pré-condição**                 | Entrar no sistema                                                                             |
| **Pós-condição**                 | Turmas terão que estar incluidas   para atribuir os alunos e horários corretos                |

| **Fluxo Principal**                   |                                                                                     |
|---------------------------------------|-------------------------------------------------------------------------------------|
| **Ações do   Ator**                   | **Ações do Sistema**                                                                |
| 1.   Seleciona a opção Manter Turmas. |                                                                                     |
|                                       |  2. Apresenta uma lista com   as Turmas que estiverem cadastradas.                  |
|                                       | 3. O sistema apresenta opções de   Incluir (FA1), Excluir (FA2) ou Consultar (FA3). |
|  4.   Seleciona a opção desejada.     |                                                                                     |

| **Fluxo Alternativo 1 (FA1) – Incluir Turmas**       |                                                                  |
|------------------------------------------------------|------------------------------------------------------------------|
| **Ações do   Ator**                                  | **Ações do Sistema**                                             |
| 1.   Seleciona a opção incluir Turmas.               |                                                                  |
|                                                      |  2. O sistema apresenta os   dados que precisam ser preenchidos. |
| 3.   Preenche os dados solicitados e clica em salvar |                                                                  |
|                                                      |  4. Salva   os dados da Turma.                                   |

| **Fluxo Alternativo 2 (FA2) – Excluir Turmas** |                                                                 |
|------------------------------------------------|-----------------------------------------------------------------|
| **Ações do   Ator**                            | **Ações do Sistema**                                            |
| 1. Seleciona a opção Excluir Turmas.           |                                                                 |
|                                                |  2. O sistema apresenta os   dados da Turmas que será excluído. |
| 3.   Confirma Exclusão                         |                                                                 |
|                                                |  4. Exclui   a Turma.                                           |

| **Fluxo Alternativo 3 (FA3) – Alterar Turmas** |                                                                |
|------------------------------------------------|----------------------------------------------------------------|
| **Ações do   Ator**                            | **Ações do Sistema**                                           |
| 1. Seleciona a Turma                           |                                                                |
|                                                |  2. O sistema apresenta os   dados da Turma que será alterado. |
| 3.   Altera os dados do Disciplina             |                                                                |
| 4.   Seleciona a opção Confirmar Alterações    |                                                                |
|                                                |  5.   Atualiza os dados da Disciplina.                         |

| **Fluxo Alternativo 4 (FA4) – Consultar Turma** |                                                                              |
|-------------------------------------------------|------------------------------------------------------------------------------|
| **Ações do   Ator**                             | **Ações do Sistema**                                                         |
| 1. Seleciona a opção Consultar Turma.           |                                                                              |
|                                                 |  2. O sistema apresenta um   filtro com nome das Turmas em ordem alfabética. |
| 3.   Preenche os dados no filtro.               |                                                                              |
|                                                 | 4. O sistema apresenta as Turmas   filtradas.                                |
|  5.   Seleciona Turma desejada.                 |                                                                              |
|                                                 | 6. Apresenta os   dados da Turma selecionada.                                |

| **Especificação de caso de uso** |                                                                                                                                                                                        |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Nome**                         | **Atribuir Justificativa**                                                                                                                                                             |
| Atores                           | Secretaria                                                                                                                                                                             |
| Sumário                          | Este caso de uso permite que o a secretaria edite um registro de ausência de aluo no sistema e aplique uma   justificativa.                                                            |
| Pré-condição                     | O diretor deve estar autenticado no O secretaria deve estar autenticado no sistema O aluno deve estar registrado no sistema A ausência do aluno deve estar registrada no sistema       |
| Pós-condição                     | O sistema registra as informações da nova justificativa e atualiza as informações do aluno   correspondente, de acordo com a ação executada pela secretaria                            |

| **Fluxo Principal**                                                                      |                                                                                                                                                 |
|------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| **Ações do   Ator**                                                                      | **Ações do Sistema**                                                                                                                            |
| 1. A   secretaria acessa a funcionalidade de atribuir justificativa no sistema           |                                                                                                                                                 |
|                                                                                          | 2. O sistema exibe uma lista com   os alunos que possuem faltas não justificadas                                                                |
| 3. A   secretaria seleciona o aluno para o qual deseja atribuir a justificativa          |                                                                                                                                                 |
|                                                                                          | 4. O sistema exibe as   informações do aluno e as ausências não justificadas registradas                                                        |
| 5. A   secretaria seleciona a opção de atribuir justificativa para a ausência   desejada |                                                                                                                                                 |
|                                                                                          | 6. O sistema exibe um formulário   para o secretaria preencher as informações da justificativa (tipo de   justificativa, descrição, data, etc.) |
| 7. A   secretaria preenche as informações da justificativa e clica em   "Salvar"         |                                                                                                                                                 |
|                                                                                          | 8. O sistema   valida as informações e registra a justificativa no sistema                                                                      |
|                                                                                          | 9. O sistema   atualiza as informações do aluno, removendo a ausência não justificada   correspondente e adicionando a justificativa atribuída  |
|                                                                                          | 10. O sistema   exibe uma mensagem de confirmação para a secretaria                                                                             |

| **Fluxo Alternativo 1 (FA1) – Criar novo tipo de   justificativa**                 |                                                                                                                                       |
|------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| **Ações   do Ator**                                                                | **Ações do Sistema**                                                                                                                  |
| 6a.   A secretaria seleciona a opção de criar um novo tipo de justificativa:       |                                                                                                                                       |
|                                                                                    | 1. O sistema   exibe um formulário para o secretaria preencher as informações do novo tipo   de justificativa (nome, descrição, etc.) |
| 2. A   secretaria preenche as informações e clica em "Salvar"                      |                                                                                                                                       |
|                                                                                    | 3. O sistema valida as   informações e registra o novo tipo de justificativa no sistema                                               |
|                                                                                    | 4. O sistema   exibe uma mensagem de confirmação para o secretaria                                                                    |
| 5. A secretaria volta ao passo 6 e seleciona o novo tipo de   justificativa        |                                                                                                                                       |

| **Especificação de caso de uso** |                                                                                                                                                      |
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Nome**                         | Atribuir Faltas                                                                                                                                      |
| **Atores**                       | Professor                                                                                                                                            |
| **Sumário**                      | Este caso de uso permite que o   professor atribua faltas para alunos que não compareceram nas aulas.                                                |
| **Pré-condição**                 | O professor deve estar   autenticado no sistema      O aluno deve estar registrado no sistema                                                        |
| **Pós-condição**                 | O sistema registra as   informações da nova falta e atualiza as informações do aluno correspondente,   de acordo com a ação executada pelo professor |

| **Fluxo Principal**                                                           |                                                                                                                     |
|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| **Ações do   Ator**                                                           | **Ações do Sistema**                                                                                                |
| 1. O   professor acessa a funcionalidade de atribuir faltas no sistema        |                                                                                                                     |
|                                                                               | 2. O sistema exibe uma lista com   os alunos da turma do professor                                                  |
| 3. O   professor seleciona o aluno para o qual deseja atribuir a falta        |                                                                                                                     |
|                                                                               | 4. O sistema exibe as   informações do aluno e as presenças e faltas registradas até o momento                      |
| 5. O   professor seleciona a opção de atribuir uma falta para a data desejada |                                                                                                                     |
|                                                                               | 6. O sistema exibe um formulário   para o professor preencher as informações da falta (data, justificativa,   etc.) |
| 7. O   professor preenche as informações da falta e clica em "Salvar"         |                                                                                                                     |
|                                                                               | 8. O sistema   valida as informações e registra a falta no sistema                                                  |
|                                                                               | 9. O sistema atualiza as   informações do aluno, adicionando a falta correspondente                                 |
|                                                                               | 10. O sistema exibe uma mensagem   de confirmação para o professor                                                  |

| **Fluxo Alternativo 1 (FA1) – Atribuir falta com   justificativa**                 |                                                                                                                                                       |
|------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Ações   do Ator**                                                                | **Ações do Sistema**                                                                                                                                  |
| 5a.   O professor seleciona a opção de atribuir uma falta com justificativa:       |                                                                                                                                                       |
|                                                                                    | 1. O sistema   exibe um formulário para o professor preencher as informações da falta (data,   justificativa, tipo de justificativa, descrição, etc.) |
| 2. O   professor preenche as informações da falta e clica em "Salvar"              |                                                                                                                                                       |
|                                                                                    | 3. O sistema valida as   informações e registra a falta com justificativa no sistema                                                                  |
|                                                                                    | 4. O sistema   atualiza as informações do aluno, adicionando a falta correspondente com   justificativa                                               |
|                                                                                    | 5. O sistema   exibe uma mensagem de confirmação para o professor                                                                                     |

[*&lt;Descrição dos casos de uso&gt;*
](https://github.com/codeByEdu/ppads-2023s1/blob/da0588514578657bbea2bd94711a7e81187b00a9/docs/Especificac%CC%A7a%CC%83o%20de%20Caso%20de%20Uso%20--%20Alunos.xlsx)

# Protótipos de tela

[*&lt;Protótipos de tela&gt;*](https://github.com/codeByEdu/ppads-2023s1/blob/778ce002d94980ecf4992b470ad5ea0cc4824a4f/docs/PDF%20-%20Proto%CC%81tipo%20de%20telas.pdf)

# Modelo de domínio

![Diagrama de Domínio Faltas](https://user-images.githubusercontent.com/64917167/221467682-c7976422-31d6-4afa-a775-c90ca2d2919b.jpg)


# Decisões de arquitetura

![arquiteturaFaltas](https://user-images.githubusercontent.com/64917167/221709333-f1474767-ca26-4fcc-87e8-897a6721b8cc.jpg)



# Diagrama de implantação

*&lt;Diagrama de implantação&gt;*

# Referências

*&lt;Lista de referências&gt;*
