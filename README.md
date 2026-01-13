# IFNC Business - Landing Page

![IFNC Business Logo](./assets/img/LOGO_FINAL5.png)

> **"Seu negócio não precisa de mais marketing. Precisa de uma boa estratégia."**

Este repositório contém o código-fonte da Landing Page institucional da **IFNC Business**, uma agência focada em estratégias digitais, branding, desenvolvimento web, tráfego pago e soluções em Inteligência Artificial.

O projeto é uma página única (SPA - Single Page Application feel) responsiva, com navegação fluida, animações e seções interativas.

---

## 🚀 Funcionalidades

* **Design Responsivo:** Layout adaptável para Desktop, Tablets e Mobile utilizando Bootstrap 5 e CSS personalizado.
* **Animações de Entrada:** Elementos com efeitos de *fade-in* e *slide-up* ao rolar a página.
* **Funil de Marketing Interativo:** Visualização SVG interativa onde o usuário pode clicar nas etapas (Consciência, Conhecimento, Consideração, Decisão) para ver detalhes.
* **Portfólio Dinâmico:**
    * **Desktop:** Grid de visualização de projetos.
    * **Mobile:** Carrossel (slider) automático com suporte a gestos de "swipe" (toque).
* **Formulário de Contato Inteligente:**
    * Validação de campos em tempo real.
    * Máscara de input para telefone.
    * **Integração via Webhook:** Envio de dados assíncrono para automação (n8n/Docker).
    * Feedback visual de "Carregando", "Sucesso" ou "Erro".
* **Páginas Legais:** Termos de Uso e Política de Privacidade integrados.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura semântica.
* **CSS3:** Estilização customizada (`CONSOLIDATED-CSS.css`) com variáveis de cor e media queries.
* **JavaScript (ES6+):** Lógica de interação, máscaras e requisições HTTP (`fetch`).
* **Bootstrap 5.3.5:** Framework para grid system e componentes responsivos.
* **Google Fonts:** Tipografias *Playfair Display* e *Inter*.

---

## 📂 Estrutura de Arquivos

```text
vitor-daniel015/ifnc-landing-page/
├── assets/
│   ├── css/
│   │   └── CONSOLIDATED-CSS.css   # Estilos globais e responsivos
│   ├── img/                       # Logos de clientes e assets visuais
│   │   ├── LOGO_FINAL5.png
│   │   ├── background.png
│   │   └── ... (Portfólio e Logos)
│   └── js/
│       ├── Contato.js             # Lógica do formulário e Webhook
│       ├── Funil.js               # Lógica do SVG do Funil de Marketing
│       └── Portfolio.js           # Lógica do Carrossel Mobile
├── index.html                     # Página Principal
├── politica-de-privacidade.html   # Página de Privacidade
└── termos-de-uso.html             # Página de Termos

```

---

## ⚙️ Configuração e Instalação

### Pré-requisitos

Basta um navegador moderno para rodar o projeto visualmente. Para o funcionamento completo do formulário, é necessário um endpoint de API/Webhook.

### Como rodar

1. Clone este repositório:
```bash
git clone [https://github.com/seu-usuario/ifnc-landing-page.git](https://github.com/seu-usuario/ifnc-landing-page.git)

```


2. Abra o arquivo `index.html` no seu navegador.

### Configuração do Formulário (Webhook)

O arquivo `assets/js/Contato.js` está configurado para enviar os dados do formulário para um ambiente local Docker (n8n).

Para colocar em produção, altere a constante `urlWebhook` na **linha 94** do arquivo `Contato.js`:

```javascript
// assets/js/Contato.js

// Altere esta URL para o seu endpoint de produção
const urlWebhook = '[https://seu-endpoint-de-producao.com/webhook/](https://seu-endpoint-de-producao.com/webhook/)...'; 
// Atual: '[http://host.docker.internal:5678/webhook/sla](http://host.docker.internal:5678/webhook/sla)'

```

---

## 🎨 Paleta de Cores

O projeto utiliza um tema escuro e sofisticado, definido nas variáveis CSS:

| Cor | Hex | Uso |
| --- | --- | --- |
| **Matt Black** | `#1a1a1a` | Elementos de fundo secundários |
| **Background** | `#202122` | Fundo principal |
| **Blue** | `#002d3c` | Elementos de destaque escuros |
| **White Blue** | `#308491` | Botões e Títulos (Cor Primária) |
| **Snow White** | `#f8f8f8` | Textos principais |

---

## 📢 Portfólio Incluso

O site apresenta casos de uso reais desenvolvidos pela IFNC, incluindo:

* **Marcas:** BSN Strategy, Movimento Conscientiza Capela, Flicker, Santé HAIR.
* **Sites:** Construtora São José, Palavra Premium, Objetivo Capela, Instituto Chai.
* **Audiovisual:** Campanhas institucionais e Podcasts.

---

## 📄 Licença

Este projeto é de propriedade da **IFNC Business**. Todos os direitos reservados.

---
Desenvolvido por Vitor Daniel.
