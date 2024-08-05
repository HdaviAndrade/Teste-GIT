# Desafio 
## Analista de Qualidade de Software Júnior - BeeDoo
### Etapa 1

#### Descrição

 Como um usuário registrado do site Beedoo, quero acessar e utilizar o módulo de curso para aprender o conteúdo educacional de forma eficiente e intuitiva, garantindo que meu progresso seja salvo e que eu receba feedback adequado.

#### Critérios de Aceitação:

1 - O usuário deve poder iniciar sessão no site com credenciais válidas.

2 - O usuário deve poder navegar até a página do módulo do curso após a autenticação.

3 - O usuário deve visualizar o conteúdo do curso, incluindo vídeos, textos e quizzes.

4 - O usuário deve poder realizar quizzes e ver os resultados.

5 - O sistema deve salvar o progresso do usuário no curso.

6 - O sistema deve fornecer feedback adequado em caso de erros, como credenciais inválidas ou falhas de carregamento de conteúdo.

#### Desenvolvimento da História

A história foi desenvolvida com base em requisitos comuns para plataformas de cursos online. Presume-se que o usuário tenha acesso a uma interface intuitiva e que o sistema forneça feedback adequado em todas as etapas do processo de inscrição. Considerações incluem a necessidade de validação de dados, gerenciamento de capacidade de cursos.

#### Casos de testes
##### Cenário 1: Criação de Conta
Feature: Criação de Conta

  Scenario: Criação bem-sucedida de conta

    Given o usuário está na página de registro
    When o usuário preenche todos os campos obrigatórios corretamente
    And o usuário clica no botão de registrar
    Then o sistema deve criar a conta do usuário
    And o usuário deve ser redirecionado para a página inicial
    And o usuário deve ver uma mensagem de boas-vindas

Diretrizes de Execução:

Condições Prévias: O usuário está na página de registro.

Passos:

Preencha todos os campos obrigatórios (nome, email, senha, confirmação de senha).

Clique no botão de registrar.

Resultado Esperado: Conta criada, redirecionamento para a página inicial e exibição de mensagem de boas-vindas.

Erros Esperados: Mensagem de erro caso algum campo obrigatório esteja vazio ou inválido.

##### Cenário 2: Procura e Seleção de Curso

Feature: Procura e Seleção de Curso

  Scenario: Procura e seleção bem-sucedida de curso

    Given o usuário está autenticado e na página inicial
    When o usuário utiliza a barra de busca para procurar um curso específico
    And o usuário clica no curso desejado nos resultados da busca
    Then o usuário deve ser redirecionado para a página de detalhes do curso
    And o usuário deve ver informações detalhadas sobre o curso

Diretrizes de Execução:

Condições Prévias: O usuário está autenticado e na página inicial.

Passos:

Utilize a barra de busca para procurar um curso específico.

Clique no curso desejado nos resultados da busca.

Resultado Esperado: Redirecionamento para a página de detalhes do curso e exibição das informações detalhadas.

Erros Esperados: Mensagem de erro caso o curso não seja encontrado.

##### Cenário 3: Inscrição no Curso

Feature: Inscrição no Curso

  Scenario: Inscrição bem-sucedida no curso

    Given o usuário está na página de detalhes do curso
    When o usuário clica no botão de inscrever-se
    And o usuário confirma a inscrição
    Then o sistema deve registrar o usuário no curso
    And o usuário deve ver uma mensagem de confirmação de inscrição

Diretrizes de Execução:

Condições Prévias: O usuário está na página de detalhes do curso.

Passos:

Clique no botão de inscrever-se.

Confirme a inscrição.

Resultado Esperado: Registro no curso e exibição de mensagem de confirmação de inscrição.

Erros Esperados: Mensagem de erro caso ocorra algum problema durante o registro.


##### Cenário 4: Erro ao Inscrever-se no Curso

Feature: Inscrição no Curso

  Scenario: Erro ao inscrever-se no curso

    Given o usuário está na página de detalhes do curso
    When o usuário clica no botão de inscrever-se
    And ocorre um problema técnico
    Then o sistema deve exibir uma mensagem de erro
    And o usuário não deve ser registrado no curso

Diretrizes de Execução:

Condições Prévias: O usuário está na página de detalhes do curso.

Passos:

Clique no botão de inscrever-se.

Resultado Esperado: Mensagem de erro exibida e usuário não registrado no curso.

Erros Esperados: Falha na inscrição devido a problemas técnicos


##### Cenário 5: Inscrição em Curso Cheio

Feature: Inscrição no Curso

  Scenario: Inscrição em curso cheio

    Given o usuário está na página de detalhes do curso
    And o curso está cheio
    When o usuário clica no botão de inscrever-se
    Then o sistema deve exibir uma mensagem indicando que o curso está cheio
    And o usuário não deve ser registrado no curso

Diretrizes de Execução:

Condições Prévias: O usuário está na página de detalhes do curso e o curso está cheio.

Passos:

Clique no botão de inscrever-se.

Resultado Esperado: Mensagem indicando que o curso está cheio e usuário não registrado no curso.

Erros Esperados: Nenhum.


##### Cenário 6: Inscrição em Curso com Preço Excedendo o Orçamento

Feature: Inscrição no Curso

  Scenario: Inscrição em curso com preço excedendo o orçamento

    Given o usuário está na página de detalhes do curso
    And o preço do curso excede o orçamento do usuário
    When o usuário clica no botão de inscrever-se
    Then o sistema deve exibir uma mensagem indicando que o curso excede o orçamento
    And o usuário não deve ser registrado no curso

Diretrizes de Execução:

Condições Prévias: O usuário está na página de detalhes do curso e o preço do curso excede o orçamento do usuário.

Passos:

Clique no botão de inscrever-se.

Resultado Esperado: Mensagem indicando que o curso excede o orçamento e usuário não registrado no curso.

Erros Esperados: Nenhum.

##### Evidencias da primeira etapa
###### link
https://drive.google.com/file/d/1LrosATKPzszQQRE92f4Y8e05qFL7z8h6/view?usp=sharing

### Etapa 2
#### Relatório de Erros e Testes






