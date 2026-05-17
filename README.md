# 🚀 Rocket Barber - Sistema de Agendamento e Fidelização

![Capa do Projeto](https://via.placeholder.com/1200x400/111111/D4AF37?text=Rocket+Barber+-+Low-Code+%2B+Custom+JS)

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
