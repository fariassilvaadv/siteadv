# 🏛️ Farias & Silva Advogados Associados

Site institucional e blog do escritório de advocacia **Farias & Silva Advogados Associados**, especializado em Direito Trabalhista.

---

## 📁 Estrutura do Projeto

```
farias-silva-advogados/
├── index.html              # Landing Page principal
├── blog.html               # Página de listagem de artigos
├── blog-post.html          # Template de artigo individual
├── assets/
│   ├── css/
│   │   └── main.css        # Estilos do site
│   ├── js/
│   │   └── main.js         # Funcionalidades e interações
│   └── images/
│       ├── logomarca.png   # Logomarca do escritório
│       ├── foto-albezio.jpg # Foto do sócio Albézio
│       └── foto-filipe.jpg  # Foto do sócio Filipe
└── README.md
```

---

## 🚀 Como Publicar no GitHub Pages

### 1. Criar o Repositório
1. Acesse [github.com](https://github.com) e faça login
2. Clique em **"New repository"**
3. Nomeie como `fariasesilvaadvogados` (ou outro nome de sua preferência)
4. Deixe como **Público**
5. Clique em **"Create repository"**

### 2. Enviar os Arquivos
#### Opção A - Upload direto (mais fácil):
1. No repositório criado, clique em **"Add file" > "Upload files"**
2. Arraste todos os arquivos e pastas do projeto
3. Clique em **"Commit changes"**

#### Opção B - Via Git (para quem tem conhecimento):
```bash
git init
git add .
git commit -m "Primeira versão do site"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/fariasesilvaadvogados.git
git push -u origin main
```

### 3. Ativar o GitHub Pages
1. No repositório, vá em **"Settings"** (aba superior)
2. No menu lateral esquerdo, clique em **"Pages"**
3. Em **"Source"**, selecione a branch `main` e pasta `/ (root)`
4. Clique em **"Save"**
5. Aguarde alguns minutos. Seu site estará disponível em:
   `https://SEU-USUARIO.github.io/fariasesilvaadvogados/`

---

## 🔧 Configurações Importantes

### Google Tag Manager (GTM)
O site já possui o espaço reservado para o GTM. **Você precisa substituir o código:**

1. Acesse [Google Tag Manager](https://tagmanager.google.com/)
2. Crie uma conta e obtenha seu código (formato: `GTM-XXXXXXX`)
3. Substitua **TODAS** as ocorrências de `GTM-XXXXXXX` nos arquivos:
   - `index.html`
   - `blog.html`
   - `blog-post.html`

> São 2 substituições por arquivo (uma no `<head>` e outra no `<body>`).

### Google Analytics 4 (via GTM)
Após configurar o GTM, você pode adicionar a tag do GA4 diretamente pelo painel do Tag Manager, sem precisar editar o código do site.

---

## 📝 Como Criar Novos Posts no Blog

### Passo 1: Duplicar o Template
1. Copie o arquivo `blog-post.html`
2. Renomeie para algo descritivo, ex: `verbas-rescisorias.html`

### Passo 2: Editar o Conteúdo
Altere as seguintes informações no arquivo:

#### Meta Tags SEO:
- `<title>` - Título do artigo
- `<meta name="description">` - Resumo do artigo
- `<meta name="keywords">` - Palavras-chave
- `<meta name="author">` - Nome do autor (Albézio ou Filipe)
- `<link rel="canonical">` - URL completa do novo post
- Tags Open Graph (`og:title`, `og:description`, etc.)
- Tags Twitter (`twitter:title`, etc.)

#### Structured Data (Schema.org):
- No script `application/ld+json` do tipo **Article**, atualize:
  - `headline`
  - `description`
  - `datePublished` e `dateModified`
  - `author`
  - `@id` em `mainEntityOfPage`

#### FAQ Schema (para Google IA):
- Atualize as perguntas e respostas no schema do tipo **FAQPage**
- Isso ajuda o artigo a aparecer nos resultados de "Perguntas Frequentes" do Google

#### Conteúdo do Artigo:
- Atualize o `<header>` com título, data, autor e tags
- Substitua o conteúdo dentro da tag `<article class="blog-post-content">`
- Use tags semânticas: `<h2>`, `<h3>`, `<p>`, `<ul>`, `<blockquote>`

### Passo 3: Adicionar à Lista do Blog
No arquivo `blog.html`, adicione um novo `<article class="blog-list-item">` seguindo o modelo dos existentes.

### Passo 4: Commit e Publicação
Envie os novos arquivos para o GitHub. O site será atualizado automaticamente em poucos minutos.

---

## 🎨 Personalização de Cores

As cores do site estão baseadas na logomarca. Se desejar alterar, edite o arquivo `assets/css/main.css` nas variáveis CSS no início do arquivo:

```css
:root {
  --primary: #1a6b6b;      /* Cor principal (teal escuro) */
  --primary-dark: #145252;  /* Variante mais escura */
  --primary-light: #2d8a8a; /* Variante mais clara */
  --accent: #4ecdc4;        /* Cor de destaque */
  --accent-light: #e8f4f4;  /* Fundo claro */
  --dark: #1a1a2e;          /* Texto escuro */
  --gold: #c9a227;          /* Detalhes dourados (opcional) */
}
```

---

## 📱 Recursos do Site

- ✅ **Design Responsivo** - Funciona em desktop, tablet e mobile
- ✅ **SEO Otimizado** - Meta tags, Schema.org, Open Graph, Twitter Cards
- ✅ **Google Tag Manager** - Pronto para rastreamento e pixels
- ✅ **Botão WhatsApp Flutuante** - Com mensagem pré-definida
- ✅ **Animações Suaves** - Scroll reveal e transições
- ✅ **Menu Mobile** - Hambúrguer com animação
- ✅ **Schema.org Completo** - LegalService, Article, FAQPage, Blog
- ✅ **Acessibilidade** - ARIA labels, roles semânticos, contraste adequado
- ✅ **Performance** - Imagens com lazy loading, CSS otimizado

---

## 📞 Contato do Escritório

- **WhatsApp:** (81) 99189-4349
- **Email:** contato@fariasesilvaadv.com.br
- **Localização:** Recife, PE - Brasil

---

## ⚖️ Aviso Legal

Este site é de uso exclusivo do escritório Farias & Silva Advogados Associados. Todo o conteúdo jurídico é protegido por direitos autorais. O conteúdo dos artigos tem caráter informativo e não constitui consultoria jurídica personalizada.

---

*Desenvolvido com dedicação para Farias & Silva Advogados Associados.*
