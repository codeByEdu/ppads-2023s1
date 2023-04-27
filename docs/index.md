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
