# 🚦 Cruzamento 4.0 — Semáforo Inteligente (MVP)

Projeto desenvolvido como atividade prática integradora no curso Técnico em Desenvolvimento de Sistemas – SENAI.

O **Cruzamento 4.0** simula um sistema de controle inteligente de semáforos utilizando conceitos de IoT, lógica de programação, segurança da informação e arquitetura de sistemas, com foco em resiliência e adaptação a cenários críticos.

---

## 📌 Objetivo do Projeto

Desenvolver uma **solução mínima viável (MVP)** capaz de:
- Controlar um cruzamento inteligente
- Adaptar tempos do semáforo conforme fluxo de veículos e clima
- Operar mesmo com falhas de sensores ou servidor
- Demonstrar conceitos de IoT, segurança e clean code de forma didática

---

## 🧠 Funcionalidades Principais

- 🚗 Ajuste automático do tempo do semáforo conforme fluxo de veículos
- 🌧️ Adaptação do sistema em caso de chuva ou chuva intensa
- ⚠️ Modo de segurança em falha de sensores (pisca amarelo)
- 💻 Execução local do algoritmo quando o servidor está offline
- 🔐 Tela de login para acesso administrativo
- 🖥️ Painel visual de controle e monitoramento em tempo real
- 🔘 Botões para simulação de cenários isolados ou combinados

---

## 🏗️ Arquitetura Conceitual

**Sensores simulados**
- Fluxo de veículos
- Chuva / Chuva intensa

**Controlador**
- Lógica inspirada em microcontrolador (ESP32 / Arduino – conceitual)

**Comunicação**
- Modelo cliente-servidor
- Simulação de envio de dados ao servidor
- Execução local em caso de falha

**Interface**
- HTML, CSS e JavaScript puro
- Simulação visual dos semáforos e estados do sistema

---

## 🔁 Lógica do Algoritmo (Resumo)

O sistema avalia continuamente:
- Estado dos sensores
- Condições climáticas
- Fluxo de veículos
- Disponibilidade do servidor

Com base nessas variáveis:
- Ajusta tempos do verde e amarelo
- Prioriza segurança em falhas
- Mantém funcionamento local quando necessário

Cenários podem ser **combinados**, como:
- Chuva intensa + servidor offline
- Fluxo alto + chuva
- Falha de sensor em qualquer situação

---

## 🔐 Tela de Login

Acesso restrito ao painel do sistema:

- **Usuário:** `admin`
- **Senha:** `cruzamento4`

> ⚠️ Implementação apenas para fins didáticos.  
> Em ambiente real, seria utilizada autenticação no servidor com hash de senha e controle de sessão.

---

## 🛡️ Segurança (Visão Geral)

- Controle de acesso ao sistema
- Operação local em caso de falha de comunicação
- Modo seguro automático em falha de sensores
- Conceitos de firewall e portas aplicados de forma teórica

---

## 📂 Estrutura do Projeto

```text
/
├── login.html        # Tela de login
├── index.html        # Painel principal do sistema
├── README.md         # Documentação do projeto
└── assets/           # (opcional) Imagens e recursos visuais