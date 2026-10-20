## Olá! Eu sou o João Vitor

**Desenvolvedor Back-end • Automações com IA & APIs**

CTO na **Uv Informática** e Partner na **BotConversa**. Transformo conversas em
automações inteligentes: uso Python para orquestrar APIs e modelos de IA, criando
soluções mais robustas e flexíveis do que as plataformas de automação convencionais.

---

### O que eu construo

Automações de atendimento em WhatsApp que rodam 24h, sem menu numerado. O cliente
escreve como falaria com uma pessoa — várias linhas, abreviação, erro de digitação —
e o fluxo entende, registra e responde.

- **Determinístico primeiro** — normalização, fuzzy match e regras resolvem a maior
  parte das mensagens sem gastar token nem esperar modelo responder.
- **IA quando compensa** — o que foge do padrão vai para modelo de linguagem, local ou
  em nuvem, escolhido conforme o custo e a latência que o caso aceita.
- **Infra própria** — a **FJ-API**, gateway de WhatsApp self-hosted em Node.js com
  Baileys (sessões, pareamento, reconexão, mídia, foto de perfil e proteção antiban).
  Desde outubro/2026 atende inclusive a produção, sem custo por mensagem.
- **Handoff para humano** — quando o bot não deve decidir, a conversa passa para o
  atendente no Chatwoot com o histórico inteiro junto.
- **Operação visível** — dashboards em tempo real para acompanhar fila, status e
  intervir na mão quando precisa.

---

### FJ-API no console da UV

Cada número de WhatsApp é uma sessão do gateway, gerenciada pelo console: conectar
por QR ou código, ver o status, apontar o webhook e derrubar a sessão.

<img src="assets/uv-console-fjapi.png" alt="Console da UV: tela da FJ-API com as sessões de WhatsApp, status, número e webhook" width="800" />

<sub>Prévia do console com dados de exemplo — os repositórios são privados.</sub>

---

### No ar

- [UV Informática](https://uvinformatica.com.br) — site da empresa
- [UV Automações](https://uvinformatica.com.br/uv_automacoes/) — agentes de IA para WhatsApp
- [Grafeno](https://grafeno.uvinformatica.com.br) — atendente virtual para pizzarias no WhatsApp

---

### Stack

<img src="assets/stack.svg" alt="n8n, Claude, Ollama, Python, Flask, PostgreSQL, MySQL, SQLite, JavaScript, Node.js, Express, Java, Regex, HTML, CSS, Docker, Nginx, Linux, Bash, Git" width="600" />

---

### Onde cada uma entra

| Ferramenta | Uso no dia a dia |
| --- | --- |
| **Python + Flask** | APIs REST, regras de negócio, webhooks e autenticação |
| **PostgreSQL** | Clientes, sessões de conversa e dados transacionais |
| **Node.js + Express** | Serviço de WhatsApp com Baileys — pareamento, sessões e reconexão |
| **FJ-API** | Gateway próprio de WhatsApp de todos os clientes, produção inclusive — gerenciado pelo console |
| **n8n** | Orquestração dos fluxos de atendimento entre WhatsApp, API e IA |
| **Claude, GLM + Ollama** | Agentes e interpretação de linguagem natural — nuvem quando o caso pede qualidade, local quando pede custo zero |
| **Chatwoot** | Painel dos atendentes humanos, com tema próprio escrito em CSS |
| **Docker** | Containers do Chatwoot na VPS — operação, logs e troubleshooting |
| **Nginx** | Proxy reverso e injeção do tema customizado via `sub_filter` |
| **Linux + Bash** | VPS Ubuntu, serviços `systemd`, deploy por SSH e rollback |
| **Regex** | Parser determinístico — normalização, sinônimos e tolerância a erro de digitação |
| **Java** | Base de orientação a objetos e estruturas de dados |
