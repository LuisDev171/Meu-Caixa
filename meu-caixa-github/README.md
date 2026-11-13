# Meu Caixa

Gerenciador de finanças pessoais instalável no celular (PWA): registra entradas e saídas, mostra o saldo e acompanha a meta de gastos.

Feito por **Luis Dev** · WhatsApp (12) 99249-8702 · @luisrlq171

## Recursos
- Cadastro de entradas e saídas
- Saldo atualizado na hora e meta de gastos
- Lançamentos mais recentes sempre no topo
- Dados guardados no próprio aparelho
- Instalável no Android e no iPhone, sem loja de aplicativos
- Sem dependências e sem etapa de build: HTML, CSS e JavaScript puros

## Como rodar localmente
```bash
python3 -m http.server 8000
# abra http://localhost:8000
```
O service worker só funciona em `localhost` ou `https`.

## Publicar (GitHub Pages)
1. Suba estes arquivos em um repositório
2. **Settings > Pages > Deploy from a branch > main / (root)**
3. Abra o link gerado no celular e use "Adicionar à tela inicial"

Ao alterar qualquer arquivo, troque o número da versão em `sw.js` (`VERSION`) para o celular receber a atualização.

## Estrutura
```
index.html              app completo (HTML, CSS e JS)
sw.js                   service worker (cache dos arquivos do app)
manifest.webmanifest    dados de instalação do app
icons/                  ícones do app
```
