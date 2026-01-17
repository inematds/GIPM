# QA Gate - Checklist de Qualidade

> **Template de Quality Gate GIPM**
> Checklist para validar que cada entrega atende aos padroes de qualidade.

---

## Informacoes da Entrega

| Campo | Valor |
|-------|-------|
| **Story/Feature:** | [Numero e titulo] |
| **Branch:** | [Nome da branch] |
| **Autor:** | [Nome] |
| **Data:** | [Data] |
| **Revisor QA:** | [Nome] |

---

## 1. Validacao de Criterios de Aceitacao

### AC Checklist

| # | Criterio | Status | Evidencia |
|---|----------|--------|-----------|
| 1 | [Criterio 1] | [ ] Pass / [ ] Fail | [Screenshot/Link] |
| 2 | [Criterio 2] | [ ] Pass / [ ] Fail | [Screenshot/Link] |
| 3 | [Criterio 3] | [ ] Pass / [ ] Fail | [Screenshot/Link] |
| 4 | [Criterio 4] | [ ] Pass / [ ] Fail | [Screenshot/Link] |
| 5 | [Criterio 5] | [ ] Pass / [ ] Fail | [Screenshot/Link] |

### Resultado AC
- [ ] **PASS** - Todos os AC validados
- [ ] **FAIL** - AC pendentes (listar abaixo)

**AC com Falha:**
- [Listar AC que falharam e motivo]

---

## 2. Validacao de Codigo

### 2.1 Code Review
- [ ] PR criado e linkado
- [ ] Descricao do PR clara e completa
- [ ] Commits atomicos e bem descritos
- [ ] Sem arquivos desnecessarios (logs, .env, etc)

### 2.2 Padroes de Codigo
- [ ] Lint sem erros (`npm run lint`)
- [ ] Formatacao correta (`npm run format:check`)
- [ ] TypeScript strict mode sem erros
- [ ] Sem `any` types (ou justificado)
- [ ] Nomenclatura seguindo convencoes

### 2.3 Arquitetura
- [ ] Codigo no local correto (seguindo estrutura de pastas)
- [ ] Padroes arquiteturais respeitados
- [ ] Sem logica de negocio em controllers
- [ ] Dependencias injetadas corretamente
- [ ] Sem acoplamento desnecessario

---

## 3. Testes

### 3.1 Testes Unitarios
- [ ] Testes unitarios escritos
- [ ] Coverage minimo atingido (80%)
- [ ] Todos os testes passando
- [ ] Casos de erro cobertos
- [ ] Mocks apropriados usados

**Coverage Report:**
```
File              | % Stmts | % Branch | % Funcs | % Lines |
------------------|---------|----------|---------|---------|
[file.ts]         | [%]     | [%]      | [%]     | [%]     |
```

### 3.2 Testes de Integracao
- [ ] Testes de integracao escritos (se aplicavel)
- [ ] Database interactions testadas
- [ ] APIs externas mockadas
- [ ] Todos os testes passando

### 3.3 Testes E2E
- [ ] Fluxos criticos testados (se aplicavel)
- [ ] Todos os testes passando

### Resultado Testes
- [ ] **PASS** - Todos os testes passando
- [ ] **FAIL** - Testes falhando (listar abaixo)

**Testes com Falha:**
- [Listar testes que falharam]

---

## 4. Seguranca

### 4.1 Validacao de Input
- [ ] Todos os inputs de usuario validados
- [ ] Sanitizacao contra XSS
- [ ] Protecao contra SQL Injection
- [ ] Validacao de tipos e formatos

### 4.2 Autenticacao/Autorizacao
- [ ] Endpoints protegidos adequadamente
- [ ] Verificacao de permissoes implementada
- [ ] Tokens validados corretamente

### 4.3 Dados Sensiveis
- [ ] Nenhum secret hardcoded
- [ ] PII nao exposta em logs
- [ ] Senhas/tokens nao retornados em responses

### 4.4 Scan de Vulnerabilidades
- [ ] `npm audit` sem vulnerabilidades criticas
- [ ] Dependencias atualizadas

### Resultado Seguranca
- [ ] **PASS** - Sem issues de seguranca
- [ ] **FAIL** - Issues encontrados (listar abaixo)

**Issues de Seguranca:**
- [Listar problemas encontrados]

---

## 5. Performance

### 5.1 Metricas
- [ ] Tempo de resposta da API < [X]ms
- [ ] Queries otimizadas (sem N+1)
- [ ] Indexes apropriados usados
- [ ] Sem memory leaks identificados

### 5.2 Load Testing (se aplicavel)
- [ ] Suporta carga esperada
- [ ] Sem degradacao significativa

### Resultado Performance
- [ ] **PASS** - Performance aceitavel
- [ ] **FAIL** - Issues de performance (listar abaixo)

**Issues de Performance:**
- [Listar problemas encontrados]

---

## 6. Documentacao

### 6.1 Codigo
- [ ] Funcoes complexas documentadas
- [ ] JSDoc/TSDoc em APIs publicas
- [ ] README atualizado (se necessario)

### 6.2 API
- [ ] Endpoints documentados (Swagger/OpenAPI)
- [ ] Exemplos de request/response
- [ ] Codigos de erro documentados

### 6.3 Projeto
- [ ] Story atualizada com notas de dev
- [ ] Changelog atualizado
- [ ] Arquitetura reflete mudancas (se necessario)

### Resultado Documentacao
- [ ] **PASS** - Documentacao adequada
- [ ] **FAIL** - Documentacao pendente

---

## 7. Integracao

### 7.1 Build
- [ ] Build local passando
- [ ] CI/CD pipeline passando
- [ ] Sem warnings de build

### 7.2 Deploy
- [ ] Deploy em staging bem-sucedido
- [ ] Smoke tests passando
- [ ] Rollback testado (se aplicavel)

### Resultado Integracao
- [ ] **PASS** - Integracao OK
- [ ] **FAIL** - Problemas de integracao

---

## 8. Checklist Final

### Pre-Merge
- [ ] Todos os checks acima passando
- [ ] Aprovacao de code review obtida
- [ ] Branch atualizada com main/develop
- [ ] Conflitos resolvidos
- [ ] Story atualizada para "Review"

### Aprovacao

| Papel | Nome | Aprovado | Data |
|-------|------|----------|------|
| Dev | [Nome] | [ ] | [Data] |
| QA | [Nome] | [ ] | [Data] |
| Tech Lead | [Nome] | [ ] | [Data] |

---

## Resultado Final

### Status
- [ ] **APROVADO** - Pronto para merge
- [ ] **REJEITADO** - Requer correcoes
- [ ] **BLOQUEADO** - Aguardando dependencia

### Notas
[Observacoes gerais do QA, recomendacoes, debitos tecnicos identificados]

### Proximos Passos
1. [Acao necessaria]
2. [Acao necessaria]

---

## Bugs Identificados

| ID | Descricao | Severidade | Bloqueante | Status |
|----|-----------|------------|------------|--------|
| B1 | [Descricao] | Critica/Alta/Media/Baixa | Sim/Nao | Aberto/Resolvido |
| B2 | [Descricao] | Critica/Alta/Media/Baixa | Sim/Nao | Aberto/Resolvido |

---

## Historico

| Data | Acao | Responsavel |
|------|------|-------------|
| [Data] | QA iniciado | [Nome] |
| [Data] | Issues reportados | [Nome] |
| [Data] | Correcoes aplicadas | [Nome] |
| [Data] | QA aprovado | [Nome] |

---

> **Gerado com GIPM - Metodo de Projetos com IA Governada**
> https://github.com/inematds/GIPM
