# Davi Hensley — Catálogo de Sites & Sistemas

Site profissional e responsivo para mostrar **oito demonstrações de modelos de sites** e captar pedidos de orçamento pelo WhatsApp.

## Modelos disponíveis

1. **Concessionária de carros de luxo** — vitrine de BMW, Porsche e Mercedes-Benz, filtros por marca e categoria e consulta por modelo.
2. **Site institucional** — apresentação empresarial, serviços e contato.
3. **Loja virtual** — catálogo de moda e carrinho demonstrativo.
4. **Restaurante e delivery** — cardápio visual e seleção demonstrativa de pedidos.
5. **Portfólio profissional** — galeria visual com filtros por especialidade.
6. **Sistema de agendamento** — escolha de serviço, data e horário, com confirmação *simulada*.
7. **Landing page** — demonstração de uma página de captação de contatos e formulário que abre o WhatsApp do desenvolvedor.
8. **Painel de gestão** — indicadores ilustrativos, gráfico e pesquisa em registros fictícios.

Todos os modelos usam a identidade provisória **SUA MARCA AQUI** e mostram uma faixa indicando que se trata de demonstração. Nenhum pedido, pagamento ou agendamento é processado de verdade.

## Como publicar no GitHub Pages

1. Extraia `davi-hensley-catalogo-github.zip`.
2. Acesse [GitHub](https://github.com/) e crie um **New repository**, por exemplo `catalogo-sites` (repositório **Public**).
3. Dentro do repositório, clique em **Add file → Upload files**.
4. Envie **o conteúdo da pasta**, deixando `index.html`, `styles.css`, `app.js`, `README.md` e a pasta `assets/` **na raiz do repositório**. Não envie o `.zip` fechado.
5. Clique em **Commit changes**.
6. Acesse **Settings → Pages**. Em **Build and deployment**, selecione **Deploy from a branch**, escolha `main` e a pasta `/(root)`; depois clique em **Save**.
7. Quando a página estiver publicada, o endereço geralmente será `https://SEU-USUARIO.github.io/catalogo-sites/`.

Para usar um link direto para a concessionária, por exemplo, acrescente `#/demo/autos` ao final do endereço. Outros exemplos: `#/demo/loja`, `#/demo/restaurante`, `#/demo/agendamento`.

## Personalização

- **WhatsApp:** abra `app.js` e procure a constante `const WHATSAPP = '5584986830306';`. O número já foi configurado com código do Brasil (`55`) + DDD (`84`).
- **Nome:** troque `Davi Hensley` em `index.html` e `app.js` se desejar.
- **Título e textos do catálogo:** modifique os objetos na variável `projects`, no início do `app.js`.
- **Identidade das demonstrações:** o texto `SUA MARCA AQUI` é intencional para mostrar o lugar da identidade do futuro cliente.
- **Fotos:** utilizam URLs públicas do Unsplash. A conexão com a internet é necessária para carregar fotografias externas. Caso uma imagem não esteja disponível, o site mostra um SVG ilustrativo local.
- **Cores e estilos:** em `styles.css`.

## Estrutura

```text
catalogo-sites/
├── index.html           # Entrada do site e SEO
├── styles.css           # Estilos e responsividade
├── app.js               # Catálogo, demonstrações e interações
├── assets/
│   ├── favicon.svg
│   ├── ilustracao.svg
│   └── capa-social.png
└── README.md
```

## Observações importantes

- É um site **estático**: não precisa de `npm`, Node.js, banco de dados ou servidor para funcionar no GitHub Pages.
- Os veículos e os valores exibidos nos exemplos não são ofertas comerciais reais, nem há associação com marcas como BMW, Porsche ou Mercedes-Benz. As imagens podem mostrar veículos diferentes da denominação do card; antes de produzir um site real, devem ser substituídas por fotos oficiais/autorizadas e informações do estoque real.
- Para uma **loja funcional**, com cobrança de pagamentos, estoque e pedidos persistidos, ou para um **agendamento real**, será necessária integração com serviços de pagamento, banco de dados e/ou backend, a contratar e desenvolver separadamente.
- As fotos de terceiros são apenas ilustrativas; consulte a [Licença da Unsplash](https://unsplash.com/pt-br/licen%C3%A7a) antes de reutilizá-las em outros contextos.
- O código foi escrito em HTML, CSS e JavaScript simples para facilitar a edição e a publicação.

© Davi Hensley — Demonstrações para divulgação de serviços de desenvolvimento web.
