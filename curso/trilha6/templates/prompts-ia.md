# Prompts para IA - Colecao GIPM

> **Prompts otimizados para usar com Claude, GPT e outros LLMs**
> Cada prompt segue os principios GIPM de governanca e auditabilidade.

---

## Como Usar Esta Colecao

1. **Escolha o prompt** adequado para sua tarefa
2. **Substitua os placeholders** `[texto]` com informacoes do seu projeto
3. **Copie e cole** no seu LLM preferido
4. **Itere** com base nas respostas

### Dica GIPM
Sempre mantenha um registro das conversas com IA para auditabilidade. O humano decide, o sistema valida, a IA executa.

---

## 1. Prompts de Analise de Requisitos

### 1.1 Criar Project Brief

```
Voce e um Business Analyst experiente. Preciso criar um Project Brief para o seguinte projeto:

**Projeto:** [Nome do projeto]
**Contexto:** [Descreva o contexto do negocio]
**Problema:** [Qual problema queremos resolver]
**Publico-alvo:** [Quem sao os usuarios]

Crie um Project Brief completo incluindo:
1. Resumo executivo (2-3 frases)
2. Declaracao do problema com impacto quantificavel
3. Solucao proposta com diferenciais
4. Perfil detalhado dos usuarios-alvo
5. Metas SMART e KPIs
6. Escopo do MVP (must-have vs nice-to-have)
7. Restricoes conhecidas
8. Riscos principais e mitigacoes

Use formato Markdown com secoes claras.
```

### 1.2 Refinar Requisitos

```
Analise os seguintes requisitos de alto nivel e transforme-os em requisitos especificos e testaveis:

**Requisitos de Alto Nivel:**
[Liste os requisitos vagos ou abstratos]

Para cada requisito:
1. Identifique ambiguidades
2. Faca perguntas de esclarecimento
3. Proponha requisitos detalhados com criterios de aceitacao mensuraveis
4. Classifique como Funcional ou Nao-Funcional
5. Priorize usando MoSCoW (Must/Should/Could/Won't)

Formato de saida:
| ID | Requisito Original | Requisito Refinado | Tipo | Prioridade |
```

### 1.3 Analise de Stakeholders

```
Para o projeto [Nome do Projeto], identifique e analise os stakeholders:

**Contexto:** [Descreva o projeto brevemente]

Crie uma matriz de stakeholders incluindo:
1. Identificacao de todos os stakeholders (internos e externos)
2. Nivel de influencia (Alto/Medio/Baixo)
3. Nivel de interesse (Alto/Medio/Baixo)
4. Expectativas principais
5. Estrategia de engajamento recomendada

Apresente em formato de tabela e um quadrante de poder/interesse.
```

---

## 2. Prompts de Arquitetura

### 2.1 Propor Arquitetura de Sistema

```
Voce e um Software Architect senior. Projete a arquitetura para:

**Projeto:** [Nome]
**Tipo:** [Web App / Mobile / API / Microservicos]
**Requisitos Principais:**
- [Requisito 1]
- [Requisito 2]
- [Requisito 3]

**Restricoes:**
- Orcamento: [Alto/Medio/Baixo]
- Time: [Experiencia do time]
- Timeline: [Prazo]

Forneca:
1. Resumo da arquitetura (3-5 frases)
2. Diagrama em Mermaid (graph ou C4)
3. Tech stack recomendada com justificativas
4. Padroes arquiteturais a usar
5. Trade-offs e alternativas consideradas
6. Riscos tecnicos e mitigacoes
```

### 2.2 Revisar Arquitetura Existente

```
Revise a seguinte arquitetura e identifique melhorias:

**Arquitetura Atual:**
[Cole a descricao ou diagrama]

Analise considerando:
1. Escalabilidade - suporta crescimento?
2. Manutenibilidade - facil de evoluir?
3. Seguranca - vulnerabilidades potenciais?
4. Performance - gargalos possiveis?
5. Custo - otimizacoes possiveis?

Para cada problema encontrado:
- Descricao do problema
- Impacto potencial
- Solucao recomendada
- Esforco de implementacao (P/M/G)
```

### 2.3 Design de API

```
Projete uma REST API para:

**Dominio:** [Descreva o dominio]
**Entidades:** [Liste as entidades principais]
**Operacoes:** [O que a API deve fazer]

Forneca:
1. Lista de endpoints com metodos HTTP
2. Estrutura de request/response para cada endpoint
3. Codigos de status HTTP apropriados
4. Estrategia de autenticacao
5. Versionamento da API
6. Especificacao OpenAPI/Swagger parcial

Siga RESTful best practices e inclua exemplos de curl.
```

---

## 3. Prompts de Desenvolvimento

### 3.1 Implementar Feature

```
Implemente a seguinte feature:

**User Story:**
Como [usuario], eu quero [acao] para que [beneficio].

**Criterios de Aceitacao:**
1. [AC1]
2. [AC2]
3. [AC3]

**Tech Stack:**
- [Linguagem/Framework]
- [Database]
- [Outras tecnologias]

**Padroes a seguir:**
- [Padrao 1]
- [Padrao 2]

Forneca:
1. Codigo completo e funcional
2. Testes unitarios
3. Documentacao inline (JSDoc/docstrings)
4. Instrucoes de uso

IMPORTANTE:
- Nao use 'any' types
- Valide todos os inputs
- Trate erros apropriadamente
- Siga os principios SOLID
```

### 3.2 Refatorar Codigo

```
Refatore o seguinte codigo para melhorar qualidade:

```[linguagem]
[Cole o codigo aqui]
```

Objetivos da refatoracao:
- [ ] Melhorar legibilidade
- [ ] Remover duplicacao
- [ ] Aplicar principios SOLID
- [ ] Melhorar performance
- [ ] Adicionar tipagem forte
- [ ] Melhorar tratamento de erros

Forneca:
1. Codigo refatorado
2. Lista de mudancas feitas e justificativas
3. Testes para validar que comportamento nao mudou
4. Metricas de melhoria (se mensuravel)
```

### 3.3 Debug de Codigo

```
Analise e corrija o bug no seguinte codigo:

```[linguagem]
[Cole o codigo com bug]
```

**Comportamento esperado:**
[Descreva o que deveria acontecer]

**Comportamento atual:**
[Descreva o que esta acontecendo]

**Erro/Stack trace (se disponivel):**
[Cole o erro]

Forneca:
1. Identificacao da causa raiz
2. Explicacao de por que o bug ocorre
3. Codigo corrigido
4. Teste que previne regressao
5. Sugestoes para evitar bugs similares
```

---

## 4. Prompts de Testes

### 4.1 Gerar Testes Unitarios

```
Gere testes unitarios para o seguinte codigo:

```[linguagem]
[Cole o codigo]
```

**Framework de teste:** [Jest/Pytest/etc]

Inclua testes para:
1. Cenarios de sucesso (happy path)
2. Casos de borda (edge cases)
3. Tratamento de erros
4. Validacao de inputs
5. Mocks para dependencias externas

Use o padrao AAA (Arrange, Act, Assert).
Garanta coverage > 80%.
```

### 4.2 Criar Plano de Testes

```
Crie um plano de testes para a seguinte feature:

**Feature:** [Nome da feature]
**Descricao:** [O que a feature faz]
**Criterios de Aceitacao:**
1. [AC1]
2. [AC2]

Inclua:
1. **Testes Funcionais**
   - Casos de teste com steps
   - Dados de teste necessarios
   - Resultado esperado

2. **Testes de Integracao**
   - Pontos de integracao a testar
   - Dependencias a mockar

3. **Testes de Regressao**
   - Areas impactadas
   - Testes de smoke

4. **Testes Nao-Funcionais**
   - Performance
   - Seguranca
   - Acessibilidade

Formato tabular para cada categoria.
```

---

## 5. Prompts de Code Review

### 5.1 Review de PR

```
Faca code review do seguinte codigo/PR:

**Contexto:** [O que este codigo faz]
**Arquivos modificados:**
[Liste os arquivos]

**Codigo:**
```[linguagem]
[Cole o codigo]
```

Revise considerando:
1. **Corretude** - O codigo faz o que deveria?
2. **Design** - Esta bem estruturado?
3. **Legibilidade** - E facil de entender?
4. **Performance** - Ha otimizacoes obvias?
5. **Seguranca** - Ha vulnerabilidades?
6. **Testes** - Esta adequadamente testado?
7. **Documentacao** - Esta documentado?

Formato de feedback:
- 🔴 Bloqueante: [descricao]
- 🟡 Sugestao: [descricao]
- 🟢 Elogio: [descricao]
```

---

## 6. Prompts de Documentacao

### 6.1 Gerar Documentacao de API

```
Gere documentacao para a seguinte API:

**Endpoints:**
[Liste os endpoints]

**Codigo do Controller:**
```[linguagem]
[Cole o codigo]
```

Gere:
1. Descricao de cada endpoint
2. Parametros de entrada com tipos e validacoes
3. Formato de response com exemplos
4. Codigos de erro possiveis
5. Exemplos de uso (curl)
6. Formato OpenAPI/Swagger YAML
```

### 6.2 Criar README

```
Crie um README.md para o projeto:

**Nome:** [Nome do projeto]
**Descricao:** [O que o projeto faz]
**Tech Stack:** [Tecnologias usadas]
**Estrutura de pastas:**
[Cole a estrutura]

Inclua secoes:
1. Badges (build, coverage, license)
2. Descricao do projeto
3. Features principais
4. Pre-requisitos
5. Instalacao passo-a-passo
6. Configuracao (variaveis de ambiente)
7. Como executar
8. Como rodar testes
9. Estrutura do projeto
10. Como contribuir
11. Licenca
```

---

## 7. Prompts de DevOps

### 7.1 Criar Pipeline CI/CD

```
Crie um pipeline CI/CD para:

**Projeto:** [Tipo de projeto]
**Plataforma:** [GitHub Actions/GitLab CI/etc]
**Stack:** [Tecnologias]
**Ambientes:** [dev/staging/prod]

O pipeline deve:
1. Rodar em push para branches especificas
2. Instalar dependencias
3. Executar lint
4. Executar testes
5. Build da aplicacao
6. Deploy automatico para ambiente apropriado
7. Notificar em caso de falha

Forneca o arquivo YAML completo com comentarios.
```

### 7.2 Dockerizar Aplicacao

```
Crie Dockerfile e docker-compose para:

**Aplicacao:** [Tipo]
**Stack:** [Tecnologias]
**Servicos necessarios:** [DB, Cache, etc]

Requisitos:
- Multi-stage build para producao
- Imagem final otimizada
- Variaveis de ambiente configuráveis
- Health checks
- Volumes para persistencia
- Network para comunicacao entre servicos

Forneca:
1. Dockerfile com comentarios
2. docker-compose.yml
3. .dockerignore
4. Instrucoes de uso
```

---

## 8. Prompt Master - GIPM Orchestrator

```
Voce e um GIPM Orchestrator - um especialista em governanca de projetos com IA.

Seu papel:
1. Ajudar a definir e estruturar projetos seguindo o metodo GIPM
2. Garantir que todos os artefatos necessarios sejam criados
3. Validar que as decisoes humanas estao documentadas
4. Assegurar auditabilidade completa do projeto

Principios GIPM que voce segue:
1. API-first - Tudo via APIs
2. Backend orquestra, IA executa - IA nunca controla fluxo
3. Regra de duas fases - IA gera estrutura, sistema gera artefatos
4. Persistencia total - Tudo e armazenado
5. Modularidade - Componentes sao substituiveis

**Meu projeto:**
[Descreva o projeto]

**Fase atual:**
[ ] Ideacao
[ ] Requisitos
[ ] Arquitetura
[ ] Desenvolvimento
[ ] Testes
[ ] Deploy

**O que preciso:**
[Descreva sua necessidade]

Ajude-me a avancar mantendo a governanca e documentacao adequadas.
```

---

## Dicas de Uso

### Para Melhores Resultados

1. **Seja especifico** - Quanto mais contexto, melhor a resposta
2. **Use exemplos** - Mostre o formato de saida desejado
3. **Itere** - Refine a resposta com follow-ups
4. **Valide** - Sempre revise o output antes de usar
5. **Documente** - Mantenha registro das conversas

### Formato de Contexto Ideal

```
CONTEXTO:
[Informacoes de background]

OBJETIVO:
[O que voce quer alcancar]

RESTRICOES:
[Limitacoes e requisitos]

FORMATO DE SAIDA:
[Como voce quer a resposta]
```

---

> **Gerado com GIPM - Metodo de Projetos com IA Governada**
> https://github.com/inematds/GIPM
