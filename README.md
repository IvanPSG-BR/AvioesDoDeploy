# Aviões do Deploy

Bem-vindo ao repositório da landing page da **Aviões do Deploy** — a comunidade que transforma eventos em projetos reais!

## 🎯 Propósito do Site

A Aviões do Deploy é uma comunidade focada em **aprendizado prático através de hacathons e projetos reais**. Este site funciona como o ponto de entrada para conhecer o movimento, entender nossos valores, explorar os projetos em desenvolvimento e descobrir como se juntar a um time pequeno com ideias grandes.

O objetivo é criar uma experiência envolvente que comunique nossa missão: aprenda fazendo com a comunidade Aviões do Deploy.

## 🛠️ Stack Técnica

- **Framework**: [Astro 5.18.0](https://astro.build/) — site estático rápido e moderno
- **Gerenciador de Pacotes**: [pnpm](https://pnpm.io/)
- **Linguagem**: Astro (`.astro`) com JavaScript/TypeScript
- **Styling**: CSS customizado (sem framework CSS no momento)
- **Fontes**: Google Fonts (Inter, Fira Code)
- **Ícones**: Bootstrap Icons

## 📦 Estrutura do Projeto

```
src/
├── components/          # Componentes Astro reutilizáveis
│   ├── Header.astro     # Navegação principal
│   ├── Hero.astro       # Seção de apresentação
│   ├── Values.astro     # Valores da comunidade
│   ├── Projects.astro   # Galeria de projetos
│   ├── TeamGrid.astro   # Grid do time
│   ├── HowToJoin.astro  # Call-to-action para participação
│   └── Footer.astro     # Rodapé
├── pages/
│   ├── index.astro      # Página principal
│   └── manifesto.astro  # Página com manifesto
└── styles/
    └── global.css       # Estilos globais

public/
├── favicon.webp         # Ícone do site
├── global.css           # CSS global adicional
└── manifesto.pdf        # PDF do manifesto
```

## 🚀 Como Começar

### 1. Instalar Dependências

```bash
pnpm install
```

### 2. Iniciar Desenvolvimento

```bash
pnpm run dev
```

O site estará disponível em `http://localhost:3000` com hot reload automático.

### 3. Build para Produção

```bash
pnpm run build
```

Isso gera a versão otimizada em `dist/`.

### 4. Visualizar Preview da Build

```bash
pnpm run preview
```

Testa a versão de produção localmente.

## 📝 Scripts Disponíveis

| Script | Comando | Descrição |
|--------|---------|-----------|
| **dev** | `pnpm run dev` | Inicia servidor de desenvolvimento com hot reload |
| **build** | `pnpm run build` | Gera build otimizada para produção |
| **preview** | `pnpm run preview` | Visualiza a build de produção localmente |

## 🌐 Deploy

O site é totalmente estático e pode ser deployado em qualquer plataforma que suporte conteúdo HTML/CSS/JS:

### Vercel
```bash
npm install -g vercel
vercel
```

### Netlify
```bash
npm install -g netlify-cli
netlify deploy --prod --dir=dist
```

### Outros Hosts
Faça upload da pasta `dist/` gerada após `pnpm run build`.

## 🧩 Trabalhando com Componentes

Cada componente Astro em `src/components/` é independente e pode ser importado diretamente em páginas:

```astro
---
import Hero from '../components/Hero.astro';
---

<Hero />
```

Os componentes não requerem hidratação JavaScript por padrão (renderização estática), mantendo o site rápido e leve.

## 📋 Variáveis de Ambiente

Não há variáveis de ambiente obrigatórias no momento. Se precisar adicionar no futuro:

```bash
# .env
PUBLIC_SITE_URL=https://avioesdodeploy.dev
```

## 🔗 Recursos Úteis

- [Documentação do Astro](https://docs.astro.build/)
- [Google Fonts](https://fonts.google.com/)
- [Bootstrap Icons](https://icons.getbootstrap.com/)

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para detalhes.

---

**Aviões do Deploy** — Do Aeroporto para o Mundo! ✈️
