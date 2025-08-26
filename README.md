# shirt-store-layout
# Layout de Loja de Camisetas (Vue + CDN)

Um layout simples e responsivo para uma página de **loja de camisetas**, construído com **HTML**, **CSS** e **Vue (via CDN)**. Focado em clareza, componentização leve e facilidade de manutenção.

> **Stack:** HTML • CSS • Vue 3 (CDN)

---

## ✨ Recursos

* Catálogo de produtos com cartão de item
* Barra de busca/filtragem (client-side)
* Estado reativo com Vue (sem build, sem bundlers)
* Layout responsivo (mobile-first)
* Estilos organizados e fáceis de customizar

---

## 📁 Estrutura de Pastas

```
root/
├─ index.html          # ponto de entrada
├─ /assets             # imagens, ícones, fontes
├─ /css
│  └─ styles.css       # estilos globais
└─ /js
   └─ app.js           # lógica Vue (CDN)
```

> *Os nomes podem variar conforme seu projeto; ajuste aqui se necessário.*

---

## 🚀 Como Rodar Localmente

Como o projeto usa Vue via **CDN**, você pode abrir direto no navegador:

1. **Clone o repositório**

   ```bash
   git clone https://github.com/<seu-usuario>/<seu-repo>.git
   cd <seu-repo>
   ```
2. **Abra o `index.html`** no navegador (duplo clique) **ou** sirva com um servidor simples:

   ```bash
   # Python 3
   python -m http.server 5173
   # ou Node.js (http-server)
   npx http-server -p 5173
   ```
3. Acesse: `http://localhost:5173`

---

## 🧠 Conceitos Vue Utilizados

* **Instância de app** com `Vue.createApp(...)`
* **Reatividade** via `data()`
* **Bindings**: `v-model`, `v-for`, `v-if`/`v-else`, `:class`, `:src`
* **Eventos**: `@click`, `@input`
* **Computed/Methods** para busca e formatações

> Por ser via CDN, não há Single File Components (SFC). A estrutura é simples e ideal para protótipo/estudo.

---

## 🧩 Seções do Layout

* **Header**: logo, navegação e campo de busca
* **Grid de Produtos**: cards com imagem, nome, preço e ação (ex.: “Adicionar”)
* **Filtro**: por termo (nome) — pode ser estendido para categorias/tamanhos
* **Footer**: links e créditos

---

## 🎨 Estilos (CSS)

* **Mobile-first** com media queries
* **Variáveis CSS** para cores, tipografia e espaçamentos
* **Grid/Flex** para layout de cards
* Classes utilitárias simples (ex.: `.container`, `.grid`, `.btn`)

> Customize `:root { --primary: ... }` em `styles.css` para trocar a paleta rapidamente.

---

## 🔧 Configuração Rápida de Dados

No `app.js`, você encontra um array `products`:

```js
const products = [
  { id: 1, name: 'Camiseta Básica', price: 59.9, size: 'M', image: 'assets/shirt-1.jpg' },
  { id: 2, name: 'Camiseta Estampada', price: 69.9, size: 'G', image: 'assets/shirt-2.jpg' },
  // ...
]
```

* Adicione/edite itens conforme necessário
* Imagens ficam em `/assets`

---

## 🧪 Teste Manual

* Buscar por termo e verificar filtragem
* Responsividade (320px → 1440px)
* Acessibilidade: foco visível, textos alternativos (`alt`), contraste

---

## 🌐 Deploy (GitHub Pages)

1. Faça push do código para a branch `main`
2. No GitHub: **Settings → Pages → Build and deployment**
3. Escolha **Branch: `main` / folder: `/root`** (ou `/docs` se publicar a partir de uma pasta)
4. Salve e aguarde a URL pública

---

## 📝 Convenções de Commit (sugestão)

Use o padrão *Conventional Commits*:

* `feat:` nova funcionalidade
* `fix:` correção de bug
* `docs:` documentação
* `style:` formatação (semântico)
* `refactor:` melhoria interna
* `perf:` performance
* `chore:` tarefas diversas

Ex.: `feat: filtro por tamanho nas camisetas`

---

## 🔭 Roadmap

* [ ] Filtro por tamanho/cor/categoria
* [ ] Ordenação por preço/popularidade
* [ ] Modal de detalhes do produto
* [ ] Carrinho simples no front
* [ ] Integração com API (futuro)

---

## 🤝 Contribuição

1. Faça um fork
2. Crie uma branch: `git checkout -b feat/minha-feature`
3. Commit: `git commit -m "feat: minha feature"`
4. Push: `git push origin feat/minha-feature`
5. Abra um Pull Request

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja `LICENSE` para mais detalhes.

---

## 👤 Autor

**Kael Requena**
*Link para o repositório:* `https://github.com/<seu-usuario>/<seu-repo>`

> Dúvidas ou sugestões? Abra uma *issue* no repositório!
