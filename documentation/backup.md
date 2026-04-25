REQUISITOS FUNCIONAIS
RF.01: O sistema deve permitir cadastro de usuário.
RF.02: O sistema deve permitir autenticação de contas de usuário
RF.03: O sistema deve permitir autenticação de administradores em uma conta distinta, com permissões administrativas.
RF.04: O sistema deve exibir uma página de perfil com a lista de seguidores do perfil, a lista de perfis seguidos pelo usuário, os jogos adquiridos e os jogos publicados, de acordo com a visibilidade dessas abas
# alterar numeração…
RF.08: O sistema deve permitir que o dono do perfil altere a visibilidade das suas informações
# alterar numeração…
RF.12: O sistema deve permitir que o usuário adquira jogos gratuitos ou pagos.
RF.13: O sistema deve permitir que o usuário publique jogos.
RF.14: O sistema deve permitir o download de um jogo após sua aquisição.
RF.15: O sistema deve exibir uma página contendo uma biblioteca de jogos adquiridos pelo usuário.
RF.16: O sistema deve manter uma biblioteca de jogos publicados pelo usuário.
RF.17: O sistema deve permitir pagamentos via Pix.
RF.18: O sistema deve permitir pagamentos via Cartão.
RF.19: O sistema deve permitir que qualquer pessoa reporte jogos.
RF.20: O sistema deve permitir a avaliação de reports por responsáveis pela moderação.
RF.21: O sistema deve permitir que os usuários avaliem os jogos. As avaliações podem ou não conter comentários.
RF.22: O sistema deve restringir a avaliação aos usuários que comprovadamente consumiram o jogo. 
RF.23: O sistema deve permitir pesquisa de jogos por categoria.
RF.24: O sistema deve permitir pesquisa de jogos por nome.
RF.25: O sistema deve permitir que usuários sigam ou deixem de seguir outros perfis.
RF.26: O sistema deve permitir que os usuários visualizem a lista de solicitações para seguir.
RF.27: O sistema deve permitir que desenvolvedores registrem o andamento de seus projetos em desenvolvimento (DevLog).
RF.28: O sistema deve permitir confirmação de e-mail no cadastro.
RF.29: O sistema deve permitir atualização de dados cadastrais do usuário.
RF.30: O sistema deve permitir que o usuário visualize o histórico de compras.
RF.31: O sistema deve registrar e disponibilizar o status de cada compra, como pendente, aprovada ou cancelada.
RF.32: O sistema deve manter a associação entre jogo adquirido e conta compradora.
RF.33: O sistema deve permitir que o usuário visualize a página detalhada de um jogo antes da compra.
RF.34: O sistema deve permitir que o desenvolvedor edite e atualize jogos publicados.
RF.35: O sistema deve permitir que o desenvolvedor remova seus jogos, conforme regras da plataforma.
RF.36: O sistema deve permitir que o administrador remova jogos publicados.
RF.37: O sistema deve permitir que comentários e avaliações sejam moderados ou denunciados.
RF.38: O sistema deve permitir que o administrador consulte as informações das contas dos usuários.
RF.39: O sistema deve permitir que o administrador delete a conta de um usuário.
RF.40: O sistema deve permitir a notificação de interações relevantes, como compra, comentário, follow ou resposta a report.

REQUISITOS NÃO-FUNCIONAIS

RNF.01: O sistema deve disponibilizar autenticação em conta com verificação dupla.
RNF.02: O sistema deve proteger as credenciais dos usuários por meio de armazenamento seguro de senhas.
RNF.03: O sistema deve manter confidencialidade dos dados pessoais e das informações de pagamento.
RNF.04: O sistema deve criptografar as comunicações entre cliente e servidor.
RNF.05: O sistema deve responder às consultas de busca por nome ou categoria em até 2 segundos.
RNF.06: O sistema deve manter a plataforma disponível durante a maior parte do tempo, com alta confiabilidade operacional de  99% do tempo..
RNF.07: O sistema deve suportar acesso simultâneo de até 500 usuários sem degradação excessiva de desempenho.
RNF.08: O sistema deve processar compras, downloads e publicações de forma consistente e com baixa latência percebida pelo usuário.
RNF.09: O sistema deve ser escalável para comportar crescimento no número de usuários, jogos, avaliações, comentários e publicações.
RNF.10: O sistema deve ser capaz de armazenar e recuperar até 1TB de dados relacionados a jogos, usuários, bibliotecas, comentários e reports.
RNF.11: O sistema deve garantir a integridade dos dados de bibliotecas, compras, avaliações e publicações.
RNF.12: O sistema deve registrar logs de operações importantes, como login, compra, upload, report, moderação e alteração de privacidade. (Possível requisito arquitetural; possível implementação do RNF.13)
RNF.13: O sistema deve permitir rastreabilidade das ações executadas por usuários e administradores.
RNF.14: O sistema deve se adaptar adequadamente a diferentes tamanhos de tela, quando acessado em dispositivos distintos.
RNF.15: O sistema deve permitir correção e atualização de funcionalidades sem comprometer os dados existentes.
RNF.16: O sistema deve ser tolerante a falhas nas operações, realizando recuperação de dados
RNF 17: O sistema deve validar entradas do usuário para reduzir erros, inconsistências e uso indevido da plataforma.
RNF.18: O sistema deve atender a requisitos legais e de privacidade aplicáveis ao tratamento de dados dos usuários.






CASOS DE USO



UC 01 - Cadastrar usuário

UC 02 - Confirmar e-mail de cadastro

UC 03 - Autenticar usuário
Login
Validação de administradores e usuários comuns

UC 04 - Atualizar dados cadastrais do usuário:
Dados Cadastrais = Email cadastrado
Nome do perfil, etc. 
Não conta com senha

UC 05 - Excluir conta de usuário

UC 06 - Visualizar informações do perfil
Cenário A: visualizar seguidores
Cenário B: visualizar perfis seguidos
Cenário C: visualizar jogos adquiridos 
Cenário D: visualizar jogos publicados

UC 07 - Alterar visibilidade de informações do perfil
Setar suas informações como públicas/privadas. 
Informações seriam: 
perfis seguidos
perfis que o perfil segue
jogos publicados
jogos adquiridos

UC 08 - Visualizar histórico de compras

UC 09 - Busca de jogos
Cenário 1: busca por nome
Cenário 2: busca por categoria 

UC 10 - Visualizar página detalhada de jogo

UC 11 - Adquirir um jogo gratuito 

UC 12 - Adquirir um jogo pago	 
<<include>>  - Selecionar método de pagamento
<<include>>  - Processar pagamento
<<include>> - Consultar status da compra 

UC 13 - Baixar jogo adquirido

UC 14 - Enviar solicitação de seguimento

UC 15 - Deixar de seguir usuário

UC 16 - Visualizar solicitações de seguimento:
Cenário A (opcional): Aceitar solicitação de seguimento
Cenário B (opcional): Recusar solicitação de seguimento

UC 17 - Publicar jogo

UC 18 - Atualizar jogo publicado 

UC 19 - Remover jogo publicado

UC 20 - Registrar DevLog em um jogo

UC 21 - Visualizar DevLog

UC 22 - Avaliar jogo (Like/Deslike + comentário adicional não obrigado)
Cenário A (Opcional): Avaliação com comentário


UC 23 - Denunciar avaliação

UC 24 - Reportar jogo

UC 25 - Visualizar denúncia (moderação)
Cenário A: Denúncia de avaliação de jogo
Cenário B: Denúncia de jogo publicado

UC 26 - Deletar jogo publicado (moderação)

UC 27 - Deletar avaliação de usuário (moderação)

UC 28 - Deletar conta de usuário (moderação)

UC 29 - Consultar dados do usuário (moderação)

UC 30 - Exibir histórico de notificações

UC 31 - Selecionar método de pagamento

UC 31 - Processar pagamento

UC 32 - Consultar status da compra


DETALHAMENTO DOS CASOS DE USO

UC 01 - Cadastrar usuário

Atores: Usuário (não autenticado)

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário realiza seu cadastro na plataforma, fornecendo dados obrigatórios para criação de uma conta. Ao final, a conta é criada com status pendente de verificação.

Referência Cruzada: RF.01 – Cadastro de usuário;  RF.28 – Confirmação de e-mail; RNF.02 – Segurança de senhas; RNF.17 – Validação de entradas

Gatilho: O usuário seleciona a opção “Criar conta” ou “Cadastrar-se” na interface do sistema.

Pré-condições: 1 - O usuário não está autenticado no sistema; 2- O e-mail informado não está previamente cadastrado

Pós-condições: Conta criada com status não verificada; E-mail de confirmação enviado ao usuário; Dados do usuário armazenados de forma segura

Fluxo Principal (Cenário de Sucesso)

O usuário acessa a tela de cadastro
O sistema exibe o formulário de cadastro
O usuário preenche os dados obrigatórios (ex: nome, e-mail, senha)
O usuário submete o formulário
O sistema valida os dados informados
O sistema verifica a unicidade do e-mail
O sistema cria a conta com status pendente
O sistema envia e-mail de confirmação
O sistema informa sucesso no cadastro

Casos Alternativos:
A1 – Dados inválidos (No passo 5):

O sistema identifica inconsistências (campos vazios, formato inválido, senha fraca)
O sistema exibe mensagens de erro
O fluxo retorna ao passo 3

A2 – E-mail já cadastrado (No passo 6):

O sistema detecta duplicidade de e-mail
O sistema informa o usuário
O fluxo retorna ao passo 3

A3 – Falha no envio do e-mail de confirmação (No passo 8):

O sistema não consegue enviar o e-mail
O sistema registra a falha
O usuário pode solicitar reenvio posteriormente


UC 02 - Confirmar e-mail de cadastro

Atores: Usuário (não autenticado ou parcialmente autenticado)

Visão Geral: Este caso de uso descreve o processo de validação do e-mail do usuário após o cadastro. A confirmação é realizada por meio de um link ou código enviado ao e-mail informado, permitindo a ativação completa da conta no sistema.

Referência Cruzada: RF.28 – Confirmação de e-mail; RF.01 – Cadastro de usuário; RNF.01 – Verificação dupla (relacionado); RNF.03 – Confidencialidade dos dados

Gatilho: O usuário acessa o link de confirmação enviado por e-mail após o cadastro

Pré-condições: 1 - O usuário realizou o cadastro (UC01); 2 - A conta está com status não verificada; 3 - Existe um token/código de validação válido associado à conta

Pós-condições: Conta atualizada para status verificada/ativa; Usuário apto a utilizar todas as funcionalidades do sistema; Token de confirmação invalidado após uso

Fluxo Principal (Cenário de Sucesso):

O usuário acessa o link de confirmação recebido por e-mail
O sistema recebe o token de validação
O sistema verifica a validade do token
O sistema identifica a conta associada ao token
O sistema altera o status da conta para verificada
O sistema invalida o token utilizado
O sistema informa ao usuário que a conta foi confirmada com sucesso

Casos Alternativos:

A1 – Token inválido (No passo 3):

O sistema identifica que o token não é válido
O sistema exibe mensagem de erro
Retorna ao passo 2

A2 – Token expirado (No passo 3):

O sistema detecta que o token expirou
O sistema informa o usuário
O sistema oferece opção de reenvio de confirmação
Retorna ao passo 1

A3 – Conta já verificada (No passo 4):

O sistema identifica que a conta já foi confirmada
O sistema informa o usuário
O fluxo é encerrado

UC 03 - Autenticar usuário
Ator: Usuário Não Autenticado
Visão geral: Descreve o processo pelo qual um visitante fornece suas credenciais para acessar os recursos protegidos da plataforma, recebendo as permissões adequadas ao seu nível de acesso.
Referência cruzada:
Gatilho: Usuário acessa a página de login
Pré-condições: O usuário deve possuir um cadastro ativo e com o e-mail já confirmado (UC 02).
Pós-condições: Uma sessão segura é estabelecida (ex: geração de um token JWT de acesso); O sistema registra a data e hora do último login.
Fluxo Principal (Cenário de Sucesso):
O usuário insere seu e-mail e senha.
O usuário confirma as informações fornecidas
O sistema criptografa a senha inserida e a compara com o hash armazenado no banco de dados.
O sistema verifica os privilégios da conta (Usuário Comum ou Administrador).
O sistema redireciona o ator para a página inicial correspondente ao seu perfil (Dashboard Admin ou Home da Loja).
Casos alternativos:

A1 - Credenciais inválidas (No passo 3):
O sistema detecta que o e-mail não existe ou o hash da senha não confere.
O sistema nega o acesso e exibe uma mensagem de erro genérica ("E-mail ou senha incorretos").
O ator permanece na tela de login.
A2 - E-mail Não Confirmado (No passo 3):
O sistema valida as credenciais, mas verifica que o e-mail ainda não foi confirmado via link.
O sistema nega o acesso e exibe um alerta solicitando a confirmação, oferecendo a opção de reenviar o e-mail.




UC 04 – Atualizar dados cadastrais do usuário


Atores: Usuário (autenticado)

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário autenticado pode atualizar seus dados cadastrais na plataforma, como nome de perfil e e-mail, garantindo que suas informações estejam atualizadas.

Referência Cruzada: RF.29 – Atualização de dados cadastrais; RF.02 – Autenticação de usuário; RNF.02 – Segurança de credenciais; RNF.17 – Validação de entradas

Gatilho: O usuário acessa a opção “Editar perfil” ou “Atualizar dados cadastrais”

Pré-condições: 1- O usuário deve estar autenticado no sistema; 2- A conta do usuário deve estar ativa (e-mail já confirmado); 

Pós-condições: 1- Dados cadastrais atualizados com sucesso; 2- Informações persistidas no sistema; 3- Caso o e-mail seja alterado, pode exigir nova confirmação

Fluxo Principal (Cenário de Sucesso):

O usuário acessa a área de edição de perfil
O sistema exibe os dados atuais do usuário
O usuário altera os campos desejados (ex: nome, e-mail)
O usuário submete as alterações
O sistema valida os dados informados
O sistema atualiza os dados no banco
O sistema confirma a atualização ao usuário

Casos Alternativos:
A1 – Dados inválidos (No passo 5):

O sistema identifica dados inconsistentes (formato inválido, campos obrigatórios vazios)
O sistema exibe mensagens de erro
O fluxo retorna ao passo 3

A2 – E-mail já cadastrado por outro usuário (No passo 6):

O sistema detecta duplicidade de e-mail
O sistema informa o usuário
O fluxo retorna ao passo 3

A3 – Alteração de e-mail requer nova confirmação (No passo 6):

O sistema atualiza o e-mail com status não verificado
O sistema envia novo e-mail de confirmação
O usuário fica com acesso parcial até confirmar


UC 05 - Excluir conta

Atores: Usuário (autenticado)

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário solicita a exclusão de sua própria conta na plataforma. O sistema deve garantir a confirmação da intenção, tratar os dados associados conforme regras de integridade e privacidade, e finalizar a sessão do usuário.

Referência Cruzada: RF.29 – Atualização de dados cadastrais; RF.30 – Histórico de compras; RF.32 – Associação entre jogo e conta; RNF.03 – Confidencialidade dos dados; RNF.11 – Integridade dos dados; RNF.13 – Rastreabilidade; RNF.18 – Requisitos legais e de privacidade

Gatilho: O usuário seleciona a opção “Excluir conta” nas configurações do perfil.

Pré-condições: 1 - O usuário está autenticado no sistema; 2 - A conta do usuário existe e está ativa

Pós-condições: 1 - Conta do usuário excluída ou desativada no sistema; 2 - Dados pessoais tratados conforme política (remoção ou anonimização); 3 - Registros relevantes mantidos para integridade (ex: histórico de compras); 4 - Ação registrada em log; 5 - Sessão do usuário encerrada

Fluxo Principal (Cenário de Sucesso):

O usuário seleciona a opção de exclusão de conta
O sistema solicita confirmação da ação
O usuário confirma a exclusão
O sistema valida a identidade do usuário
O sistema processa a exclusão da conta
O sistema remove os dados do usuário
O sistema encerra a sessão do usuário
O sistema informa que a conta foi excluída com sucesso

Casos Alternativos:

A1 – Cancelamento da operação (No passo 3):
O usuário opta por não confirmar a exclusão
O sistema cancela a operação
O fluxo é encerrado

A2 – Falha na validação de identidade (No passo 5):
O sistema identifica credenciais inválidas
O sistema informa erro ao usuário
O fluxo é encerrado


UC 06 - Visualizar perfil de usuário

Atores: Usuário autenticado

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário acessa e visualiza o perfil de outro usuário na plataforma, incluindo suas informações públicas, como seguidores, perfis seguidos, jogos adquiridos e jogos publicados, conforme as configurações de privacidade definidas.

Referência Cruzada: RF.04 – Exibir seguidores; RF.05 – Exibir perfis seguidos; RF.06 – Exibir jogos adquiridos; RF.07 – Exibir jogos publicados; RF.08–RF.11 – Controle de visibilidade; RNF.03 – Confidencialidade dos dados

Gatilho: O usuário seleciona um perfil para visualização (ex: clique em nome de usuário, busca ou lista de usuários).

Pré-condições: O perfil a ser visualizado existe no sistema;

Pós-condições: Página de perfil exibida ao usuário; Informações apresentadas respeitando as configurações de visibilidade; Nenhuma alteração de estado no sistema

Fluxo Principal (Cenário de Sucesso):

O usuário acessa um perfil (via busca, link ou navegação)
O sistema recebe a solicitação de visualização
O sistema recupera os dados do perfil
O sistema verifica as configurações de visibilidade do perfil
O sistema filtra as informações disponíveis
O sistema exibe os dados do perfil ao usuário, incluindo:
seguidores (quando público)
perfis seguidos (quando público)
jogos adquiridos (quando público)
jogos publicados (quando público)

Casos Alternativos:

A1 – Cenário A: Visualizar seguidores (No passo 6):
O sistema exibe a lista de seguidores, caso a informação esteja pública

A2 – Cenário B: Visualizar perfis seguidos (No passo 6):
O sistema exibe a lista de perfis seguidos, caso a informação esteja pública

A3 – Cenário C: Visualizar jogos adquiridos (No passo 6):
O sistema exibe a lista de jogos adquiridos, caso a informação esteja pública

A4 – Cenário D: Visualizar jogos publicados (No passo 6):
O sistema exibe a lista de jogos publicados, caso a informação esteja pública

A5 – Informação privada (No passo 4):
O sistema identifica que determinadas informações estão como privadas
O sistema oculta essas informações
O sistema exibe apenas os dados públicos disponíveis

A6 – Perfil não encontrado (No passo 3): 
O sistema não localiza o perfil solicitado
O sistema informa que o perfil não existe
O fluxo é encerrado


UC 07 - Alterar visibilidade do perfil
Visão geral: Neste caso de uso, o usuário(dono do perfil) acessa a área de gerenciamento da sua conta para configurar a privacidade das suas informações na plataforma. O sistema permite que ele defina, de forma independente, o status de visibilidade (Público ou Privado) para quatro painéis específicos de sua página: a lista de seguidores, a lista de perfis que ele segue, a biblioteca de jogos adquiridos e a vitrine de jogos publicados.
Referências cruzadas: RF.08 - Alterar visibilidade das abas de informações do perfil
Gatilho: O ator aciona o caso de uso ao clicar na opção de "Configurações de Privacidade" ou ao acessar a área de "Editar Perfil" estando autenticado na sua conta.
Pré-condição: O ator deve estar devidamente autenticado no sistema (RF.02) e possuir um perfil ativo. O sistema de banco de dados deve estar operante.
Pós-condição: As mudanças são registradas no sistema, visíveis para todos os usuários.
Fluxo principal (Cenário de sucesso):
O ator acessa a tela de configurações de privacidade de perfil.
O sistema recupera e exibe o estado atual (Público ou Privado) das chaves de visibilidade referentes à: Seguidores, Perfis Seguidos, Jogos Adquiridos e Jogos Publicados.
O ator interage com a interface, modificando as opções desejadas de Público para Privado ou vice-versa.
O ator clica no botão para salvar as alterações.
O sistema valida os dados enviados, confirmando que a requisição partiu do usuário autenticado correto (RNF.17).
O sistema atualiza os atributos de privacidade do usuário no banco de dados.
O sistema gera e armazena um log da operação, registrando a data, a hora e a alteração de privacidade realizada (RNF.12).
O sistema exibe uma mensagem de sucesso na tela (ex: "Preferências de privacidade atualizadas") e mantém o ator na página de configurações.
Casos alternativos:
Cenário Alternativo 1: Navegação sem salvar (Referente ao passo 3)
O ator modifica uma ou mais chaves de visibilidade na tela.
Antes de acionar o botão de salvar, o ator tenta navegar para outra página, fechar a aba ou clicar em um link externo.
O sistema (via interface/frontend) exibe um alerta avisando que há alterações não salvas.
O ator pode optar por cancelar a navegação e retornar ao passo 4 do fluxo principal, ou confirmar a saída, descartando as edições feitas (o caso de uso é encerrado sem alterações no banco).
Cenário de Exceção 1: Falha na persistência dos dados (Referente ao passo 6)
O sistema tenta gravar as novas preferências, mas ocorre uma falha na comunicação com o banco de dados ou um erro interno de processamento.
O sistema aborta a transação para manter a integridade dos dados anteriores (RNF.11 e RNF.16).
O sistema exibe uma mensagem de erro amigável, informando que não foi possível salvar as configurações no momento e orientando o ator a tentar novamente mais tarde.
As opções na tela retornam ao seu estado original.




UC 08 - Visualizar histórico de compras

Atores: Usuário (autenticado)

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário autenticado acessa e visualiza o histórico de suas compras realizadas na plataforma, incluindo informações como jogos adquiridos, datas e status das transações.

Referência Cruzada: RF.30 – Visualizar histórico de compras; RF.31 – Status da compra; RF.32 – Associação entre jogo e conta; RNF.11 – Integridade dos dados

Gatilho: O usuário seleciona a opção “Histórico de compras” nas configurações da conta ou perfil.

Pré-condições: 1- O usuário está autenticado no sistema; 2- A conta do usuário existe

Pós-condições: 1- Histórico de compras exibido ao usuário; 2- Informações apresentadas de forma organizada e consistente

Fluxo Principal (Cenário de Sucesso):

O usuário seleciona a opção “Histórico de compras”
O sistema recebe a solicitação
O sistema recupera os dados de compras associados ao usuário
O sistema organiza as informações (data, jogo, status, valor)
O sistema exibe o histórico de compras ao usuário

Casos Alternativos:

A1 – Nenhuma compra registrada (No passo 4):
O sistema não encontra registros de compras
O sistema informa que não há compras no histórico
O fluxo é encerrado

A2 – Dados inconsistentes ou incompletos (No passo 5):
 O sistema identifica inconsistências nos registros
 O sistema exibe os dados disponíveis de forma parcial
 O sistema pode registrar o problema para auditoria


UC 09 - Busca de jogos

Atores: Usuário (autenticado ou não autenticado)

Visão Geral:
Este caso de uso descreve o processo pelo qual um usuário realiza buscas por jogos na plataforma, podendo utilizar diferentes critérios como nome ou categoria, com o objetivo de localizar títulos de interesse.

Referência Cruzada: RF.23 – Pesquisa de jogos por categoria; RF.24 – Pesquisa de jogos por nome; RNF.05 – Tempo de resposta em buscas

Gatilho: O usuário acessa a funcionalidade de busca e insere um termo ou seleciona uma categoria.

Pré-condições: 1- O sistema está disponível; 2- Existem jogos cadastrados na plataforma

Pós-condições: 1- Lista de jogos exibida conforme os critérios de busca; 2- Resultados organizados de forma compreensível ao usuário

Fluxo Principal (Cenário de Sucesso):

O usuário acessa a barra ou página de busca
O usuário informa um termo de busca ou seleciona uma categoria
O sistema recebe os critérios de busca
O sistema realiza a consulta na base de dados
O sistema filtra os resultados conforme o critério informado
O sistema exibe a lista de jogos correspondentes

Casos Alternativos:

A1 – Busca por nome (No passo 2):
 O usuário insere o nome (ou parte do nome) do jogo
 Retorna ao passo 3

A2 – Busca por categoria (No passo 2):
 O usuário seleciona uma categoria
 Retorna ao passo 3

A3 – Nenhum resultado encontrado (No passo 5):
 O sistema não encontra jogos correspondentes
 O sistema informa que não há resultados para a busca
 O fluxo é encerrado

UC 10 - Visualizar página detalhada do jogo

Atores: Usuário (autenticado ou não autenticado)

Visão Geral:
Este caso de uso descreve o processo pelo qual um usuário acessa a página detalhada de um jogo na plataforma, visualizando informações completas como descrição, categoria, imagens, avaliações, desenvolvedor e opções de aquisição.

Referência Cruzada:
RF.33 – Visualizar página detalhada de jogo; RF.21 – Avaliações de jogos; RF.23 – Pesquisa por categoria; RF.24 – Pesquisa por nome; RNF.05 – Tempo de resposta em consultas

Gatilho:
O usuário seleciona um jogo na loja, em resultados de busca, recomendações ou biblioteca.

Pré-condições: 1 - O jogo existe na plataforma; 2 - O usuário possui acesso à loja ou catálogo de jogos

Pós-condições:
• Página detalhada do jogo exibida ao usuário
• Informações do jogo apresentadas de forma organizada
• Nenhuma alteração persistente realizada no sistema

Fluxo Principal (Cenário de Sucesso):

O usuário acessa a loja ou catálogo de jogos

O usuário seleciona um jogo específico

O sistema recebe a solicitação de visualização

O sistema recupera os dados do jogo

O sistema recupera informações complementares (avaliações, imagens, categoria, desenvolvedor)

O sistema organiza os dados da página

O sistema exibe a página detalhada do jogo ao usuário

Casos Alternativos:

A1 – Jogo não encontrado (No passo 4):
• O sistema não localiza o jogo solicitado
• O sistema informa que o jogo não está disponível
• O fluxo é encerrado

A2 – Falha ao recuperar dados do jogo (No passo 4):
• O sistema não consegue acessar as informações do jogo
• O sistema informa erro ao usuário
• O fluxo é encerrado

A3 – Informações complementares indisponíveis (No passo 5):
• O sistema não consegue recuperar avaliações, imagens ou metadados adicionais
• O sistema exibe apenas as informações básicas disponíveis
• O fluxo continua normalmente

A4 – Conteúdo restrito ou removido (No passo 4):
• O sistema identifica que o jogo foi removido ou ocultado
• O sistema informa indisponibilidade do conteúdo
• O fluxo é encerrado


UC 11 - Adquirir um jogo gratuito
Atores: Usuário (autenticado)
Visão Geral:
 Este caso de uso descreve o processo pelo qual um usuário adiciona um jogo gratuito à sua biblioteca, sem a necessidade de realizar pagamento, garantindo a associação do jogo à sua conta.
Referência Cruzada:
 RF.12 – Aquisição de jogos; RF.15 – Biblioteca de jogos adquiridos; RF.32 – Associação entre jogo e conta; RNF.11 – Integridade dos dados
Gatilho:
 O usuário seleciona a opção “Obter” ou “Adicionar à biblioteca” em um jogo gratuito.
Pré-condições:
O usuário está autenticado no sistema


O jogo está disponível como gratuito


Pós-condições:
 • Jogo adicionado à biblioteca do usuário
 • Associação entre o jogo e a conta registrada
 • Jogo disponível para download
Fluxo Principal (Cenário de Sucesso):
O usuário acessa a página detalhada de um jogo gratuito


O usuário seleciona a opção de adquirir o jogo


O sistema recebe a solicitação


O sistema verifica se o jogo é gratuito


O sistema verifica se o usuário já possui o jogo


O sistema registra a aquisição do jogo


O sistema associa o jogo à conta do usuário


O sistema atualiza a biblioteca do usuário


O sistema informa sucesso na aquisição


Casos Alternativos:
A1 – Jogo já adquirido (No passo 5):
 • O sistema identifica que o usuário já possui o jogo
 • O sistema informa que o jogo já está na biblioteca
 • O fluxo é encerrado
A2 – Jogo não é gratuito (No passo 4):
 • O sistema identifica que o jogo possui custo
 • O sistema redireciona para o fluxo de compra de jogo pago
 • O fluxo é encerrado

UC 13 - Baixar jogo adquirido

Atores: Usuário (autenticado)

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário realiza o download de um jogo previamente adquirido (gratuito ou pago) a partir de sua biblioteca pessoal, tornando-o disponível em sua máquina local.

Referência Cruzada: RF.14 – Download de jogo; RF.15 – Biblioteca de jogos adquiridos; RF.12 – Aquisição de jogos; RNF.08 – Baixa latência nas operações; RNF.11 – Integridade dos dados

Gatilho: O usuário acessa sua biblioteca pessoal

Pré-condições: 1- O usuário está autenticado no sistema; 2- O jogo já foi adquirido pelo usuário; 3- O jogo está disponível para download

Pós-condições: 1- Download do jogo iniciado ou concluído na máquina do usuário;  2- Registro da ação pode ser armazenado (log); 3- Jogo disponível localmente para execução

Fluxo Principal (Cenário de Sucesso):

O sistema exibe a lista de jogos adquiridos
O usuário seleciona um jogo
O usuário seleciona a opção “Baixar”
O sistema verifica se o usuário possui o jogo
O sistema verifica a disponibilidade do download
O sistema inicia o download do jogo
O sistema acompanha o progresso do download
O sistema conclui o download
O sistema informa que o jogo está pronto para uso

Casos Alternativos:

A1 – Jogo não adquirido (No passo 5):
 O sistema identifica que o usuário não possui o jogo
 O sistema impede o download
 O sistema informa que é necessário adquirir o jogo
 O fluxo é encerrado

A2 – Jogo indisponível para download (No passo 6):
 O sistema identifica indisponibilidade (manutenção, remoção, etc.)
 O sistema informa o usuário
 O fluxo é encerrado

A3 – Falha no download (No passo 7):
 O sistema identifica erro durante o download
 O sistema pausa ou cancela o processo
 O sistema informa o usuário
 O usuário pode tentar novamente

A4 – Interrupção pelo usuário (No passo 8):
 O usuário cancela ou pausa o download
 O sistema interrompe o processo
 O progresso pode ser salvo (se aplicável)


UC 14 - Enviar solicitação de seguimento


Atores: Usuário (autenticado)

Visão Geral: Este caso de uso descreve o processo pelo qual um usuário solicita seguir outro perfil na plataforma. Dependendo das configurações de privacidade do perfil alvo, ou ficar pendente de aprovação.

Referência Cruzada: RF.25 – Seguir ou deixar de seguir perfis; RF.26 – Visualizar solicitações de seguimento; RF.04 – Visualizar seguidores; RNF.11 – Integridade dos dados; RNF.17 – Validação de entradas

Gatilho: O usuário seleciona a opção “Seguir” ao acessar o perfil de outro usuário.

Pré-condições: 1 - O usuário está autenticado no sistema; 2 - O perfil alvo existe; 3 - O usuário não segue atualmente o perfil alvo; 4 - Não existe solicitação pendente entre os usuários

Pós-condições: 1 - Solicitação de seguimento registrada no sistema; 2 - Atualização do estado de relacionamento entre os usuários; 3 - Notificação enviada ao usuário alvo

Fluxo Principal (Cenário de Sucesso):

O usuário acessa o perfil de outro usuário
O sistema exibe as informações do perfil
O usuário seleciona a opção “Seguir”
O sistema registra a solicitação de seguimento
O sistema atualiza o status (pendente ou aprovado automaticamente) (?)
O sistema confirma a ação ao usuário

Casos Alternativos:

A1 – Perfil público (No passo 4):
O sistema identifica que o perfil é público
O sistema realiza o seguimento automaticamente
O sistema atualiza a lista de seguidores e seguidos
O fluxo segue para o passo 7

A2 – Perfil privado (No passo 4):
O sistema identifica que o perfil é privado
O sistema registra a solicitação como pendente
O usuário alvo deverá aprovar ou recusar posteriormente
O fluxo segue para o passo 7

A3 – Usuário já segue o perfil (No passo 3):
O sistema identifica que o seguimento já existe
O sistema informa o usuário
O fluxo é encerrado

A4 – Solicitação já existente (No passo 3):
O sistema detecta uma solicitação pendente
O sistema informa o usuário
O fluxo é encerrado

A5 – Tentativa de seguir a si mesmo (No passo 3):
O sistema identifica que o usuário tentou seguir o próprio perfil
O sistema bloqueia a ação
O sistema informa o usuário
O fluxo é encerrado

A6 – Falha ao registrar solicitação (No passo 5):
O sistema não consegue salvar a solicitação
O sistema informa erro ao usuário
O fluxo é encerrado


UC 15 - Deixar de seguir usuário
Atores: Usuário (autenticado)
Visão Geral:
 Este caso de uso descreve o processo pelo qual um usuário deixa de seguir outro perfil na plataforma, removendo a relação de seguimento previamente estabelecida.
Referência Cruzada:
 RF.25 – Seguir ou deixar de seguir perfis; RF.04 – Visualizar seguidores; RF.05 – Visualizar perfis seguidos; RNF.11 – Integridade dos dados
Gatilho:
 O usuário seleciona a opção “Deixar de seguir” ao acessar o perfil de um usuário que já segue.
Pré-condições:
O usuário está autenticado no sistema


O usuário segue o perfil alvo


Pós-condições:
 • Relação de seguimento removida
 • Listas de seguidores e seguidos atualizadas
 • (Opcional) Notificação pode ser gerada
Fluxo Principal (Cenário de Sucesso):
O usuário acessa o perfil de outro usuário que já segue
O sistema exibe a opção “Deixar de seguir”
O usuário seleciona essa opção
O sistema recebe a solicitação
O sistema verifica a existência do relacionamento
O sistema remove a relação de seguimento
O sistema atualiza as listas de seguidores e seguidos
O sistema confirma a ação ao usuário


Casos Alternativos:
A1 – Usuário não segue o perfil (No passo 5):
 • O sistema identifica que não existe relação de seguimento
 • O sistema informa o usuário
 • O fluxo é encerrado



UC 16 - Visualizar solicitações de seguimento

Atores: Usuário (autenticado)
Visão Geral: Este caso de uso descreve o processo pelo qual um usuário visualiza as solicitações de seguimento recebidas e pode decidir aceitar, recusar ou não tomar nenhuma ação sobre elas.
Referência Cruzada: RF.26 – Visualizar solicitações de seguimento; RF.25 – Seguir usuários; RF.04 – Lista de seguidores; RNF.11 – Integridade dos dados
Gatilho: O usuário acessa a opção “Solicitações de seguimento” em sua conta ou perfil.
Pré-condições: 1- O usuário está autenticado no sistema; 2- Existem solicitações de seguimento registradas (ou não, mas o acesso deve ser possível)
Pós-condições: 1- Lista de solicitações exibida ao usuário; 2- Solicitações podem ser aceitas ou recusadas; 3- Listas de seguidores/seguidos atualizadas conforme ação
Fluxo Principal (Cenário de Sucesso):
O usuário acessa a área de solicitações de seguimento
O sistema recupera as solicitações pendentes
O sistema exibe a lista de solicitações ao usuário
O usuário seleciona uma solicitação específica
O usuário escolhe uma ação: aceitar, recusar ou ignorar
O sistema processa a ação escolhida
O sistema atualiza o status da solicitação
O sistema confirma a ação ao usuário

Casos Alternativos:

A1 – Nenhuma solicitação pendente (No passo 2):
 O sistema não encontra solicitações
 O sistema informa que não há solicitações pendentes
 O fluxo é encerrado
A2 – Usuário não realiza nenhuma ação (No passo 5):
 O usuário opta por não aceitar nem recusar
 O sistema mantém a solicitação como pendente
 O fluxo é encerrado
A3 – Usuário aceita  (No passo 6):
 O sistema atualiza as listas de seguidores e seguidos 
 Retorna ao passo 7









UC 30 - Selecionar método de pagamento

Atores: Usuário (comum).
Visão geral: Descreve a etapa em que o usuário, durante um fluxo de compra, escolhe a forma pela qual deseja pagar e fornece os dados necessários para essa modalidade.
Pré-condições:
O ator deve estar no processo de aquisição de um jogo pago (acionado pelo UC 12).
O sistema deve ter calculado o valor total da transação.
Pós-condições:
Os dados de pagamento (ex: token do cartão de crédito) são validados em formato e armazenados temporariamente em memória segura para o processamento.
O fluxo é devolvido ao Caso de Uso principal para iniciar o processamento.
Fluxo principal (Cenário de Sucesso - Cartão de Crédito):
O sistema apresenta as opções de pagamento disponíveis (Pix e Cartão de Crédito).
O ator seleciona "Cartão de Crédito".
O sistema exibe um formulário seguro solicitando Número do Cartão, Nome, Validade e CVV.
O ator preenche os dados e clica em "Confirmar Pagamento".
O sistema realiza uma validação de formato (ex: se o cartão tem 16 dígitos e se a data é válida).
O sistema criptografa os dados e conclui esta etapa, acionando em seguida o "Processar pagamento".
Casos Alternativos:
Cenário Alternativo 1: Pagamento via Pix (Referente ao passo 2)
O ator seleciona "Pix".
O sistema não exige preenchimento de formulário.
O ator clica em "Gerar código Pix".
O sistema conclui esta etapa e avança para o processamento.
Casos de Exceção:
Cenário de Exceção 1: Dados do cartão inválidos (Referente ao passo 5)
O sistema detecta que o número do cartão é inválido (falha no algoritmo de Luhn) ou está vencido.
O sistema destaca os campos com erro em vermelho e exibe uma mensagem de alerta.
O ator corrige os dados e tenta novamente. O fluxo retorna ao passo 4.



[GEMINI]: A VERIFICAR

[UC 12] Adquirir um jogo pago
Este é o coração financeiro da plataforma. Note como utilizamos os <<includes>> para manter o fluxo principal limpo e legível.
Ator Principal: Usuário (Comum) 
Atores Secundários: Gateway de Pagamento (Ator Externo)
Resumo: Descreve os passos necessários para um usuário comprar um jogo na plataforma, escolhendo a forma de pagamento e recebendo a liberação para download.
Pré-condições: * O ator deve estar autenticado (UC 03).
O jogo selecionado deve estar com status "Publicado" e ter um valor maior que zero.
Pós-condições: * O jogo é adicionado à biblioteca de "Jogos Adquiridos" do perfil do ator.
Um recibo/histórico da transação é gerado no banco de dados.
O sistema emite uma notificação de compra bem-sucedida para o usuário (via UC 31).
Fluxo Principal (Cenário de Sucesso):
O ator, na página detalhada do jogo (UC 11), clica em "Comprar".
O sistema verifica se o ator já possui o jogo em sua biblioteca.
O sistema exibe o resumo do pedido (nome do jogo e valor).
O ator executa o <<include>> Selecionar método de pagamento (escolhendo Pix ou Cartão).
O sistema inicia uma transação pendente no banco de dados.
O sistema executa o <<include>> Processar pagamento comunicando-se com o Gateway Externo.
O sistema executa o <<include>> Consultar status da compra até obter a resposta de "Aprovado".
O sistema consolida a transação, liberando o jogo na conta do ator.
O sistema exibe a tela de sucesso com um botão direto para "Baixar jogo adquirido" (UC 14).
Fluxos Alternativos:
[FA.01] Usuário já possui o jogo (Referente ao Passo 2):
O sistema identifica que o jogo já está na biblioteca de Adquiridos ou Publicados (se ele for o dono).
O sistema oculta/desabilita o botão de compra e exibe o botão "Baixar jogo adquirido". O caso de uso é encerrado.
Fluxos de Exceção:
[FE.01] Pagamento Recusado (Referente ao Passo 7):
O Gateway de pagamento retorna um status de "Recusado" ou falha de comunicação.
O sistema reverte (rollback) a transação pendente.
O sistema exibe uma mensagem de falha, orientando o ator a tentar outro cartão ou verificar o saldo.
O sistema retorna o ator para a tela de seleção de método de pagamento (Passo 4).