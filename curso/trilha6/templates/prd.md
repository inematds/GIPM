# PRD - Product Requirements Document
## [Nome do Projeto]

> **Documento de Requisitos do Produto GIPM**
> Detalha requisitos funcionais/nao-funcionais, epicos e historias de usuario.

---

## 1. Metas e Contexto

### 1.1 Metas do Produto
- [ ] [Meta 1 - resultado desejado]
- [ ] [Meta 2 - resultado desejado]
- [ ] [Meta 3 - resultado desejado]

### 1.2 Contexto de Background
[1-2 paragrafos resumindo o problema, mercado e por que este produto e necessario. Referencia o Project Brief para detalhes completos.]

### 1.3 Historico de Alteracoes

| Data | Versao | Descricao | Autor |
|------|--------|-----------|-------|
| [Data] | 1.0 | Versao inicial | [Nome] |

---

## 2. Requisitos

### 2.1 Requisitos Funcionais

| ID | Requisito | Prioridade |
|----|-----------|------------|
| FR1 | [O sistema deve permitir que usuarios facam X] | Must |
| FR2 | [O sistema deve processar Y em menos de Z segundos] | Must |
| FR3 | [O sistema deve notificar usuarios quando W] | Should |
| FR4 | [O sistema deve suportar integracao com V] | Could |

### 2.2 Requisitos Nao-Funcionais

| ID | Requisito | Categoria |
|----|-----------|-----------|
| NFR1 | [O sistema deve ter disponibilidade de 99.9%] | Disponibilidade |
| NFR2 | [Tempo de resposta da API deve ser < 200ms] | Performance |
| NFR3 | [Todos os dados devem ser criptografados em transito e repouso] | Seguranca |
| NFR4 | [O sistema deve estar em conformidade com LGPD] | Compliance |
| NFR5 | [O sistema deve suportar 1000 usuarios simultaneos] | Escalabilidade |

---

## 3. Metas de Design de Interface

### 3.1 Visao Geral de UX
[Descreva a visao de experiencia do usuario - minimalista, gamificada, profissional, etc.]

### 3.2 Paradigmas de Interacao
[Como usuarios interagem - drag-and-drop, formularios, chat, etc.]

### 3.3 Telas e Views Principais
- [ ] Tela de Login/Registro
- [ ] Dashboard Principal
- [ ] [Tela especifica do produto 1]
- [ ] [Tela especifica do produto 2]
- [ ] Configuracoes

### 3.4 Acessibilidade
- [ ] WCAG AA
- [ ] WCAG AAA
- [ ] Requisitos customizados: [especificar]

### 3.5 Branding
[Elementos de marca, paleta de cores, guias de estilo]

### 3.6 Plataformas-Alvo
- [ ] Web Responsivo
- [ ] Mobile (iOS/Android)
- [ ] Desktop
- [ ] [Outra plataforma]

---

## 4. Premissas Tecnicas

### 4.1 Estrutura de Repositorio
- [ ] Monorepo
- [ ] Polyrepo

**Justificativa:** [Por que esta escolha]

### 4.2 Arquitetura de Servicos
- [ ] Monolito
- [ ] Microservicos
- [ ] Serverless

**Justificativa:** [Por que esta escolha]

### 4.3 Requisitos de Testes
- [ ] Testes Unitarios
- [ ] Testes de Integracao
- [ ] Testes E2E
- [ ] Testes de Performance

### 4.4 Outras Premissas Tecnicas
- [Premissa tecnica 1]
- [Premissa tecnica 2]

---

## 5. Lista de Epicos

| Epico | Titulo | Objetivo |
|-------|--------|----------|
| E1 | Fundacao e Infraestrutura | Estabelecer setup do projeto, CI/CD e autenticacao basica |
| E2 | [Titulo do Epico 2] | [Objetivo em 1 frase] |
| E3 | [Titulo do Epico 3] | [Objetivo em 1 frase] |
| E4 | [Titulo do Epico 4] | [Objetivo em 1 frase] |

---

## 6. Detalhamento dos Epicos

### Epico 1: Fundacao e Infraestrutura

**Objetivo:** Estabelecer a base do projeto com setup, CI/CD, autenticacao e funcionalidade inicial verificavel.

#### Story 1.1: Setup do Projeto
**Como** desenvolvedor,
**Eu quero** ter o projeto configurado com estrutura basica,
**Para que** eu possa comecar a desenvolver funcionalidades.

**Criterios de Aceitacao:**
1. Repositorio criado com estrutura de pastas definida
2. Dependencias basicas instaladas e configuradas
3. Scripts de build e dev funcionando
4. Lint e formatacao configurados
5. README com instrucoes de setup

---

#### Story 1.2: Pipeline de CI/CD
**Como** desenvolvedor,
**Eu quero** ter um pipeline automatizado,
**Para que** builds e deploys sejam consistentes.

**Criterios de Aceitacao:**
1. Pipeline de CI executando testes em cada PR
2. Build automatico em push para main
3. Deploy automatico para ambiente de staging
4. Notificacoes de falha configuradas

---

#### Story 1.3: Autenticacao Basica
**Como** usuario,
**Eu quero** fazer login no sistema,
**Para que** eu possa acessar funcionalidades protegidas.

**Criterios de Aceitacao:**
1. Tela de login funcional
2. Registro de novo usuario
3. Recuperacao de senha
4. Tokens JWT implementados
5. Rotas protegidas funcionando

---

### Epico 2: [Titulo do Epico]

**Objetivo:** [Descreva o objetivo expandido do epico em 2-3 frases]

#### Story 2.1: [Titulo da Story]
**Como** [tipo de usuario],
**Eu quero** [acao],
**Para que** [beneficio].

**Criterios de Aceitacao:**
1. [Criterio testavel 1]
2. [Criterio testavel 2]
3. [Criterio testavel 3]

---

#### Story 2.2: [Titulo da Story]
**Como** [tipo de usuario],
**Eu quero** [acao],
**Para que** [beneficio].

**Criterios de Aceitacao:**
1. [Criterio testavel 1]
2. [Criterio testavel 2]

---

### Epico 3: [Titulo do Epico]

[Repetir estrutura para cada epico...]

---

## 7. Proximos Passos

### Prompt para UX Expert
> Revise este PRD e crie wireframes/mockups para as telas principais listadas na secao 3.3. Foque na experiencia do usuario e nos paradigmas de interacao definidos.

### Prompt para Arquiteto
> Com base neste PRD, crie o Documento de Arquitetura detalhando tech stack, padroes arquiteturais, modelos de dados e estrutura do projeto. Use as premissas tecnicas da secao 4 como ponto de partida.

---

## Checklist de Revisao

- [ ] Todas as metas estao claras e mensuraveis
- [ ] Requisitos funcionais cobrem todas as funcionalidades do MVP
- [ ] Requisitos nao-funcionais estao especificados
- [ ] Epicos estao em ordem logica de implementacao
- [ ] Cada story e independente e entrega valor
- [ ] Criterios de aceitacao sao testaveis
- [ ] Premissas tecnicas estao documentadas

---

> **Gerado com GIPM - Metodo de Projetos com IA Governada**
> https://github.com/inematds/GIPM
