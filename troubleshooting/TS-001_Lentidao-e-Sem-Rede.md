# TS-001: Fluxograma de Diagnóstico para Falhas de Rede e Conectividade no Windows

* **Código:** TS-001
* **Categoria:** Infraestrutura / Redes
* **Nível de Atendimento:** N1
* **Última Atualização:** Agosto/2026

---

## 🎯 Objetivo
Servir de guia de investigação rápida quando o usuário relata "Sem acesso à internet", "Sistemas fora do ar" ou "Rede lenta".

---

## 🧪 Roteiro de Diagnóstico Sequencial (Linha de Comando)

Abra o **Prompt de Comando (cmd)** como Administrador na máquina do usuário afetado e execute a sequência abaixo:

### Passo 1: Verificar se a placa de rede recebeu IP válido
```cmd
ipconfig /all

### Passo 2: Testar conectividade local (Gateway Padrão)
```cmd
ping [IP-DO-GATEWAY]

Exemplo: ping 192.168.1.1

Se responder: O cabo, o switch e a comunicação local estão ok. Vá para o Passo 3.

Se der "Esgotado o tempo limite da solicitação": Problema no roteador local, cabo danificado ou porta do switch.

### Passo 3: Testar comunicação externa via IP direto
```cmd
ping 8.8.8.8

Se responder: A internet está funcionando. O problema provável é resolução de nomes (DNS). Vá para o Passo 4.

Se não responder: O link de internet da empresa ou a VPN pode estar fora do ar.

### Passo 4: Limpeza e Resolução de DNS
```cmd
ipconfig /flushdns
nslookup google.com

Ação: Se o nslookup falhar, altere temporariamente os servidores DNS da placa para 8.8.8.8 e 1.1.1.1 para testar.

Quando escalar para o Nível 2 (Infra/Redes)?
Escale o chamado anexando o print dos comandos acima se:

Mais de 3 usuários no mesmo setor apresentarem o mesmo problema simultaneamente (suspeita de queda de Switch ou Link).

A placa de rede continuar sem IP mesmo após comandos de ipconfig /release e ipconfig /renew





