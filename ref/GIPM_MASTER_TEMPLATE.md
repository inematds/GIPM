# GIPM Master - Template de Referencia

> **Documento Padrao** - Regras e templates para o curso GIPM Master
> **Versao:** 1.0 | **Data:** 2026-01-16

---

## Indice

- [Estrutura do Curso](#estrutura-do-curso)
- [Cores por Trilha](#cores-por-trilha)
- [Navegacao Global](#navegacao-global)
- [Estrutura de Pagina de Trilha](#estrutura-de-pagina-de-trilha)
- [Estrutura de Pagina de Modulo](#estrutura-de-pagina-de-modulo)
- [Componentes](#componentes)
- [Templates HTML](#templates-html)
- [Checklist de Qualidade](#checklist-de-qualidade)

---

## Estrutura do Curso

```
GIPM Master
├── 5 Trilhas
│   ├── T1: Fundamentos (Emerald) - 8 modulos
│   ├── T2: O Metodo (Blue) - 10 modulos
│   ├── T3: Aplicacao Avancada (Purple) - 8 modulos
│   ├── T4: Projeto NotebookLMX (Amber) - 10 modulos
│   └── T5: Exercicio Pratico (Teal) - 10 modulos
├── 46 Modulos totais
├── ~300 Topicos
└── 6-8 Topicos por Modulo
```

---

## Cores por Trilha

| Trilha | Nome | Cor | Classes Tailwind |
|--------|------|-----|------------------|
| T1 | Fundamentos | Emerald | `text-emerald-400`, `bg-emerald-500/20`, `border-emerald-500/30` |
| T2 | O Metodo | Blue | `text-blue-400`, `bg-blue-500/20`, `border-blue-500/30` |
| T3 | Aplicacao Avancada | Purple | `text-purple-400`, `bg-purple-500/20`, `border-purple-500/30` |
| T4 | Projeto NotebookLMX | Amber | `text-amber-400`, `bg-amber-500/20`, `border-amber-500/30` |
| T5 | Exercicio Pratico | Teal | `text-teal-400`, `bg-teal-500/20`, `border-teal-500/30` |

### Cores Especiais

| Cor | Codigo | Uso |
|-----|--------|-----|
| Primary (Yellow) | `#FACC15` | Logo, CTAs, destaques |
| Sky | `text-sky-400` | Link INEMA.CLUB |
| Neutral | `text-neutral-300/400` | Texto secundario |

---

## Navegacao Global

**OBRIGATORIO em TODAS as paginas:**

1. Logo: `🎓 GIPM Master` (yellow-400)
2. Link: `INEMA.CLUB` (sky-400)
3. Trilhas: Fundamentos | O Metodo | Avancado | NotebookLMX | Pratico
4. Theme Toggle: dark/light

```html
<nav class="sticky top-0 z-50 bg-dark-900/95 backdrop-blur-sm border-b border-dark-600">
  <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-14">
      <!-- Logo + INEMA.CLUB -->
      <div class="flex items-center space-x-4">
        <a href="../../index.html" class="flex items-center space-x-2 text-yellow-400 hover:text-yellow-300">
          <span class="text-2xl">🎓</span>
          <span class="font-bold text-lg hidden sm:inline">GIPM Master</span>
        </a>
        <span class="text-neutral-600">|</span>
        <a href="https://inema.club" target="_blank" class="text-sky-400 hover:text-sky-300 text-sm font-medium">INEMA.CLUB</a>
      </div>

      <!-- Trilhas + Theme Toggle -->
      <div class="flex items-center space-x-1 sm:space-x-2">
        <!-- Trilhas aqui -->
        <button id="theme-toggle">...</button>
      </div>
    </div>
  </div>
</nav>
```

---

## Estrutura de Pagina de Trilha

```
TRILHA INDEX
├── Navigation Global (com INEMA.CLUB)
├── Header
│   └── Badge da trilha (TRILHA X)
│   └── Titulo + emoji
│   └── Descricao
│   └── Stats (Modulos, Topicos, Duracao, Nivel)
├── Modulos (cards)
│   └── Modulo Card
│       ├── Header (numero, titulo, descricao, duracao)
│       ├── Topicos Expansiveis (6-8 por modulo)
│       │   └── Numero em CIRCULO (nao seta!)
│       │   └── Emoji + titulo + subtitulo
│       │   └── Conteudo com 3 secoes:
│       │       ├── O que e
│       │       ├── Por que aprender
│       │       └── Conceitos-chave
│       └── Botoes (ESQUERDA - justify-start)
│           ├── 📖 Ver em Modal
│           └── 📄 Ver Completo
├── Navegacao (Voltar | Proxima Trilha)
└── Footer
```

---

## Estrutura de Pagina de Modulo

```
MODULO COMPLETO
├── Navigation Global (com INEMA.CLUB)
├── Breadcrumb (Inicio / Trilha X / Modulo X.X)
├── Header
│   └── Badge (MODULO X.X)
│   └── Titulo + emoji
│   └── Descricao
│   └── Stats (Topicos, Minutos, Nivel, Tipo)
├── Topicos (6 secoes ricas)
│   └── Section por topico
│       ├── Numero em circulo grande + titulo
│       ├── Paragrafo introdutorio
│       ├── Boxes de conteudo:
│       │   ├── Conceito Principal (gradiente da trilha)
│       │   ├── Dados/Pesquisa (blue)
│       │   ├── Dica Pratica (primary/yellow)
│       │   ├── Grid Fazer vs Evitar (emerald/red)
│       │   ├── Timeline de casos/passos
│       │   └── Box de alerta (red)
│       └── Espacamento: mb-16 entre topicos
├── Resumo Final
│   └── Checklist do que aprendemos
│   └── Proximo modulo
│   └── CTAs de navegacao
└── Footer
```

---

## Componentes

### Numero em Circulo (Topico Pequeno)

```html
<span class="w-6 h-6 rounded-full bg-emerald-500/20 text-emerald-400 text-sm font-bold flex items-center justify-center flex-shrink-0">1</span>
```

### Numero em Circulo (Topico Grande)

```html
<span class="flex items-center justify-center w-12 h-12 rounded-full bg-emerald-500/20 text-emerald-400 font-bold text-xl">1</span>
```

### Conteudo do Topico Expansivel (3 Secoes)

```html
<div class="bg-dark-700/50 rounded-lg p-4 space-y-3 ml-9">
  <div>
    <span class="text-emerald-400 font-semibold">O que e:</span>
    <p class="text-neutral-300 text-sm">Definicao clara...</p>
  </div>
  <div>
    <span class="text-emerald-400 font-semibold">Por que aprender:</span>
    <p class="text-neutral-300 text-sm">Beneficios praticos...</p>
  </div>
  <div>
    <span class="text-emerald-400 font-semibold">Conceitos-chave:</span>
    <p class="text-neutral-300 text-sm">Lista de termos...</p>
  </div>
</div>
```

### Botoes do Modulo (ESQUERDA)

```html
<div class="p-4 bg-dark-700/30 flex justify-start space-x-3">
  <button onclick="openModal('modal-X-X')" class="px-4 py-2 text-sm bg-dark-600 hover:bg-dark-500 rounded-lg transition-colors">
    📖 Ver em Modal
  </button>
  <a href="modulo-X-X.html" class="px-4 py-2 text-sm bg-emerald-600 hover:bg-emerald-500 text-white rounded-lg transition-colors">
    📄 Ver Completo
  </a>
</div>
```

### Box Conceito Principal

```html
<div class="bg-gradient-to-br from-emerald-900/30 to-dark-800 rounded-xl border border-emerald-500/30 p-6 mb-6">
  <h3 class="text-lg font-semibold text-emerald-400 mb-4 flex items-center">
    <span class="mr-2">📋</span> Titulo
  </h3>
  <!-- conteudo -->
</div>
```

### Box Dados/Pesquisa

```html
<div class="bg-blue-900/20 rounded-xl border border-blue-500/30 p-6 mb-6">
  <h3 class="text-lg font-semibold text-blue-400 mb-4 flex items-center">
    <span class="mr-2">📊</span> Dados de Pesquisa
  </h3>
  <!-- conteudo -->
</div>
```

### Box Dica Pratica

```html
<div class="bg-primary/10 rounded-xl border border-primary/30 p-6">
  <h3 class="text-lg font-semibold text-primary mb-3 flex items-center">
    <span class="mr-2">💡</span> Dica Pratica
  </h3>
  <p class="text-neutral-300">Texto da dica...</p>
</div>
```

### Grid Fazer vs Evitar

```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-6">
  <div class="bg-emerald-900/20 rounded-xl border border-emerald-500/30 p-6">
    <h4 class="font-bold text-emerald-400 mb-4">✓ O que FAZER</h4>
    <ul class="space-y-3 text-neutral-300">
      <li class="flex items-start space-x-2">
        <span class="text-emerald-400">✓</span>
        <span>Item positivo</span>
      </li>
    </ul>
  </div>
  <div class="bg-red-900/20 rounded-xl border border-red-500/30 p-6">
    <h4 class="font-bold text-red-400 mb-4">✗ O que NAO fazer</h4>
    <ul class="space-y-3 text-neutral-300">
      <li class="flex items-start space-x-2">
        <span class="text-red-400">✗</span>
        <span>Item negativo</span>
      </li>
    </ul>
  </div>
</div>
```

### Timeline de Casos

```html
<div class="space-y-6 mb-6">
  <div class="flex items-start space-x-4">
    <div class="flex-shrink-0 w-12 h-12 rounded-full bg-red-500/20 flex items-center justify-center">
      <span class="text-red-400 font-bold">1</span>
    </div>
    <div class="flex-1 bg-dark-800 rounded-xl p-6 border border-dark-600">
      <h4 class="font-semibold text-white mb-2">Titulo do Caso</h4>
      <p class="text-sm text-neutral-400 mb-3">Contexto</p>
      <p class="text-neutral-300 text-sm">Descricao...</p>
    </div>
  </div>
</div>
```

### Resumo do Modulo

```html
<section class="mb-12">
  <div class="bg-gradient-to-br from-emerald-900/40 via-dark-800 to-dark-800 rounded-xl border border-emerald-500/30 p-8">
    <h2 class="text-2xl font-bold mb-6 flex items-center">
      <span class="mr-3">📝</span> Resumo do Modulo
    </h2>

    <div class="space-y-4 mb-8">
      <div class="flex items-start space-x-3">
        <span class="text-emerald-400 mt-1">✓</span>
        <div>
          <strong class="text-white">Ponto principal</strong>
          <span class="text-neutral-400"> - Explicacao breve</span>
        </div>
      </div>
    </div>

    <div class="flex flex-col sm:flex-row gap-4">
      <a href="index.html" class="flex-1 text-center px-6 py-3 bg-dark-700 text-neutral-300 rounded-lg font-semibold hover:bg-dark-600 transition-colors">
        ← Voltar para Trilha
      </a>
      <a href="modulo-X-Y.html" class="flex-1 text-center px-6 py-3 bg-emerald-600 text-white rounded-lg font-semibold hover:bg-emerald-500 transition-colors">
        Proximo Modulo →
      </a>
    </div>
  </div>
</section>
```

---

## Templates HTML

### Estrutura Base

```html
<!DOCTYPE html>
<html lang="pt-BR" class="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>[Titulo] | GIPM Master</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          colors: {
            primary: '#FACC15',
            dark: { 900: '#111827', 800: '#1f2937', 700: '#374151', 600: '#4b5563' }
          }
        }
      }
    }
  </script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    body { font-family: 'Inter', sans-serif; }
    .dark body { background-color: #111827; }
    .topic-explanation { display: none; }
    .topic-explanation.active { display: block; }

    /* Light mode overrides */
    html:not(.dark) body {
      background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 50%, #f1f5f9 100%);
    }
    html:not(.dark) .bg-dark-900 { background-color: #ffffff; }
    html:not(.dark) .bg-dark-800 { background-color: #f9fafb; }
    html:not(.dark) .bg-dark-700 { background-color: #f3f4f6; }
    html:not(.dark) .bg-dark-600 { background-color: #e5e7eb; }
    html:not(.dark) .text-neutral-100 { color: #111827; }
    html:not(.dark) .text-neutral-300 { color: #4b5563; }
    html:not(.dark) .text-neutral-400 { color: #6b7280; }
    html:not(.dark) .text-neutral-500 { color: #9ca3af; }
    html:not(.dark) .border-dark-600 { border-color: #d1d5db; }
    html:not(.dark) .border-dark-700 { border-color: #e5e7eb; }
  </style>
</head>
<body class="bg-dark-900 text-neutral-100 min-h-screen">
  <!-- Conteudo -->
</body>
</html>
```

### JavaScript Necessario

```javascript
// Theme Toggle
const themeToggle = document.getElementById('theme-toggle');
const themeToggleDarkIcon = document.getElementById('theme-toggle-dark-icon');
const themeToggleLightIcon = document.getElementById('theme-toggle-light-icon');
const html = document.documentElement;

if (localStorage.getItem('theme') === 'light' || (!localStorage.getItem('theme') && !html.classList.contains('dark'))) {
  themeToggleDarkIcon.classList.remove('hidden');
  html.classList.remove('dark');
} else {
  themeToggleLightIcon.classList.remove('hidden');
}

themeToggle.addEventListener('click', () => {
  themeToggleDarkIcon.classList.toggle('hidden');
  themeToggleLightIcon.classList.toggle('hidden');
  html.classList.toggle('dark');
  localStorage.setItem('theme', html.classList.contains('dark') ? 'dark' : 'light');
});

// Toggle Topics
function toggleTopic(button) {
  const topicItem = button.closest('.topic-item');
  const explanation = topicItem.querySelector('.topic-explanation');
  const moduleCard = button.closest('.bg-dark-800');

  moduleCard.querySelectorAll('.topic-explanation.active').forEach(exp => {
    if (exp !== explanation) {
      exp.classList.remove('active');
    }
  });

  explanation.classList.toggle('active');
}
```

---

## Checklist de Qualidade

### Antes de Publicar

**Estrutura:**
- [ ] Navigation com INEMA.CLUB (sky-400)
- [ ] Trilhas com nomes completos (Fundamentos, O Metodo, Avancado, NotebookLMX, Pratico)
- [ ] Header completo (badge, titulo, descricao)
- [ ] Stats banner com 4 metricas
- [ ] Topicos com NUMEROS em circulo (nao setas)
- [ ] 3 secoes por topico (O que e, Por que, Conceitos)
- [ ] Botoes a ESQUERDA (justify-start)
- [ ] Resumo/checklist no final
- [ ] Breadcrumb em paginas de modulo

**Visual:**
- [ ] Cores seguem o padrao da trilha
- [ ] Emojis usados consistentemente
- [ ] Dark/light mode funcionando
- [ ] Light mode CSS incluido

**Tecnico:**
- [ ] Links funcionando
- [ ] Responsivo em mobile
- [ ] Modal carrega conteudo
- [ ] Theme toggle funcional

---

## Estrutura de Arquivos

```
gipm-master/
├── index.html                    # Landing page
├── curso/
│   ├── trilha1/                  # Fundamentos (Emerald)
│   │   ├── index.html            # Index da trilha
│   │   ├── modulo-1-1.html       # O Problema da IA Desgovernada
│   │   ├── modulo-1-2.html       # O que e o GIPM
│   │   └── ...
│   ├── trilha2/                  # O Metodo (Blue)
│   ├── trilha3/                  # Aplicacao Avancada (Purple)
│   ├── trilha4/                  # Projeto NotebookLMX (Amber)
│   └── trilha5/                  # Exercicio Pratico (Teal)
├── ref/                          # Documentos de referencia
│   └── GIPM_MASTER_TEMPLATE.md   # Este documento
└── assets/
    ├── css/
    └── js/
```

---

**Ultima atualizacao:** 2026-01-16
**Versao:** 1.0
**Projeto:** GIPM Master
