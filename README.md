## Olá! Eu sou o João Vitor

**Desenvolvedor Back-end • Automações com IA & APIs**

CTO na **Uv Informática** e Partner na **BotConversa**. Transformo conversas em
automações inteligentes: uso Python para orquestrar APIs e modelos de IA, criando
soluções mais robustas e flexíveis do que as plataformas de automação convencionais.

---

### O que eu construo

Atendimento automatizado em WhatsApp que roda 24h, sem menu numerado. O cliente
escreve como falaria com uma pessoa — várias linhas, abreviação, erro de digitação —
e o sistema entende.

- **Determinístico primeiro (~90%)** — normalização, fuzzy match e regras resolvem a
  maior parte dos pedidos sem gastar token nem esperar modelo responder.
- **IA no fallback (~10%)** — quando a mensagem foge do padrão, aí sim entra o modelo
  de linguagem.
- **Infra própria** — serviço de WhatsApp self-hosted em Node.js com Baileys: sessões,
  QR, reconexão e reenvio, em vez de pagar por mensagem em plataforma de terceiro.
- **Operação visível** — dashboard em tempo real onde o balcão acompanha pedido,
  tempo de preparo e status da entrega.

---

### Stack

<img src="assets/stack.svg" alt="n8n, Python, Flask, PostgreSQL, MySQL, SQLite, JavaScript, Node.js, Express, Java, Regex, HTML, CSS, Docker, Nginx, Linux, Bash, Git" width="540" />

---

### Onde cada uma entra

| Ferramenta | Uso no dia a dia |
| --- | --- |
| **Python + Flask** | API de pedidos, cálculo de cardápio, webhooks e autenticação |
| **PostgreSQL** | Pedidos, clientes, cardápio e histórico de conversa |
| **Node.js + Express** | Serviço de WhatsApp com Baileys — pareamento, sessões e reconexão |
| **n8n** | Orquestração dos fluxos de atendimento entre WhatsApp, API e IA |
| **Chatwoot** | Painel dos atendentes humanos, com tema próprio escrito em CSS |
| **Docker** | Containers do Chatwoot na VPS — operação, logs e troubleshooting |
| **Nginx** | Proxy reverso e injeção do tema customizado via `sub_filter` |
| **Linux + Bash** | VPS Ubuntu, serviços `systemd`, deploy por SSH e rollback |
| **Regex** | Parser determinístico — normalização, sinônimos e tolerância a erro de digitação |
| **Java** | Base de orientação a objetos e estruturas de dados |
