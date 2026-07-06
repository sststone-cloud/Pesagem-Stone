# Painel de Treinamentos — Pedreira Jaguary

Painel web (GitHub Pages) que lê os dados diretamente de uma planilha, com o logo da Pedreira Jaguary no topo.

## Como atualizar os dados

Existem **duas formas** de manter o painel atualizado, sem precisar mexer no código:

### Opção 1 — Substituir o arquivo `dados.csv` (mais simples)
1. Na planilha `MATRIZ_DE_TREINAMENTO_ATUALIZADA.xlsx`, abra a aba **BASE_POWERBI**.
2. Exporte/salve essa aba como CSV (Arquivo → Salvar Como → CSV UTF-8).
3. No GitHub, abra o arquivo `dados.csv` deste repositório → clique no ícone de lápis (editar) ou em "Add file → Upload files" → envie o novo CSV substituindo o antigo.
4. Faça o commit. O painel atualiza sozinho (é só recarregar a página).

### Opção 2 — Link publicado do Excel (atualiza sozinho, sem precisar subir nada no GitHub)
1. Salve a planilha no OneDrive/SharePoint (Excel Online).
2. Vá na aba BASE_POWERBI → **Arquivo → Compartilhar → Publicar na Web**.
3. Escolha essa planilha/aba e o formato **CSV** → gere o link → copie o link.
4. No painel, clique em **"⚙ Fonte de dados"** no topo, cole o link e clique em "Salvar e recarregar".
5. A partir daí, toda vez que você editar e salvar a planilha no Excel Online, o painel vai refletir os dados novos automaticamente (o link publicado sempre aponta para a versão mais recente).

> Obs.: o link fica guardado no navegador (e também pode ser compartilhado via URL, ex: `...github.io/painel/?src=SEU_LINK`). Para voltar a usar o `dados.csv` local, clique em "⚙ Fonte de dados" → "Usar dados.csv local".

## Estrutura
- `index.html` — o painel (dashboard).
- `dados.csv` — base de dados padrão (exportada da aba BASE_POWERBI).
- `logo.png` — logo da Pedreira Jaguary usado no cabeçalho.

## Publicar no GitHub Pages
1. Settings → Pages → Source: `main` branch, pasta `/ (root)`.
2. O painel ficará disponível em `https://SEU_USUARIO.github.io/NOME_DO_REPOSITORIO/`.
