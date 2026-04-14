# Beira Mar Pescados

Sistema web de gestão para a peixaria Beira Mar, com áreas para cliente e funcionário (dashboard, estoque, produção, vendas, fluxo de caixa, notificações e chat).

## Stack

- HTML5, CSS3, JavaScript (vanilla)
- Bootstrap 5.3, Font Awesome 6, Google Fonts (Poppins)
- Arquitetura SPA simples com troca de páginas via `navigation.js`

## Estrutura

```
├── index.html              # Entrada principal (funcionário)
├── cliente.html            # Área do cliente
├── funcionario.html        # Área do funcionário
├── script.js               # Script principal
├── styles.css              # Estilos globais
├── assets/                 # Logos e imagens de produtos
└── components/
    ├── css/                # Estilos por módulo
    ├── html/               # Parciais HTML (sidebar, header, modais…)
    └── js/                 # Módulos JS (auth, estoque, vendas, etc.)
```

## Como executar

Basta abrir `index.html` em um navegador moderno, ou servir a pasta com qualquer servidor estático:

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## Páginas principais

- **index.html / funcionario.html** — dashboard administrativo (estoque, produção, vendas, fluxo)
- **cliente.html** — área de compras do cliente (carrinho, pagamento, avaliações)

## Notas

- Referências quebradas a `fluxo.css` e `notificacoes.css` foram removidas (os estilos já estão cobertos pelos demais arquivos CSS).
