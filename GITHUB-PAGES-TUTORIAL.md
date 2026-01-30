# 🚀 Deploy no GitHub Pages - Passo a Passo Completo

## 📋 Requisitos
- Conta no GitHub (gratuita)
- Os arquivos: `index.html`

---

## 🎯 Método 1: Via Interface Web (MAIS FÁCIL)

### Passo 1: Criar Repositório
1. Acesse: https://github.com
2. Faça login (ou crie conta gratuita)
3. Clique no botão **"+"** no canto superior direito
4. Clique em **"New repository"**

### Passo 2: Configurar Repositório
1. **Repository name:** `matriz-impacto-valor` (ou qualquer nome)
2. **Public** (deixe marcado)
3. ✅ Marque: **"Add a README file"**
4. Clique em **"Create repository"**

### Passo 3: Upload do Arquivo
1. No repositório criado, clique em **"Add file"** → **"Upload files"**
2. Arraste o arquivo **`index.html`** para a área de upload
3. Role para baixo e clique em **"Commit changes"**

### Passo 4: Ativar GitHub Pages
1. No repositório, clique em **"Settings"** (engrenagem no topo)
2. No menu lateral esquerdo, clique em **"Pages"**
3. Em **"Source"**, selecione:
   - Branch: **main** (ou master)
   - Folder: **/ (root)**
4. Clique em **"Save"**

### Passo 5: Aguardar Deploy
1. Aguarde 1-2 minutos
2. Atualize a página
3. Você verá uma mensagem verde:
   **"Your site is live at https://seu-usuario.github.io/matriz-impacto-valor/"**

### Passo 6: Testar
1. Clique no link ou copie a URL
2. Abra em nova aba para testar
3. **Pronto!** 🎉

---

## 🎯 Método 2: Via GitHub Desktop (Interface Gráfica)

### Passo 1: Instalar GitHub Desktop
1. Baixe: https://desktop.github.com
2. Instale e faça login

### Passo 2: Criar Repositório Local
1. Clique em **"File"** → **"New Repository"**
2. Nome: `matriz-impacto-valor`
3. Local: Escolha uma pasta
4. Clique em **"Create Repository"**

### Passo 3: Adicionar Arquivo
1. Copie o arquivo `index.html` para a pasta do repositório
2. No GitHub Desktop, verá o arquivo na lista de mudanças
3. Escreva uma mensagem: "Adicionar matriz interativa"
4. Clique em **"Commit to main"**

### Passo 4: Publicar
1. Clique em **"Publish repository"**
2. ✅ Desmarque "Keep this code private"
3. Clique em **"Publish repository"**

### Passo 5: Ativar GitHub Pages
1. Acesse: https://github.com/seu-usuario/matriz-impacto-valor
2. Clique em **"Settings"** → **"Pages"**
3. Source: **main** branch, **/ (root)** folder
4. Clique em **"Save"**

---

## 🎯 Método 3: Via Git CLI (Terminal/CMD)

### Passo 1: Instalar Git
- Windows: https://git-scm.com/download/win
- Mac: `brew install git`
- Linux: `sudo apt install git`

### Passo 2: Configurar Git (primeira vez)
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

### Passo 3: Criar e Configurar Repositório
```bash
# Criar pasta
mkdir matriz-impacto-valor
cd matriz-impacto-valor

# Inicializar repositório
git init

# Copiar o index.html para esta pasta
# (use seu gerenciador de arquivos)

# Adicionar arquivo
git add index.html

# Fazer commit
git commit -m "Adicionar matriz interativa"

# Criar repositório no GitHub via CLI (se tiver gh instalado)
gh repo create matriz-impacto-valor --public --source=. --remote=origin --push
```

### Passo 4: Ou Push Manual
Se não tiver `gh` CLI, crie o repo manualmente no GitHub e:

```bash
git remote add origin https://github.com/SEU-USUARIO/matriz-impacto-valor.git
git branch -M main
git push -u origin main
```

### Passo 5: Ativar Pages via CLI
```bash
gh repo edit --enable-pages --pages-branch main
```

Ou faça manualmente via Settings → Pages (como nos métodos anteriores)

---

## 📝 Usar no Genially

Depois do deploy, use esta URL:

```html
<iframe 
  src="https://SEU-USUARIO.github.io/matriz-impacto-valor/" 
  width="100%" 
  height="800px" 
  frameborder="0"
  style="border: none;"
></iframe>
```

**Substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub!**

---

## 🔄 Como Atualizar o Site

### Via Interface Web:
1. Vá no repositório
2. Clique no arquivo `index.html`
3. Clique no ícone de lápis (editar)
4. Faça as alterações
5. Role para baixo e clique em **"Commit changes"**
6. Aguarde 1-2 minutos para atualizar

### Via GitHub Desktop:
1. Edite o `index.html` localmente
2. Abra GitHub Desktop
3. Verá as mudanças
4. Commit e Push

### Via Git CLI:
```bash
# Editar arquivo
# Depois:
git add index.html
git commit -m "Atualizar matriz"
git push
```

---

## ⚠️ Troubleshooting

### Página não aparece?
1. Aguarde 2-5 minutos
2. Verifique se o repositório é **público**
3. Verifique se Pages está ativado em Settings
4. Limpe cache do navegador (Ctrl+Shift+R)

### URL errada?
A URL será sempre:
`https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`

### Erro 404?
- Certifique-se que o arquivo se chama exatamente `index.html` (minúsculo)
- Verifique se está na raiz do repositório (não em pasta)

---

## 💡 Dicas Extras

### Domínio Personalizado
Você pode adicionar um domínio próprio de graça:
1. Settings → Pages → Custom domain
2. Adicione seu domínio (precisa ter um)

### HTTPS
GitHub Pages tem HTTPS automático! ✅

### Limite
- Repositório: 1GB
- Banda mensal: 100GB
- Sites ilimitados!

---

## 🎯 Resumo dos 3 Métodos

| Método | Dificuldade | Tempo | Melhor Para |
|--------|-------------|-------|-------------|
| Interface Web | ⭐ Fácil | 5 min | Iniciantes |
| GitHub Desktop | ⭐⭐ Médio | 7 min | Quem prefere UI |
| Git CLI | ⭐⭐⭐ Avançado | 10 min | Desenvolvedores |

**Recomendo: Interface Web (Método 1)** - Mais simples! 🚀

---

## ✅ Checklist Final

- [ ] Criar conta no GitHub
- [ ] Criar repositório público
- [ ] Upload do index.html
- [ ] Ativar GitHub Pages em Settings
- [ ] Aguardar 1-2 minutos
- [ ] Copiar URL gerada
- [ ] Testar URL no navegador
- [ ] Usar URL no Genially
- [ ] 🎉 Celebrar!

---

**Precisa de ajuda em algum passo específico? Me avise!** 😊
