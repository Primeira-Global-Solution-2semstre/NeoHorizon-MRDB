# 🌌 NeoHorizon – Sistema Inteligente para Monitoramento de Detritos Espaciais

## Global Solution 2026/1

### Mastering Relational and Non-Relational Database

---

## 👨‍💻 Integrantes

| Nome                   | RM       |
| ---------------------- | -------- |
| RAFAEL KUBAGAWA RAMOS  | RM565572 |
| VINICIUS SOTERAS BRAGA | RM566230 |

---

# 🚀 Sobre o Projeto

O **NeoHorizon** é um sistema desenvolvido em Oracle PL/SQL com o objetivo de monitorar detritos espaciais, identificar potenciais riscos de colisão e auxiliar na proteção de satélites ativos em órbita terrestre.

A solução simula um ambiente de monitoramento orbital capaz de transformar dados de telemetria em informações estratégicas para tomada de decisão, utilizando recursos avançados de banco de dados relacional, automação por gatilhos, encapsulamento de regras de negócio e geração de relatórios analíticos.

O projeto foi desenvolvido como parte da disciplina **Mastering Relational and Non-Relational Database**, demonstrando a aplicação prática de conceitos de modelagem de dados, programação PL/SQL e automação de processos.

---

# 🎯 Objetivo

O NeoHorizon tem como finalidade:

* Monitorar detritos espaciais em órbita terrestre.
* Catalogar objetos orbitais e satélites ativos.
* Detectar possíveis riscos de colisão.
* Gerar alertas automáticos de risco.
* Automatizar processos através de Procedures, Functions e Triggers.
* Disponibilizar relatórios analíticos para apoio à tomada de decisão.

---

# 🏗️ Arquitetura do Sistema

O sistema é composto por uma estrutura relacional totalmente normalizada e integrada.

Fluxo simplificado:

```text
SATELITES
     │
     ▼
MISSOES
     │
     ▼
DETRITOS
     │
     ▼
COLISOES
     │
     ▼
ALERTAS

OBSERVACOES
OPERADORES
LOGS
```

As tabelas são relacionadas através de chaves primárias e estrangeiras, garantindo integridade referencial e consistência dos dados.

---

# 📋 Requisitos Acadêmicos Atendidos

| Requisito                      | Status |
| ------------------------------ | ------ |
| 8 Tabelas Relacionais          | ✅      |
| 8 Sequences                    | ✅      |
| 3 Functions                    | ✅      |
| 3 Procedures                   | ✅      |
| 3 Triggers                     | ✅      |
| 1 Package PL/SQL               | ✅      |
| 4 Cursores Explícitos          | ✅      |
| 6 Blocos Anônimos              | ✅      |
| 5 Relatórios Analíticos        | ✅      |
| Mais de 90 Registros Simulados | ✅      |

---

# 🗄️ Estrutura do Banco de Dados

## Tabelas Principais

### SATELITES

Armazena informações dos satélites monitorados pelo sistema.

### DETRITOS

Responsável pelo cadastro dos detritos espaciais identificados.

### MISSOES

Contém os dados das missões espaciais associadas aos satélites.

### COLISOES

Registra eventos e previsões de colisões orbitais.

### ALERTAS

Armazena alertas gerados automaticamente pelo sistema.

### OBSERVACOES

Registra observações realizadas pelos operadores.

### OPERADORES

Cadastro dos usuários responsáveis pelo monitoramento.

### LOGS

Histórico de eventos e operações executadas.

---

# ⚙️ Recursos Implementados

## 🔹 Functions

As funções foram desenvolvidas para:

* Calcular índices de risco orbital.
* Retornar informações consolidadas.
* Automatizar consultas recorrentes.

---

## 🔹 Procedures

As procedures executam:

* Cadastro automatizado de informações.
* Atualização de status operacionais.
* Processamento de eventos críticos.

---

## 🔹 Triggers

### TRG_ALERTA_AUTOMATICO

Gera alertas automaticamente quando condições críticas são identificadas.

### TRG_PADRONIZA_DADOS

Padroniza informações antes da gravação.

### TRG_LOG_OPERACAO

Registra eventos importantes para auditoria.

---

## 🔹 Package PKG_NEOHORIZON

O package centraliza as regras de negócio do sistema.

Principais responsabilidades:

* Gerenciamento de detritos.
* Monitoramento de riscos.
* Processamento de alertas.
* Consultas operacionais.
* Automatização de processos críticos.

---

# 🔄 Cursores Explícitos

O sistema utiliza 4 cursores explícitos para:

* Navegação de registros de detritos.
* Processamento de alertas.
* Atualização de estados orbitais.
* Geração de relatórios analíticos.

---

# 📊 Relatórios Analíticos

Foram desenvolvidos 5 relatórios utilizando INNER JOIN, GROUP BY e funções de agregação.

Exemplos:

* Quantidade de detritos por categoria.
* Satélites monitorados por missão.
* Histórico de alertas emitidos.
* Eventos de colisão registrados.
* Estatísticas gerais do sistema.

---

# 🧪 Dados Simulados

O banco é populado automaticamente com mais de 90 registros fictícios para simular um ambiente real de monitoramento espacial.

Os dados incluem:

* Satélites ativos.
* Detritos espaciais.
* Missões espaciais.
* Alertas.
* Observações operacionais.
* Eventos de colisão.

---

# 🚀 Como Executar o Projeto

## 1. Abrir o Oracle SQL Developer

Conecte-se a uma instância Oracle local ou Oracle Cloud.

---

## 2. Habilitar saída do console

```sql
SET SERVEROUTPUT ON;
```

---

## 3. Executar o Script Principal

```sql
@NeoHorizon_Oracle_Corrigido.sql
```

ou simplesmente execute todo o conteúdo do arquivo no SQL Developer.

---

## 4. Verificar Objetos Criados

```sql
SELECT OBJECT_NAME,
       OBJECT_TYPE
FROM USER_OBJECTS
ORDER BY OBJECT_TYPE, OBJECT_NAME;
```

---

# 📈 Exemplo de Saída

```text
ALERTA CRÍTICO GERADO

SATÉLITE: ORBITAL-X1
DETRITO: DH-459
RISCO DE COLISÃO: 92%

STATUS:
AÇÃO IMEDIATA RECOMENDADA
```

---

# 🛡️ Benefícios da Solução

* Automação de processos de monitoramento.
* Redução de riscos operacionais.
* Centralização das informações orbitais.
* Geração automática de alertas.
* Facilidade de manutenção através de Package PL/SQL.
* Alto nível de integridade dos dados.

---

# 💻 Tecnologias Utilizadas

* Oracle Database
* Oracle SQL Developer
* SQL
* PL/SQL
* GitHub
* Oracle Cloud

---

# 📚 Conceitos Aplicados

* Modelagem Relacional
* Normalização de Dados
* Constraints
* Sequences
* Procedures
* Functions
* Packages
* Triggers
* Cursores Explícitos
* Tratamento de Exceções
* Blocos Anônimos
* Relatórios Analíticos
* Integridade Referencial

---

# 🌍 Contexto da Global Solution

O aumento constante da quantidade de satélites e detritos espaciais representa um desafio global para a segurança das operações orbitais.

O NeoHorizon foi concebido como uma plataforma de demonstração capaz de aplicar conceitos de banco de dados para monitorar esse cenário, simulando processos de análise, prevenção e resposta a eventos de risco no ambiente espacial.

---

# ✅ Conclusão

O NeoHorizon demonstra a aplicação prática dos recursos avançados do Oracle PL/SQL na construção de uma solução robusta para monitoramento espacial.

Além de atender integralmente aos requisitos acadêmicos da disciplina, o projeto evidencia a utilização de boas práticas de modelagem de dados, automação de processos e desenvolvimento de sistemas orientados a banco de dados.
