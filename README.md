# NOVA — Soluções Digitais (Projeto Fictício de Portfólio)

Site institucional simples, feito em **HTML, CSS e JavaScript puro**, sem frameworks e sem build tools. Criado como projeto fictício para demonstrar habilidades de front-end em portfólio.

---

## 1. Visão geral do projeto

| Item | Descrição |
|---|---|
| Nome da empresa (fictícia) | **NOVA — Soluções Digitais** |
| Tipo de projeto | Site institucional de uma página inicial + 3 páginas internas |
| Tecnologias | HTML5, CSS3, JavaScript (vanilla) |
| Páginas | Início, Sobre, Serviços, Contato |
| Logotipo | SVG inline (sem dependência de imagem externa) |
| Responsivo | Sim (mobile, tablet, desktop) |

### Estrutura de arquivos

```
nova-site/
├── index.html        → Página inicial (com os 3 botões de navegação)
├── sobre.html        → Página "Sobre a NOVA"
├── servicos.html     → Página "Nossos Serviços"
├── contato.html       → Página "Fale Conosco" (com formulário simulado)
├── style.css          → Folha de estilos compartilhada por todas as páginas
└── README.md          → Esta documentação
```

### Os 3 botões de navegação

Na página inicial (`index.html`), os 3 cartões clicáveis levam para:

1. **Sobre a NOVA** → `sobre.html`
2. **Nossos Serviços** → `servicos.html`
3. **Fale Conosco** → `contato.html`

---

## 2. Passo a passo — Criando o projeto no VSCode

1. **Instale o VSCode**, se ainda não tiver: [https://code.visualstudio.com](https://code.visualstudio.com)

2. **Crie uma pasta para o projeto** no seu computador, por exemplo:
   ```
   Documentos/projetos/nova-site
   ```

3. **Abra a pasta no VSCode**:
   - Abra o VSCode
   - Vá em `Arquivo → Abrir Pasta...` (ou `File → Open Folder...`)
   - Selecione a pasta `nova-site`

4. **Crie os arquivos** dentro da pasta, usando o painel **Explorer** (ícone de páginas no canto superior esquerdo):
   - Clique no ícone "Novo Arquivo" e crie, um por um:
     - `index.html`
     - `sobre.html`
     - `servicos.html`
     - `contato.html`
     - `style.css`

5. **Copie o conteúdo de cada arquivo** (gerado neste projeto) para o arquivo correspondente no VSCode e salve com `Ctrl + S` (ou `Cmd + S` no Mac).

6. **Instale a extensão "Live Server"** (recomendado):
   - Vá na aba de Extensões (ícone de blocos no canto esquerdo, ou `Ctrl+Shift+X`)
   - Pesquise por **Live Server** (autor: Ritwick Dey)
   - Clique em **Install**

7. **Visualize o site no navegador**:
   - Clique com o botão direito no arquivo `index.html`
   - Selecione **"Open with Live Server"**
   - O navegador abrirá automaticamente em algo como `http://127.0.0.1:5500`
   - Qualquer alteração salva no VSCode atualiza o navegador automaticamente

---

## 3. Passo a passo — Publicando no GitHub (para portfólio)

### 3.1. Criar o repositório

1. Crie uma conta em [https://github.com](https://github.com), se ainda não tiver.
2. Clique no botão **"New"** (ou no `+` no canto superior direito → **New repository**).
3. Preencha:
   - **Repository name**: `nova-site` (ou outro nome de sua preferência)
   - **Description**: "Projeto fictício de site institucional — HTML, CSS e JS"
   - Marque como **Public** (para aparecer no portfólio)
   - Marque **"Add a README file"** (pode substituir depois pelo seu)
4. Clique em **Create repository**.

### 3.2. Enviar os arquivos (duas formas)

**Opção A — Pela interface do GitHub (mais simples):**

1. No repositório criado, clique em **"Add file" → "Upload files"**.
2. Arraste os arquivos `index.html`, `sobre.html`, `servicos.html`, `contato.html`, `style.css` e `README.md`.
3. Escreva uma mensagem de commit, por exemplo: `Primeira versão do site NOVA`.
4. Clique em **"Commit changes"**.

**Opção B — Usando Git pelo terminal (recomendado para portfólio, mostra fluência em Git):**

```bash
# 1. Entre na pasta do projeto
cd caminho/para/nova-site

# 2. Inicialize o repositório Git
git init

# 3. Adicione todos os arquivos
git add .

# 4. Crie o primeiro commit
git commit -m "Primeira versão do site NOVA"

# 5. Conecte ao repositório remoto (substitua pela URL do seu repositório)
git remote add origin https://github.com/SEU-USUARIO/nova-site.git

# 6. Renomeie a branch principal (se necessário)
git branch -M main

# 7. Envie os arquivos para o GitHub
git push -u origin main
```

### 3.3. Deixar pronto para portfólio

- No repositório, clique na engrenagem ⚙️ ao lado de **"About"** (na barra lateral direita) e adicione:
  - Uma descrição curta do projeto
  - O link do site publicado (depois do passo 4)
  - Tags/topics como: `html`, `css`, `javascript`, `frontend`, `portfolio`

---

## 4. Passo a passo — Hospedagem gratuita (GitHub Pages)

Como o repositório já está no GitHub, a forma mais simples e gratuita de publicar é o **GitHub Pages**.

1. No repositório, vá em **Settings** (Configurações).
2. No menu lateral, clique em **Pages**.
3. Em **"Build and deployment" → "Source"**, selecione **"Deploy from a branch"**.
4. Em **"Branch"**, selecione `main` e a pasta `/ (root)`.
5. Clique em **Save**.
6. Aguarde 1 a 2 minutos. O GitHub mostrará a URL pública, algo como:
   ```
   https://seu-usuario.github.io/nova-site/
   ```
7. Acesse essa URL — seu site estará no ar, gratuitamente.

> **Alternativas de hospedagem gratuita** (caso prefira outra plataforma):
> - **Netlify** ([netlify.com](https://netlify.com)) — arraste a pasta do projeto direto no painel ("Deploy manually")
> - **Vercel** ([vercel.com](https://vercel.com)) — conecta direto ao repositório do GitHub
> - **Cloudflare Pages** ([pages.cloudflare.com](https://pages.cloudflare.com)) — também conecta ao GitHub

---

## 5. Sobre a documentação deste projeto

Esta documentação (README.md) foi estruturada para servir como modelo de boas práticas de documentação de projeto front-end. Ao adaptar este projeto para outro propósito, considere manter as seguintes seções:

1. **Visão geral** — o que é o projeto, tecnologias usadas, estrutura de arquivos.
2. **Como rodar localmente** — passo a passo de instalação/visualização.
3. **Como contribuir / publicar** — fluxo de Git e deploy.
4. **Hospedagem** — onde o projeto está publicado e como replicar.
5. **Capturas de tela** (opcional, recomendado para portfólio) — adicione imagens do site na pasta `screenshots/` e referencie aqui com:
   ```markdown
   ![Página inicial](screenshots/home.png)
   ```
6. **Licença e autor** — créditos e, se quiser, uma licença (ex: MIT).

---

## 6. Créditos

Projeto fictício desenvolvido para fins de portfólio e estudo de front-end.
**Autor:** Fabiano Jesus
**Ano:** 2026
