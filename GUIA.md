# 📚 Guia de Uso - NgolaLabs

Bem-vindo ao seu novo site! Este guia vai te ajudar a entender como usar e personalizar o site, mesmo sem conhecimento de programação.

## 📁 Arquivos do Site

Você recebeu 4 arquivos principais:

1. **index.html** - Página inicial (vazia, pronta para você adicionar artigos)
2. **template-artigo.html** - Template limpo para criar seus artigos
3. **sobre.html** - Página sobre você
4. **GUIA.md** - Este arquivo com instruções

## 🎨 Como Personalizar

### 1. Mudar suas informações pessoais

#### Na página "Sobre" (sobre.html):

Abra o arquivo `sobre.html` em qualquer editor de texto (Bloco de Notas, Notepad++, etc) e procure por:

```html
<h1>Sobre Mim</h1>
<p>Engenheiro Veeam Backup | Especialista em Proteção de Dados</p>
```

Substitua "Engenheiro Veeam Backup | Especialista em Proteção de Dados" pelo seu título.

Encontre também:
```html
<a href="mailto:seu-email@exemplo.com" class="contact-link">✉️ Email</a>
```

E substitua "seu-email@exemplo.com" pelo seu email real.

Faça o mesmo para LinkedIn e GitHub.

#### Adicionar sua foto:

Procure por:
```html
<img src="https://via.placeholder.com/200" alt="Sua foto" class="profile-image">
```

Substitua `https://via.placeholder.com/200` pelo link da sua foto (pode usar uma foto do LinkedIn, por exemplo).

### 2. Criar Seu Primeiro Artigo

Para criar um novo artigo:

1. **Copie** o arquivo `template-artigo.html`
2. **Renomeie** para algo descritivo como `meu-primeiro-artigo.html`
3. **Edite** o conteúdo seguindo os comentários no template

O template já vem com exemplos de:
- Títulos e subtítulos
- Parágrafos
- Listas
- Caixas de informação e aviso
- Tags
- Como adicionar imagens

Basta substituir o texto de exemplo pelo seu conteúdo!

### 3. Adicionar o Artigo na Página Inicial

Abra `index.html` e procure por:

```html
<div class="articles">
```

Logo após esta linha, você verá uma mensagem de placeholder. **Substitua** toda a div do placeholder por este código:

```html
<article class="article-card">
    <div class="article-meta">
        <span>📅 SUA DATA</span>
        <span>•</span>
        <span>⏱️ X min leitura</span>
    </div>
    <h2><a href="meu-primeiro-artigo.html">Título do Seu Artigo</a></h2>
    <p class="article-excerpt">
        Um breve resumo do que o artigo aborda. Mantenha em 2-3 linhas.
    </p>
    <div class="tags">
        <span class="tag">Tag1</span>
        <span class="tag">Tag2</span>
    </div>
    <a href="meu-primeiro-artigo.html" class="read-more">Ler artigo completo</a>
</article>
```

**IMPORTANTE:** 
- Substitua `meu-primeiro-artigo.html` pelo nome do arquivo que você criou
- Para adicionar mais artigos, copie todo o bloco `<article>...</article>` e cole novamente

## 🎯 Dicas de Formatação

### Adicionar uma caixa de informação:

```html
<div class="info-box">
    <h4>💡 Dica</h4>
    <p>Seu texto aqui</p>
</div>
```

### Adicionar uma caixa de aviso:

```html
<div class="warning-box">
    <h4>⚠️ Atenção</h4>
    <p>Seu aviso aqui</p>
</div>
```

### Adicionar código inline:

```html
Use <code>este formato</code> para código
```

### Negrito:

```html
<strong>texto em negrito</strong>
```

### Adicionar links:

```html
<a href="https://exemplo.com">texto do link</a>
```

## 🌐 Como Colocar o Site Online

Você tem várias opções GRATUITAS para hospedar seu site:

### Opção 1: GitHub Pages (Recomendado)

1. Crie uma conta no GitHub (github.com)
2. Crie um novo repositório
3. Faça upload dos arquivos HTML
4. Vá em Settings > Pages
5. Selecione a branch main e clique em Save
6. Seu site estará em: `seu-usuario.github.io/nome-do-repositorio`

**Tutorial completo:** https://pages.github.com/

### Opção 2: Netlify

1. Vá para netlify.com
2. Crie uma conta gratuita
3. Arraste a pasta com seus arquivos HTML
4. Pronto! Seu site estará online

**Link:** https://www.netlify.com/

### Opção 3: Vercel

Mesmo processo do Netlify:
1. Vá para vercel.com
2. Faça upload dos arquivos
3. Site no ar!

**Link:** https://vercel.com/

## 🎨 Personalizar Cores

Se quiser mudar as cores do site, procure no início de qualquer arquivo HTML por:

```css
:root {
    --primary-green: #00b336;
    --accent-cyan: #00d4ff;
    --bg-dark: #0a0e0f;
}
```

Você pode mudar estes códigos de cor (são códigos hexadecimais). Use um site como https://colorpicker.me/ para escolher cores.

## ❓ Perguntas Frequentes

**P: Como adiciono imagens nos artigos?**
R: Use esta tag HTML:
```html
<img src="URL-DA-IMAGEM" alt="descrição" class="article-image">
```

**P: Como mudo o título do site?**
R: Procure por:
```html
<title>Veeam Knowledge Hub</title>
```
E substitua o texto entre as tags.

**P: Posso usar um domínio próprio?**
R: Sim! No GitHub Pages, Netlify ou Vercel você pode configurar um domínio customizado (exemplo: seunome.com). Você precisará comprar o domínio em sites como Namecheap ou GoDaddy.

## 📝 Checklist para Começar

- [ ] Editar página "Sobre" com suas informações
- [ ] Adicionar sua foto
- [ ] Atualizar links de contato (email, LinkedIn, GitHub)
- [ ] Criar seu primeiro artigo
- [ ] Adicionar o artigo na página inicial
- [ ] Fazer upload para GitHub Pages, Netlify ou Vercel
- [ ] Compartilhar com a comunidade!

## 💡 Sugestões de Conteúdo

Ideias para seus primeiros artigos:
- Como você começou com Veeam
- Erros comuns e como evitá-los
- Tutoriais passo a passo
- Comparações entre versões
- Dicas de otimização
- Estudos de caso reais
- Preparação para certificações

## 🆘 Precisa de Ajuda?

Se tiver dúvidas ou precisar de ajuda para personalizar algo específico:
1. Tente pesquisar no Google: "como fazer X em HTML"
2. Use o ChatGPT ou Claude para perguntas específicas
3. Comunidades: Stack Overflow, fóruns de Veeam

---

**Boa sorte com seu novo site de conhecimento Veeam! 🚀**
