# Plano do Curso: GIPM Master

## Visão Geral

**Nome:** GIPM Master - Método de Projetos com IA Governada
**Formato:** HTML estático no GitHub Pages
**Link Externo:** INEMA.CLUB (sky-400)

### Configuração de Cores por Trilha

| Trilha | Nome | Cor | Classes Tailwind |
|--------|------|-----|------------------|
| T1 | Fundamentos | Emerald | `text-emerald-400`, `bg-emerald-500/20`, `border-emerald-500/30` |
| T2 | O Método | Blue | `text-blue-400`, `bg-blue-500/20`, `border-blue-500/30` |
| T3 | Aplicação Avançada | Purple | `text-purple-400`, `bg-purple-500/20`, `border-purple-500/30` |
| T4 | Projeto NotebookLMX | Amber | `text-amber-400`, `bg-amber-500/20`, `border-amber-500/30` |
| T5 | Exercício Prático | Teal | `text-teal-400`, `bg-teal-500/20`, `border-teal-500/30` |

---

## TRILHA 1: FUNDAMENTOS (Emerald)
**Subtítulo:** Entenda o Porquê e Como Funciona a Governança de IA

### Módulo 1.1 - O Problema da IA Desgovernada
**6 Tópicos:**
1. 🎯 O que acontece quando IA decide sozinha
2. 💥 Casos reais de falhas por falta de governança
3. 🔍 O mito da IA autônoma
4. ⚠️ Riscos institucionais e regulatórios
5. 💡 A inversão de paradigma: governar vs usar
6. 📊 Custo da imprevisibilidade

### Módulo 1.2 - O que é o GIPM
**6 Tópicos:**
1. 🎯 Definição: Governed Intelligence Project Method
2. 📜 Origem e evolução do método (v1.0 → v1.2)
3. 🏛️ Filosofia central: IA como componente controlado
4. 🎯 Objetivo: sistemas que governam como IA pensa
5. 🌍 Aplicabilidade: setor público, educação, produtos
6. ✅ Benefícios: auditabilidade, previsibilidade, escalabilidade

### Módulo 1.3 - Os 5 Princípios Inalteráveis
**6 Tópicos:**
1. 🔌 Princípio 1: API-first sempre
2. 🎛️ Princípio 2: Backend orquestra, IA executa
3. 📦 Princípio 3: IA gera estrutura, sistema gera artefatos
4. 💾 Princípio 4: Persistência total
5. 🔄 Princípio 5: Modularidade e anti-lock-in
6. 🔒 Por que são inalteráveis

### Módulo 1.4 - Arquitetura de Três Camadas
**6 Tópicos:**
1. 👤 Camada 1: Decisão Humana
2. 🖥️ Camada 2: Sistema (Orquestração)
3. 🤖 Camada 3: IA (Cognição)
4. 🚫 Limites de cada camada
5. 🔀 Fluxo de responsabilidades
6. 📐 Diagrama da arquitetura

### Módulo 1.5 - Mentalidade de Governança
**6 Tópicos:**
1. 🧠 Mudança de mindset: de usuário a governante
2. 🎯 Pensar em políticas, não em prompts
3. 📊 IA como serviço, não como decisor
4. 🔍 Rastreabilidade como valor
5. 💰 Custo como métrica de qualidade
6. 🏢 Visão institucional vs experimental

### Módulo 1.6 - Comparativo: GIPM vs Abordagens Tradicionais
**6 Tópicos:**
1. ⚔️ GIPM vs "Prompt Engineering"
2. ⚔️ GIPM vs Agentes Autônomos
3. ⚔️ GIPM vs No-Code AI Tools
4. ⚔️ GIPM vs LLM direto na aplicação
5. 📊 Matriz comparativa
6. ✅ Quando usar cada abordagem

### Módulo 1.7 - Níveis de Profundidade
**6 Tópicos:**
1. 🔬 Nível Exploratório: protótipos e experimentos
2. ⚙️ Nível Operacional: uso recorrente
3. 🏛️ Nível Institucional: governança forte
4. 📈 Escalonamento de rigor
5. 🔄 Mesmo pipeline, parâmetros diferentes
6. 🎯 Como escolher o nível certo

### Módulo 1.8 - Vocabulário Essencial do GIPM
**6 Tópicos:**
1. 📖 Glossário: Governança, Persona, Pipeline
2. 📖 Glossário: Depth Level, Two-Phase Rule
3. 📖 Glossário: Cognitive Governance, Audit Trail
4. 📖 Glossário: Anti-Lock-In, Reference Implementation
5. 📖 Glossário: Materialização, Persistência
6. 🧪 Quiz de fixação

---

## TRILHA 2: O MÉTODO (Blue)
**Subtítulo:** Cada Componente em Detalhes

### Módulo 2.1 - Pipeline Universal: Visão Geral
**8 Tópicos:**
1. 🔄 O que é o Pipeline Universal
2. 📋 Os 9 passos do pipeline
3. 🎯 Por que todo endpoint segue o mesmo fluxo
4. 🔀 Entrada → Processamento → Saída
5. 📊 Diagrama do pipeline completo
6. 🔗 Interdependência entre passos
7. ⚠️ Erros comuns na implementação
8. ✅ Checklist de validação

### Módulo 2.2 - Pipeline: Passos 1-3 (Entrada)
**6 Tópicos:**
1. 📥 Passo 1: Solicitação do usuário
2. 🔐 Passo 2: Validação de acesso
3. 🗂️ Passo 3: Coleta de contexto
4. 🔀 Fluxo de dados entre passos
5. 💻 Implementação em código
6. 🧪 Exemplos práticos

### Módulo 2.3 - Pipeline: Passos 4-6 (Processamento)
**6 Tópicos:**
1. 📐 Passo 4: Normalização
2. 🎭 Passo 5: Injeção de persona e preferências
3. 🤖 Passo 6: Chamada à IA (estrutura)
4. 🔀 Preparação para chamada LLM
5. 💻 System prompts e contexto
6. 🧪 Exemplos de injeção

### Módulo 2.4 - Pipeline: Passos 7-9 (Saída)
**6 Tópicos:**
1. 💾 Passo 7: Persistência
2. 📦 Passo 8: Materialização
3. ↩️ Passo 9: Retorno
4. 🗃️ Estrutura de armazenamento
5. 🔀 JSON → Artefatos finais
6. 🧪 Exemplos de materialização

### Módulo 2.5 - Governança Cognitiva
**8 Tópicos:**
1. 🧠 O que é Governança Cognitiva
2. 🎭 Personas como políticas de pensamento
3. ⚙️ Preferências persistentes
4. 💉 Injeção automática em toda chamada
5. 📋 Exemplos de personas (Critical Reviewer, Simple Explainer)
6. 🔧 Como criar personas customizadas
7. 🚫 O que personas NÃO são (não é UX)
8. 📊 Medindo eficácia das personas

### Módulo 2.6 - Regra das Duas Fases
**6 Tópicos:**
1. 📐 Fase 1: IA gera estrutura (JSON, outlines)
2. 📦 Fase 2: Sistema gera artefatos (.pptx, .docx, .mp4)
3. 🚫 Por que IA nunca gera arquivos finais
4. 🔄 Fluxo completo da regra
5. 💻 Implementação prática
6. 🧪 Exemplos: roteiro → vídeo

### Módulo 2.7 - Persistência Total
**6 Tópicos:**
1. 💾 O que persistir: inputs, outputs, custos
2. 🗃️ Estrutura de banco de dados
3. 📊 Audit trail completo
4. 🔍 Rastreabilidade de decisões
5. 📈 Aprendizado acumulativo
6. 🔐 Segurança e retenção

### Módulo 2.8 - Governança de Custos
**6 Tópicos:**
1. 💰 Custo como métrica de qualidade
2. 📊 Métricas: por execução, por entrega, por usuário
3. 📈 Dashboard de custos
4. ⚠️ Alertas e limites
5. 🔧 Otimização de chamadas
6. 📋 Relatórios de ROI

### Módulo 2.9 - Filosofia de Falha
**6 Tópicos:**
1. ❌ Simulação = Falha do sistema
2. ❌ Placeholders = Falha do sistema
3. ❌ Dados fictícios = Falha do sistema
4. ✅ Critérios de sucesso
5. 🔍 Validação de outputs
6. 🛠️ Tratamento de erros

### Módulo 2.10 - Implementações de Referência
**6 Tópicos:**
1. 📚 O papel das Reference Implementations
2. 🎯 Ensino, validação e auditoria
3. 📋 Documentação METHOD_MAPPING.md
4. 📋 Documentação COGNITIVE_GOVERNANCE.md
5. 🔍 Como auditar uma implementação
6. ✅ Checklist de conformidade

---

## TRILHA 3: APLICAÇÃO AVANÇADA (Purple)
**Subtítulo:** Dicas e Técnicas para Dominar o GIPM

### Módulo 3.1 - Design de Personas Avançado
**8 Tópicos:**
1. 🎭 Taxonomia de personas
2. 🔧 Personas compostas
3. 🔀 Personas dinâmicas por contexto
4. 📊 Métricas de performance de personas
5. 🧪 A/B testing de personas
6. 📝 Templates de persona
7. ⚠️ Anti-patterns de personas
8. 🎯 Personas para domínios específicos

### Módulo 3.2 - Arquiteturas Avançadas
**8 Tópicos:**
1. 🏗️ Multi-tenant GIPM
2. 🔀 Pipelines paralelos
3. 📊 Event-driven architecture
4. 🗃️ Estratégias de cache
5. 🔄 Async processing
6. 📈 Escalabilidade horizontal
7. 🔐 Security patterns
8. 🌐 Multi-region deployment

### Módulo 3.3 - Integrações e APIs
**6 Tópicos:**
1. 🔌 Padrões de API GIPM
2. 🔄 Webhooks e callbacks
3. 🔗 Integração com sistemas legados
4. 📊 API Gateway patterns
5. 🔐 Authentication & Authorization
6. 📈 Rate limiting e quotas

### Módulo 3.4 - Migração para GIPM
**8 Tópicos:**
1. 📊 Avaliação de sistemas existentes
2. 📋 Roadmap de migração
3. 🔄 Estratégia incremental
4. ⚠️ Riscos e mitigações
5. 🧪 Testes de regressão
6. 📈 Métricas de sucesso
7. 👥 Change management
8. 📝 Documentação de migração

### Módulo 3.5 - GIPM para Diferentes Setores
**6 Tópicos:**
1. 🏛️ Setor Público: compliance e auditoria
2. 🎓 Educação: rastreabilidade acadêmica
3. 🔬 Pesquisa: reprodutibilidade
4. 🏢 Enterprise: governança corporativa
5. 🏥 Saúde: LGPD e regulações
6. 💰 Finanças: audit trail

### Módulo 3.6 - Troubleshooting e Debug
**6 Tópicos:**
1. 🔍 Logs estruturados
2. 🐛 Debug de pipelines
3. 📊 Tracing distribuído
4. ⚠️ Alertas inteligentes
5. 📈 Dashboards de monitoramento
6. 🛠️ Ferramentas recomendadas

### Módulo 3.7 - Performance e Otimização
**6 Tópicos:**
1. ⚡ Otimização de prompts
2. 🗃️ Caching inteligente
3. 📊 Batch processing
4. 🔄 Lazy loading de contexto
5. 💰 Cost optimization
6. 📈 Benchmarking

### Módulo 3.8 - Evolução do Método
**6 Tópicos:**
1. 📜 Histórico de versões
2. 🔮 Roadmap futuro
3. 🤝 Contribuindo para o método
4. 📚 Comunidade GIPM
5. 🎓 Certificação
6. 📈 Tendências em AI Governance

---

## TRILHA 4: PROJETO NotebookLMX (Amber)
**Subtítulo:** Implementação de Referência Completa

### Módulo 4.1 - Visão Geral do NotebookLMX
**6 Tópicos:**
1. 🎯 O que é o NotebookLMX
2. 📋 Funcionalidades principais
3. 🏗️ Arquitetura geral
4. 🔧 Stack tecnológico (FastAPI, Gemini)
5. 📊 Mapeamento GIPM → Implementação
6. 🔍 Como usar como referência

### Módulo 4.2 - Estrutura do Projeto
**6 Tópicos:**
1. 📁 Organização de pastas
2. 📋 Principais arquivos
3. 🔧 Configurações
4. 📊 Dependências
5. 🚀 Setup e instalação
6. 🧪 Ambiente de desenvolvimento

### Módulo 4.3 - Backend: FastAPI e Orquestração
**8 Tópicos:**
1. 🔌 Endpoints principais (/notebooks, /sources, /chat)
2. 🎛️ Router structure
3. 🔐 Validação de acesso
4. 📊 Estado e sessões
5. 🔄 Middleware GIPM
6. 📋 Schemas e modelos
7. ⚠️ Error handling
8. 📈 Logging estruturado

### Módulo 4.4 - Integração com Gemini
**6 Tópicos:**
1. 🤖 Configuração do cliente Gemini
2. 📋 System prompts
3. 🎭 Injeção de personas
4. 📊 Parsing de respostas
5. 💰 Tracking de custos
6. ⚠️ Fallbacks e retry

### Módulo 4.5 - Governança Cognitiva na Prática
**8 Tópicos:**
1. 📁 Arquivo persona_utils.py
2. 🎭 Definição de personas
3. ⚙️ Settings por notebook
4. 💉 Injeção automática
5. 📊 Preferências de output
6. 🔄 Persistência de preferências
7. 🧪 Testando personas
8. 📈 Métricas de uso

### Módulo 4.6 - Pipeline Universal Implementado
**6 Tópicos:**
1. 📥 Request → Validation
2. 🗂️ Context collection
3. 🔄 Normalization
4. 🤖 AI call
5. 💾 Persistence
6. 📦 Materialization

### Módulo 4.7 - Materialização de Artefatos
**8 Tópicos:**
1. 📄 Gerando .docx
2. 📊 Gerando .pptx
3. 🎵 Gerando .mp3 (TTS)
4. 🎬 Gerando .mp4
5. 🔀 JSON → Artefato
6. 📁 Storage e download
7. 🔄 Processamento async
8. ⚠️ Tratamento de erros

### Módulo 4.8 - Persistência e Banco de Dados
**6 Tópicos:**
1. 🗃️ Modelo de dados
2. 📊 Tabelas principais
3. 🔍 Queries de auditoria
4. 📈 Histórico completo
5. 💰 Registro de custos
6. 🔐 Backup e recuperação

### Módulo 4.9 - Frontend e UX
**6 Tópicos:**
1. 🎨 Interface do NotebookLMX
2. 📱 Componentes principais
3. 🔄 Comunicação com API
4. 📊 Exibição de resultados
5. ⚙️ Configuração de preferências
6. 🧪 Testes de usabilidade

### Módulo 4.10 - Deploy e Operação
**6 Tópicos:**
1. 🚀 Deploy options
2. 📊 Monitoring
3. 📈 Métricas de produção
4. 🔐 Security em produção
5. 📋 Runbook operacional
6. 🔄 CI/CD pipeline

---

## TRILHA 5: EXERCÍCIO PRÁTICO (Teal)
**Subtítulo:** Crie Seu Próprio Projeto GIPM

### Módulo 5.1 - Definindo o Projeto
**6 Tópicos:**
1. 🎯 Escolhendo o domínio
2. 📋 Requisitos funcionais
3. 📊 Requisitos não-funcionais
4. 👥 Stakeholders
5. 🔍 Análise de viabilidade
6. 📝 Project brief

### Módulo 5.2 - Arquitetura GIPM do Projeto
**8 Tópicos:**
1. 🏗️ Definindo as 3 camadas
2. 🎭 Desenhando personas
3. 📋 Mapeando o pipeline
4. 📊 Escolha de depth level
5. 🔧 Stack tecnológico
6. 🗃️ Modelo de dados
7. 🔌 Design de APIs
8. 📐 Diagrama de arquitetura

### Módulo 5.3 - Setup do Projeto
**6 Tópicos:**
1. 📁 Estrutura de pastas
2. 🔧 Configuração inicial
3. 📦 Dependências
4. 🐳 Docker setup
5. 🗃️ Banco de dados
6. 🧪 Ambiente de testes

### Módulo 5.4 - Implementando o Pipeline
**8 Tópicos:**
1. 📥 Passo 1-2: Request e validação
2. 🗂️ Passo 3-4: Contexto e normalização
3. 🎭 Passo 5: Injeção de persona
4. 🤖 Passo 6: Chamada à IA
5. 💾 Passo 7: Persistência
6. 📦 Passo 8: Materialização
7. ↩️ Passo 9: Retorno
8. 🧪 Testes do pipeline

### Módulo 5.5 - Implementando Governança Cognitiva
**6 Tópicos:**
1. 🎭 Criando suas personas
2. ⚙️ Sistema de preferências
3. 💉 Mecanismo de injeção
4. 📊 Logs de governança
5. 🧪 Validando comportamento
6. 📈 Métricas de qualidade

### Módulo 5.6 - Materialização de Outputs
**6 Tópicos:**
1. 📊 Definindo formatos de saída
2. 🔧 Implementando geradores
3. 📁 Sistema de storage
4. 🔄 Processamento assíncrono
5. ⚠️ Tratamento de falhas
6. 🧪 Testes de integração

### Módulo 5.7 - Persistência e Auditoria
**6 Tópicos:**
1. 🗃️ Implementando o modelo
2. 📊 CRUD operations
3. 🔍 Queries de auditoria
4. 💰 Tracking de custos
5. 📈 Dashboards
6. 🔐 Compliance

### Módulo 5.8 - Testes e Qualidade
**6 Tópicos:**
1. 🧪 Testes unitários
2. 🧪 Testes de integração
3. 🧪 Testes de pipeline
4. 📊 Coverage
5. 🔍 Code review checklist
6. ✅ Definition of done GIPM

### Módulo 5.9 - Documentação GIPM
**6 Tópicos:**
1. 📋 METHOD_MAPPING.md
2. 📋 COGNITIVE_GOVERNANCE.md
3. 📋 API Documentation
4. 📋 Runbook
5. 📋 Architecture Decision Records
6. ✅ Checklist de documentação

### Módulo 5.10 - Deploy e Apresentação
**6 Tópicos:**
1. 🚀 Preparando para deploy
2. 📊 Configuração de produção
3. 📈 Monitoring setup
4. 🎤 Apresentando o projeto
5. 📋 Entrega final
6. 🏆 Certificação GIPM

---

## RESUMO ESTRUTURAL

| Trilha | Nome | Cor | Módulos | Tópicos/Módulo |
|--------|------|-----|---------|----------------|
| T1 | Fundamentos | Emerald | 8 | 6 cada |
| T2 | O Método | Blue | 10 | 6-8 cada |
| T3 | Aplicação Avançada | Purple | 8 | 6-8 cada |
| T4 | Projeto NotebookLMX | Amber | 10 | 6-8 cada |
| T5 | Exercício Prático | Teal | 10 | 6-8 cada |

**Total:** 5 trilhas, 46 módulos, ~300 tópicos

---

## ESTRUTURA DE ARQUIVOS

```
gipm-master/
├── index.html                    # Landing page
├── curso/
│   ├── trilha1/                  # Fundamentos (Emerald)
│   │   ├── index.html            # Index da trilha
│   │   ├── modulo-1-1.html       # O Problema da IA Desgovernada
│   │   ├── modulo-1-2.html       # O que é o GIPM
│   │   └── ...
│   ├── trilha2/                  # O Método (Blue)
│   │   ├── index.html
│   │   └── ...
│   ├── trilha3/                  # Aplicação Avançada (Purple)
│   │   ├── index.html
│   │   └── ...
│   ├── trilha4/                  # Projeto NotebookLMX (Amber)
│   │   ├── index.html
│   │   └── ...
│   └── trilha5/                  # Exercício Prático (Teal)
│       ├── index.html
│       └── ...
└── assets/
    ├── css/
    └── js/
```

---

## PRÓXIMOS PASSOS

1. **Criar repositório GitHub** para o curso
2. **Criar estrutura base** de pastas e arquivos
3. **Desenvolver templates HTML** seguindo os padrões de referência
4. **Produzir conteúdo** trilha por trilha
5. **Revisar e testar** responsividade e dark/light mode
6. **Deploy** no GitHub Pages

---

## VERIFICAÇÃO

Para validar a implementação:
1. Cada página deve ter navigation com INEMA.CLUB
2. Cada módulo deve ter 6-8 tópicos com círculos numerados
3. Cada tópico deve ter 3 seções: O que é, Por que aprender, Conceitos-chave
4. Cores devem corresponder à trilha
5. Dark/light mode funcionando
6. Responsivo em mobile
7. Links de navegação corretos
