# 🧠 Missão Alphazeta – Atividade de TDD com Testes Automatizados 🚀

## 👨‍🚀 Contexto

Você está desenvolvendo um sistema de gerenciamento da **estação espacial interplanetária “Alphazeta”**, parte de uma missão para estabelecer presença humana fora da Terra.

Os membros da estação (astronautas) precisam pesquisar módulos científicos, monitorar recursos vitais e reservar equipamentos ou laboratórios de forma segura e confiável.

A missão será implementada utilizando a metodologia **TDD – Test Driven Development**, com testes automatizados escritos com **JUnit 5**.

---

## 🎯 Objetivo

Desenvolver o sistema seguindo os princípios de TDD:

1. Escrever **testes que falham** (Red).
2. Escrever a **lógica necessária para que os testes passem** (Green).
3. Refatorar quando necessário (Refactor).

Você entregará duas versões do código:

- **Versão 1**: Testes que **não passam** (sem implementação da lógica).
- **Versão 2**: Testes que **passam** (com implementação da lógica).

---

## 🚀 User Stories

### ✅ US1 – Pesquisar Módulos por Tema

> Como membro da estação, quero pesquisar módulos (como “Botânica”, “Zero-G Fitness” ou “Astrobiologia”) por nome parcial, para encontrar onde realizar minhas atividades científicas.

- A busca deve ser **parcial**, ou seja, se digitar “bio”, deve retornar “Astrobiologia”.

---

### ✅ US2 – Listar Recursos da Estação

> Como membro da estação, quero listar módulos ou recursos da estação. Por padrão, só vejo os que estão funcionando, mas posso optar por ver todos, incluindo os em manutenção.

- Deve ser possível listar **somente recursos ativos** ou **todos os recursos** (ativos e inativos).
- Recursos em manutenção devem estar marcados como **inativos**.

---

### ✅ US3 – Reservar Laboratórios ou Equipamentos

> Como membro da estação, quero reservar um laboratório ou equipamento específico.

#### Regras:

- A reserva deve ser feita com o **ID do recurso** e o **nome do astronauta**.
- Somente recursos **existentes e ativos** podem ser reservados.
- Se a reserva não for possível, o sistema deve exibir uma das seguintes mensagens:
   - "Recurso em manutenção, escolha outro."
   - "Recurso não encontrado na estação."
- Se a reserva for bem-sucedida, deve exibir:
   - "Reserva bem-sucedida."

**Observação:** Usem o JUnit 5 no classpath do projeto.

