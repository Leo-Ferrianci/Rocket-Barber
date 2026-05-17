# 🚀 Rocket Barber - Sistema de Agendamento e Fidelização

> **Projeto Académico:** Desenvolvimento de uma aplicação web funcional para pequenos negócios (Barbearia), unindo o poder de plataformas Low-Code (Softr + Airtable) com injeção de código customizado (HTML, CSS, JS) para regras de negócio e gamificação.

---

## 🔗 Links Importantes

- 🌐 **Live Demo (Aplicação a correr):** [Aceder ao Rocket Barber](https://tyrone97963.softr.app)
- 🎥 **Vídeo Pitch (Apresentação):** [Assistir no YouTube](https://www.youtube.com/watch?v=dSCof7pCDEc)

---

## 🎯 O Problema & A Solução

Pequenos negócios locais debatem-se frequentemente com a gestão manual de agendas (papel ou WhatsApp) e têm orçamentos limitados para contratar equipas de desenvolvimento. 

A **Rocket Barber** é um MVP (Minimum Viable Product) que resolve esta dor de forma ágil e económica. O sistema oferece:
1. Uma montra digital para o cliente agendar serviços.
2. Um sistema de fidelização automatizado que incentiva o retorno.
3. Um painel administrativo (Admin) para o controlo diário da operação.

---

## 🛠️ Tecnologias Utilizadas

- **[Softr](https://www.softr.io/):** Construção da interface do utilizador (Front-end), gestão de autenticação e rotas protegidas (Admin vs. Cliente).
- **[Airtable](https://airtable.com/):** Banco de dados relacional (Back-end) gerindo utilizadores, serviços e agendamentos.
- **HTML5 & CSS3:** Estilização avançada e responsiva (*Mobile-First*), criação de componentes não-nativos (Cartão Fidelidade).
- **JavaScript (Vanilla):** Manipulação do DOM, validação assíncrona de formulários e injeção de dados dinâmicos da sessão do utilizador.

---

## ✨ Destaques de Código Customizado (O Diferencial)

Para superar as limitações das ferramentas visuais e cumprir os requisitos técnicos do desafio, foram implementados *Custom Codes* diretamente no Front-end:

### 1. Validação de Regras de Negócio (JS)
Um *script* escuta o formulário de agendamento em tempo real. Se o utilizador selecionar um dia indisponível (ex: **Domingo**), o JavaScript bloqueia o botão de envio (`disabled`) e apresenta um alerta visual dinâmico, evitando a inserção de dados inválidos no banco de dados.

### 2. Cartão Fidelidade Interativo (Gamificação)
Em vez de uma simples tabela, foi criado um componente premium do zero com HTML/CSS (Grid e Flexbox). O JavaScript lê a variável global do Softr (`window['logged_in_user']['Cortes Concluidos']`), sincronizada com o cálculo (Count) do Airtable, e preenche os "carimbos" (🚀) na ecrã em tempo real.

---

## 🧪 Como Testar a Aplicação

Para validar todas as funcionalidades, segue este roteiro de testes:

**Como Cliente:**
1. Acede à [Aplicação](https://tyrone97963.softr.app).
2. Regista-te ou faz login.
3. Vai à página de **Serviços** e tenta agendar para um Domingo (observa o bloqueio via JS). Agenda para um dia de semana válido.
4. Vai ao teu **Perfil** e verifica o número de marcações no Cartão Fidelidade.

**Como Administrador (Gestão de Workflow):**
1. Faz login com as credenciais de *Admin*.
2. Observa o painel com os agendamentos pendentes do dia.
3. Clica no botão de ação **"Finalizar"** (One-click update) num agendamento.
4. Se voltares ao perfil do cliente, o Cartão Fidelidade terá somado automaticamente +1 foguete.

---

## 📱 Padrões Web Aplicados
- **Responsividade:** Layout adaptável garantido pelo *Grid* e *Media Queries*, assegurando uma experiência fluida em *smartphones*.
- **Acessibilidade:** Design em *Dark Mode* com alto contraste (fundo escuro e detalhes em dourado `#D4AF37`), além de fontes legíveis.
- **Ética e Privacidade:** Regras restritas de visibilidade de página (*Conditional Filters*), garantindo que os clientes apenas acedem aos seus próprios dados de perfil e histórico.

---

<div align="center">
  <p>Desenvolvido para o projeto académico de Low-Code / No-Code.</p>
</div>
