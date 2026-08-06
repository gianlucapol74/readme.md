# SOP-002: Redefinição de Senha e Desbloqueio de Conta no Active Directory (AD)

* **Código:** SOP-002
* **Categoria:** Identidade e Acessos (IAM)
* **Nível de Atendimento:** N1
* **Última Atualização:** Agosto/2026

---

##  Objetivo
Padronizar o atendimento para chamados de "Esquecimento de Senha" ou "Conta Bloqueada" no ambiente Windows Server / Active Directory.

##  Regra de Segurança do Suporte
> **ATENÇÃO:** Antes de alterar qualquer senha, confirme a identidade do colaborador solicitante (via confirmação de CPF, matrícula corporativa ou validação com o gestor direto) para evitar ataques de Engenharia Social.

---

##  Passo a Passo no Active Directory Users and Computers (ADUC)

### 1. Localização do Usuário
1. Acesse o servidor de domínio ou abra o console `dsa.msc` na máquina de administração.
2. Pressione `Ctrl + F` ou clique em **Find** (Localizar).
3. Digite o primeiro nome ou o *username* do colaborador e clique em **Find Now**.

### 2. Desbloqueio de Conta
1. Dê dois cliques no usuário e vá até a aba **Account** (Conta).
2. Se a opção *"Unlock account. This account is currently locked out..."* estiver marcada, marque a caixa de seleção.
3. Clique em **Apply**.

### 3. Redefinição de Senha
1. Clique com o botão direito sobre o nome do usuário e selecione **Reset Password** (Redefinir Senha).
2. Insira uma senha temporária padronizada (Ex: `Empresa@2026`).
3. **OBRIGATÓRIO:** Marque a caixa *"User must change password at next logon"* (O usuário deve alterar a senha no próximo logon).
4. Clique em **OK**.

---

##  Registro no Ticket (Exemplo de Notação)
> *"Atendimento realizado via telefone. Identidade confirmada via matrícula nº 4812. Conta desbloqueada e senha temporária fornecida ao usuário. Solicitada a alteração no primeiro login."*
