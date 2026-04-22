# 📌 Requisitos do Sistema

---

## ✅ Requisitos Funcionais

- **RF.01:** Permitir cadastro de usuário  
- **RF.02:** Permitir autenticação de contas de usuário  
- **RF.03:** Permitir autenticação de administradores com permissões distintas  
- **RF.04:** Exibir lista de seguidores (quando pública)  
- **RF.05:** Exibir lista de perfis seguidos (quando pública)  
- **RF.06:** Exibir jogos adquiridos (quando pública)  
- **RF.07:** Exibir jogos publicados (quando pública)  

### 🔐 Privacidade do Perfil
- **RF.08:** Alterar visibilidade dos seguidores  
- **RF.09:** Alterar visibilidade dos perfis seguidos  
- **RF.10:** Alterar visibilidade dos jogos adquiridos  
- **RF.11:** Alterar visibilidade dos jogos publicados  

### 🛒 Loja e Biblioteca
- **RF.12:** Adquirir jogos (gratuitos ou pagos)  
- **RF.13:** Publicar jogos  
- **RF.14:** Baixar jogo adquirido  
- **RF.15:** Exibir biblioteca de jogos adquiridos  
- **RF.16:** Manter biblioteca de jogos publicados  

### 💳 Pagamentos
- **RF.17:** Pagamento via Pix  
- **RF.18:** Pagamento via Cartão  

### 🛡️ Moderação e Interação
- **RF.19:** Reportar jogos  
- **RF.20:** Avaliar reports (moderação)  
- **RF.21:** Avaliar jogos (com ou sem comentário)  
- **RF.22:** Restringir avaliação a usuários que adquiriram o jogo  

### 🔍 Busca e Social
- **RF.23:** Buscar jogos por categoria  
- **RF.24:** Buscar jogos por nome  
- **RF.25:** Seguir/deixar de seguir usuários  
- **RF.26:** Visualizar solicitações de seguimento  

### 🧑‍💻 Desenvolvedor
- **RF.27:** Registrar DevLog  

### 📧 Conta
- **RF.28:** Confirmar e-mail  
- **RF.29:** Atualizar dados cadastrais  

### 📊 Compras
- **RF.30:** Visualizar histórico de compras  
- **RF.31:** Exibir status da compra  
- **RF.32:** Associar jogo à conta compradora  
- **RF.33:** Visualizar página detalhada de jogo  

### 🛠️ Gestão de Jogos
- **RF.34:** Editar jogos  
- **RF.35:** Remover jogos (desenvolvedor)  
- **RF.36:** Remover jogos (admin)  

### ⚠️ Administração
- **RF.37:** Moderar comentários e avaliações  
- **RF.38:** Consultar contas de usuários  
- **RF.39:** Deletar conta de usuário  

### 🔔 Notificações
- **RF.40:** Notificar interações relevantes  

---

## ⚙️ Requisitos Não-Funcionais

### 🔐 Segurança
- **RNF.01:** Autenticação com verificação dupla  
- **RNF.02:** Armazenamento seguro de senhas  
- **RNF.03:** Confidencialidade de dados  
- **RNF.04:** Criptografia de comunicação  

### ⚡ Desempenho
- **RNF.05:** Busca em até 2 segundos  
- **RNF.06:** Disponibilidade de 99%  
- **RNF.07:** Suporte a 500 usuários simultâneos  
- **RNF.08:** Baixa latência em operações  

### 📈 Escalabilidade e Dados
- **RNF.09:** Escalabilidade do sistema  
- **RNF.10:** Armazenar até 1TB  
- **RNF.11:** Integridade dos dados  

### 📜 Auditoria e Logs
- **RNF.12:** Registro de logs  
- **RNF.13:** Rastreabilidade de ações  

### 📱 Usabilidade e Manutenção
- **RNF.14:** Responsividade  
- **RNF.15:** Atualizações sem perda de dados  
- **RNF.16:** Tolerância a falhas  
- **RNF.17:** Validação de entradas  
- **RNF.18:** Conformidade legal  

<br>

# 📌 Casos de Uso


## 👤 Conta

- **UC01:** Cadastrar usuário  
- **UC02:** Confirmar e-mail de cadastro  
- **UC03:** Autenticar usuário  
  - Login  
  - Validação (admin/usuário)  

- **UC04:** Atualizar dados cadastrais  
  - Email  
  - Nome do perfil  
  - (Sem alteração de senha)

- **UC05:** Excluir conta  


## 👥 Perfil

- **UC06:** Visualizar perfil  
- **UC07:** Visualizar informações do perfil  
  - Seguidores  
  - Seguidos  
  - Jogos adquiridos  
  - Jogos publicados  

- **UC08:** Alterar visibilidade do perfil  
  - Público/Privado para:
    - Seguidores  
    - Seguidos  
    - Jogos adquiridos  
    - Jogos publicados  


## 🛒 Loja

- **UC09:** Visualizar histórico de compras  

- **UC10:** Buscar jogos  
  - Por nome  
  - Por categoria  

- **UC11:** Visualizar página de jogo  

- **UC12:** Adquirir jogo gratuito  

- **UC13:** Adquirir jogo pago  
  - `<<include>>` Selecionar método de pagamento  
  - `<<include>>` Processar pagamento  
  - `<<include>>` Consultar status da compra  

- **UC14:** Baixar jogo  



## 👥 Social

- **UC15:** Solicitar seguimento  
- **UC16:** Deixar de seguir  

- **UC17:** Gerenciar solicitações  
  - Aceitar  
  - Recusar  



## 🎮 Desenvolvedor

- **UC18:** Publicar jogo  
- **UC19:** Atualizar jogo  
- **UC20:** Remover jogo  
- **UC21:** Registrar DevLog  
- **UC22:** Visualizar DevLog  



## ⭐ Avaliações

- **UC23:** Avaliar jogo  
  - Like/Dislike  
  - (Opcional) comentário  

- **UC24:** Denunciar avaliação  


## 🚨 Moderação

- **UC25:** Reportar jogo  

- **UC26:** Visualizar denúncias  
  - De avaliação  
  - De jogo  

- **UC27:** Deletar jogo (moderação)  
- **UC28:** Deletar avaliação  
- **UC29:** Deletar conta  
- **UC30:** Consultar dados do usuário  


## 🔔 Notificações

- **UC31:** Exibir histórico de notificações  

---