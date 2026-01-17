# Story [Epic].[Story]: [Titulo da Story]

> **Template de User Story GIPM**
> Documenta requisitos, criterios de aceitacao e tracking de implementacao.

---

## Status

- [ ] Draft
- [ ] Approved
- [ ] In Progress
- [ ] Review
- [ ] Done

---

## Story

**Como** [tipo de usuario],
**Eu quero** [acao/funcionalidade],
**Para que** [beneficio/valor].

---

## Criterios de Aceitacao

1. [ ] [Criterio testavel e especifico]
2. [ ] [Criterio testavel e especifico]
3. [ ] [Criterio testavel e especifico]
4. [ ] [Criterio testavel e especifico]
5. [ ] [Criterio testavel e especifico]

---

## Tarefas / Subtarefas

- [ ] **Task 1:** [Descricao] (AC: 1, 2)
  - [ ] Subtask 1.1: [Descricao]
  - [ ] Subtask 1.2: [Descricao]

- [ ] **Task 2:** [Descricao] (AC: 3)
  - [ ] Subtask 2.1: [Descricao]

- [ ] **Task 3:** [Descricao] (AC: 4, 5)
  - [ ] Subtask 3.1: [Descricao]
  - [ ] Subtask 3.2: [Descricao]

- [ ] **Task 4:** Escrever testes (Todos AC)
  - [ ] Testes unitarios
  - [ ] Testes de integracao (se aplicavel)

---

## Notas de Desenvolvimento

### Arquivos Relevantes
```
src/
├── modules/[module]/
│   ├── [module].controller.ts  # Endpoint da API
│   ├── [module].service.ts     # Logica de negocio
│   └── [module].repository.ts  # Acesso a dados
```

### Tech Stack Relevante
- **Framework:** [NestJS / Express / etc.]
- **Database:** [PostgreSQL / MongoDB / etc.]
- **Validacao:** [class-validator / Zod]

### Padroes a Seguir
- [Padrao 1 do documento de arquitetura]
- [Padrao 2 do documento de arquitetura]

### Dependencias
- Story [X.Y] deve estar completa antes de iniciar
- API externa [X] deve estar disponivel

### Notas da Story Anterior
[Se aplicavel, incluir notas relevantes de stories anteriores]

---

## Testes

### Padroes de Teste
- **Framework:** Jest
- **Localizacao:** `src/modules/[module]/__tests__/`
- **Naming:** `[feature].spec.ts`
- **Coverage:** Minimo 80%

### Casos de Teste Obrigatorios
- [ ] Cenario de sucesso (happy path)
- [ ] Validacao de input invalido
- [ ] Tratamento de erros
- [ ] [Caso especifico desta story]

---

## Historico de Alteracoes

| Data | Versao | Descricao | Autor |
|------|--------|-----------|-------|
| [Data] | 1.0 | Criacao da story | [SM/PO] |
| [Data] | 1.1 | Ajuste nos AC | [Nome] |

---

## Registro do Dev Agent

### Modelo do Agent Usado
[Nome e versao do AI agent/assistente]

### Referencias de Debug Log
[Links ou referencias para logs de debug durante desenvolvimento]

### Notas de Conclusao
- [O que foi implementado]
- [Decisoes tomadas durante desenvolvimento]
- [Problemas encontrados e como foram resolvidos]
- [Debitos tecnicos identificados]

### Lista de Arquivos

#### Criados
- `src/modules/[module]/[file].ts`
- `src/modules/[module]/__tests__/[file].spec.ts`

#### Modificados
- `src/modules/[module]/[module].module.ts`

#### Deletados
- [Nenhum]

---

## Resultados de QA

### Checklist de QA
- [ ] Todos os AC verificados e funcionando
- [ ] Testes passando
- [ ] Code review aprovado
- [ ] Sem vulnerabilidades de seguranca
- [ ] Performance dentro dos limites
- [ ] Documentacao atualizada

### Bugs Encontrados
| Bug | Severidade | Status |
|-----|------------|--------|
| [Descricao] | [Alta/Media/Baixa] | [Aberto/Resolvido] |

### Notas do QA
[Observacoes do time de QA]

### Aprovacao Final
- [ ] QA Aprovado
- [ ] Pronto para merge

---

## Prompt para Criar Esta Story

```
Crie uma User Story para o seguinte requisito:

[Descreva o requisito aqui]

Use o formato:
- As a [usuario]
- I want [acao]
- So that [beneficio]

Inclua:
1. 5 criterios de aceitacao testaveis
2. Tasks e subtasks necessarias
3. Casos de teste obrigatorios
4. Estimativa de complexidade (P/M/G)
```

---

> **Gerado com GIPM - Metodo de Projetos com IA Governada**
> https://github.com/inematds/GIPM
