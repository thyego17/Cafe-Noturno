# Café Noturno

Site de uma cafeteria fictícia, criado como projeto de portfólio por **Thyego**. O visitante conhece a casa, navega pelo cardápio por categorias e vê na hora se o café está aberto ou fechado.

**Acesse:** [thyego17.github.io/Cafe-Noturno](https://thyego17.github.io/Cafe-Noturno/)

## Funcionalidades

- **Cardápio por abas:** quatro categorias (Cafés, Bebidas, Doces e Salgados), com nome, descrição e preço ligados por uma linha pontilhada, como em um cardápio impresso.
- **Status em tempo real:** uma etiqueta no topo informa se o café está aberto ou fechado agora.
- **Horários do dia:** a tabela de funcionamento destaca automaticamente o dia de hoje.
- **Contato e localização:** seção de visita com endereço e botão de mapa.

## Horário de funcionamento

| Dia | Horário |
| --- | --- |
| Segunda a sexta | 8h às 20h |
| Sábado | 9h às 22h |
| Domingo | 10h às 18h |

## Tecnologias

- HTML5 semântico
- CSS3 (Grid, Flexbox, variáveis CSS e animações)
- JavaScript puro, sem bibliotecas
- Fontes [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) e [Jost](https://fonts.google.com/specimen/Jost), via Google Fonts

## Design

- Visual elegante e aconchegante, com fundo marrom-café escuro, texto cor de creme e acento em cobre.
- Tipografia serifada em destaque, com palavras em itálico para dar ênfase.
- Layout responsivo, pensado primeiro para o celular, com abas que rolam na horizontal em telas pequenas.
- Foco visível, HTML semântico e respeito à preferência de movimento reduzido.

## Estrutura

```
Cafe-Noturno/
├── index.html
└── README.md
```

O site inteiro está em um único arquivo, com CSS e JavaScript incorporados.

## Como executar localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/thyego17/Cafe-Noturno.git
   ```
2. Abra o `index.html` no navegador.

Não é necessário instalar nada.

## Como personalizar

Tudo fica no `index.html`:

- **Cardápio:** altere o objeto `MENU` no início do script. Cada categoria é uma lista de itens no formato `["Nome", "Descrição", "Preço"]`.
- **Horários:** edite a lista `HOURS`. Cada linha é `["Dia", abre, fecha]`. Use `null` no lugar dos horários para marcar o dia como fechado. Para fechar depois da meia-noite, some 24 à hora de fechamento (1h vira `25`, 2h vira `26`). O domingo sempre vem primeiro.
- **Endereço e mapa:** troque o texto na seção "Venha nos visitar" e coloque o link do Google Maps no botão "Abrir no mapa", no lugar do `#`.
- **Textos:** o lema do topo e a seção "A casa" ficam no HTML.
- **Cores:** edite as variáveis em `:root`, no início do `<style>`.

## Observações

Este é um projeto de demonstração. Nome, endereço e preços são fictícios.

## Autor

**Thyego**

- Portfólio: [thyego17.github.io/Portif-lio](https://thyego17.github.io/Portif-lio/)
- GitHub: [@thyego17](https://github.com/thyego17)
