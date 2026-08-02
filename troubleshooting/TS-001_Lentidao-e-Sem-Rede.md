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
