# Ads & Analytics Lab – Web

Este projeto é um **laboratório prático de implementação de Google Analytics 4 (GA4), Google Tag Manager (GTM) e eventos de ecommerce**, criado para estudo e demonstração técnica.

O objetivo é simular um site real com eventos de negócio, validar a coleta de dados e demonstrar boas práticas de tracking.

🔗 **Site de teste:**  
https://nycollenailde.github.io/ads-analytics-site/

---

## 🎯 Objetivos do projeto

- Implementar corretamente o **Google Tag Manager**
- Configurar **Google Analytics 4** via GTM
- Enviar eventos customizados usando **dataLayer**
- Utilizar eventos recomendados de ecommerce
- Validar a implementação com **DebugView**
- Criar base para testes futuros com Google Ad Manager (GAM)

---

## 🧱 Arquitetura de tracking

Fluxo de dados implementado no projeto:

Usuário  
↓  
Site (HTML + JS)  
↓  
dataLayer.push()  
↓  
Google Tag Manager  
↓  
Google Analytics 4


📌 O site envia eventos para o `dataLayer`, que são capturados pelo GTM e encaminhados ao GA4.

---

## 🧩 Tecnologias utilizadas

- HTML5 / CSS3 / JavaScript
- Google Tag Manager (Web container)
- Google Analytics 4
- GitHub Pages (hosting)

---

## 🧪 Eventos implementados

### 1. `add_to_cart`
Evento de ecommerce recomendado pelo GA4.

**Disparo:** clique no botão *Add to Cart*  
**Parâmetros enviados:**
- `currency`
- `value`
- `items[]` (item_id, item_name, price, quantity)

---

### 2. `generate_lead`
Evento de geração de lead.

**Disparo:** clique no botão *Generate Lead*  
**Parâmetros enviados:**
- `lead_type`
- `page_location`

---

### 3. `login`
Evento de login de usuário.

**Disparo:** clique no botão *Login*  
**Parâmetros enviados:**
- `method`
- `user_id` (mock)

---

## 🔍 Validação e Debug

A implementação foi validada utilizando:

- **Preview do Google Tag Manager**
- **DebugView do GA4**

Os eventos e parâmetros podem ser observados em tempo real no DebugView.

📷 Exemplos de validação:

![DebugView add_to_cart](docs/debugview-add-to-cart.png)  
![DebugView generate_lead](docs/debugview-generate-lead.png)  
![DebugView login](docs/debugview-login.png)

---

## 📈 Próximos passos (roadmap)

- Marcar eventos como conversões no GA4
- Criar públicos baseados em comportamento
- Integrar Google Ad Manager (GAM)
- Testar eventos de impressão e clique em anúncios

---

## 👩‍💻 Autora

Projeto desenvolvido por **Nycolle Nailde**  
com foco em **Analytics, Ads e Data**.


