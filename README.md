# 🚦 Cruzamento 4.0 — Semáforo Inteligente (MVP)

Projeto desenvolvido como atividade prática integradora no curso **Técnico em Desenvolvimento de Sistemas – SENAI**.

O **Cruzamento 4.0** simula um sistema de controle inteligente de semáforos, aplicando conceitos de **IoT**, **lógica de programação**, **arquitetura de sistemas**, **sistemas operacionais** e **segurança da informação**, com foco em resiliência e adaptação a cenários críticos.

---

## 📌 Objetivo do Projeto

Desenvolver uma **Solução Mínima Viável (MVP)** capaz de:

- Controlar um cruzamento inteligente
- Ajustar dinamicamente os tempos dos semáforos
- Reagir a condições climáticas adversas
- Operar de forma segura diante de falhas de sensores ou servidor
- Demonstrar boas práticas de organização, documentação e clean code

---

## 🧠 Funcionalidades Principais

- 🚗 Ajuste automático do tempo do sinal verde conforme o fluxo de veículos
- 🌧️ Adaptação do sistema em caso de chuva ou chuva intensa
- ⚠️ Modo de segurança automático em falha de sensores (pisca amarelo)
- 💻 Execução local do algoritmo quando o servidor está offline
- 🔐 Tela de login para acesso administrativo
- 🖥️ Painel visual de controle e monitoramento em tempo real
- 🔘 Botões para simulação de cenários isolados ou combinados
- 📊 Exibição do estado operacional do sistema (servidor, sensores e reações)

---

## 🏗️ Arquitetura Conceitual do Sistema

### Sensores (Simulados)
- Sensor de fluxo de veículos
- Sensor de chuva / chuva intensa

### Controlador
- Lógica inspirada em microcontrolador (ESP32 / Arduino – conceitual)

### Comunicação
- Modelo cliente-servidor
- Simulação de envio de dados ao servidor
- Execução local automática em caso de falha de comunicação

### Interface
- HTML, CSS e JavaScript puro
- Representação visual dos semáforos (via e pedestre)
- Painel de status e controle interativo

---

## 🔁 Lógica do Algoritmo (Resumo)

O sistema avalia continuamente:

- Estado dos sensores
- Condições climáticas
- Fluxo de veículos
- Disponibilidade do servidor

Com base nessas variáveis, o algoritmo:

- Ajusta os tempos do sinal verde e amarelo
- Prioriza a segurança em falhas
- Mantém funcionamento local quando o servidor está indisponível

O sistema permite **cenários combinados**, como:
- Chuva intensa + servidor offline
- Fluxo alto + chuva
- Falha de sensor em qualquer condição

---

## 🔐 Tela de Login

Acesso restrito ao painel de controle do sistema:

- **Usuário:** `admin`
- **Senha:** `cruzamento4`

> ⚠️ Implementação realizada apenas para fins didáticos.  
> Em ambiente real, seria necessária autenticação no servidor, uso de hash de senha e controle de sessão.

---

## 🛡️ Segurança da Informação (Resumo)

O projeto contempla conceitos de segurança, incluindo:

- Controle de acesso ao sistema
- Política de Senhas e Acessos
- Operação segura em falhas de sensores
- Continuidade operacional em falha do servidor
- Conscientização contra engenharia social

A política completa pode ser consultada na documentação do projeto.

---

## 📂 Estrutura do Projeto

```text
/
├── Documentação/
│   ├── Fluxogramas/
│   │   ├── Fluxograma Semáforos.png
│   │   └── Semáforo Pinos Leitura Flow-2026-01-29-172825.png
│   ├── 2.2 atividade do projeto.docx
│   ├── ATIVIDADE REVISÃO TERMOS 1 E 2.pdf
│   ├── Política de Segurança da Informação.docx
│   ├── Relatório de Requisitos do Projeto Cruzamento 4.0.docx
│   └── relatorio do sistema ops.docx
│
├── Interface de Controle/
│   ├── index.html        # Painel principal do sistema
│   └── login.html        # Tela de login
│
├── README.md             # Documentação principal do repositório
└── wifi-scan.zip         # Material complementar