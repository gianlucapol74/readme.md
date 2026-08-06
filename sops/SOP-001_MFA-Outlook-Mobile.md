# SOP-001: Configuração de E-mail Corporativo e Autenticação Multifator (MFA) no Outlook Mobile

* **Código:** SOP-001
* **Categoria:** Software / Acessos
* **Nível de Atendimento:** N1
* **Última Atualização:** Agosto/2026

---

##  Objetivo
Orientar o analista de suporte no processo de configuração de conta corporativa (Microsoft 365) no aplicativo Outlook para dispositivos móveis (Android/iOS), incluindo a validação por Autenticação Multifator (MFA).

##  Pré-requisitos
* Usuário com conta ativa no Active Directory / Microsoft 365.
* Dispositivo móvel do usuário conectado à internet.
* Aplicativo **Microsoft Authenticator** instalado no smartphone.

---

##  Passo a Passo

### Etapa 1: Instalação e Acesso Inicial
1. Solicite ao usuário que baixe o aplicativo **Microsoft Outlook** na Google Play Store ou App Store.
2. Abra o aplicativo e digite o e-mail corporativo do usuário (`usuario@empresa.com.br`).
3. Clique em **Adicionar Conta**.

### Etapa 2: Validação de Credenciais e MFA
1. Digite a senha temporária ou atual fornecida pela equipe de TI.
2. O sistema solicitará a verificação de segurança (MFA).
3. Caso seja o primeiro acesso, selecione a opção de autenticação via aplicativo **Microsoft Authenticator** ou via envio de código SMS para o número cadastrado.
4. Insira o código de 6 dígitos recebido ou aprove a notificação no aplicativo Authenticator.

### Etapa 3: Finalização
1. Se for o primeiro acesso, o sistema exigirá a criação de uma nova senha (respeitando a complexidade de no mínimo 8 caracteres, letras maiúsculas, minúsculas e números).
2. Pule a opção de adicionar outra conta e aguarde a sincronização inicial das mensagens.

---

## Resolução de Problemas Comuns (Troubleshooting Rápido)
* **Erro "Conta não encontrada":** Verifique se o e-mail foi digitado corretamente e se a licença do Microsoft 365 está atribuída ao usuário.
* **Código MFA não chega via SMS:** Verifique a sinalização do celular ou altere o método de validação para ligação telefônica ou aplicativo Authenticator.
