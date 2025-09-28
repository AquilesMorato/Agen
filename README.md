<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/150x150/00509E/FFFFFF%3Ftext%3DAGEN" alt="Logo da aplicação AGEN" />
<h1>AGENDA PROGMUD (AGEN) 🗓️</h1>
<p><strong>Documento da Aplicação Web para Agendamento de Consultores da ProGmud</strong></p>
<p>
<img src="https://www.google.com/search?q=https://img.shields.io/badge/status-em%2520desenvolvimento-yellow" alt="Status do Projeto: Em Desenvolvimento">
<img src="https://www.google.com/search?q=https://img.shields.io/badge/licen%25C3%25A7a-MIT-blue" alt="Licença MIT">
</p>
</div>

🏛️ Sobre o Projeto
Instituição: CENTRO PAULA SOUZA - FACULDADE DE TECNOLOGIA DE JAHU

Curso: TECNOLOGIA EM DESENVOLVIMENTO DE SOFTWARE MULTIPLATAFORMA

Autores: Luca Morato & Aquiles Augusto

Local: Jahu, SP - 1º semestre/2025

🧭 Índice
📝 Resumo da Aplicação

🎯 Objetivos

📋 Documento de Requisitos

✅ Requisitos Funcionais (RF)

🔧 Requisitos Não Funcionais (RNF)

💡 Estudo de Viabilidade

📈 Regras de Negócio

🎨 Design

📱 Protótipo

🚀 Aplicação

🏁 Considerações Finais

📚 Referências

📝 Resumo da Aplicação Web
Um sistema criado com o objetivo de otimizar a experiência e a organização dos colaboradores da ProGmud em seus trabalhos diários.

🎯 Objetivos
Objetivo Geral
Facilitar a transferência de informações entre os consultores e techleads, com a criação automática de agendas, envio delas individualmente por e-mail e organização inteligente de horários.

Objetivos Específicos
Mapear processos atuais: Identificar como consultores, empresas e agendas são cadastrados e gerenciados hoje, destacando a necessidade de automação.

Definir funcionalidades-chave: Listar as principais operações do Sistema, como agendamento automatizado, envio de e-mail e controle das permissões para techleads e consultores.

Propor uma arquitetura técnica: Sugerir uma estrutura básica (front-end e back-end) para viabilizar a transição dos processos manuais para a plataforma web.

📋 Documento de Requisitos
O documento de requisitos de sistema detalha as funcionalidades, características e restrições que o software deve atender. Ele serve como um guia para a equipe de desenvolvimento e garante que o produto final esteja alinhado com as expectativas dos stakeholders.

✅ Requisitos Funcionais
Descrevem as funcionalidades específicas que o sistema deve ser capaz de executar.

Módulo de Cadastros e Gerenciamento (Core) 🗂️
RF01 – Cadastrar Consultores: Permitir que um administrador (Techlead) cadastre novos consultores com os campos: id_consultor (PK), nome_completo, email_profissional, email_pessoal, cargo, especialidade_tecnica e status (Ativo/Inativo).

RF02 – Cadastrar Techleads: Permitir o cadastro de Techleads, com permissões elevadas, contendo os campos: id_techlead (PK), nome_completo, email_profissional e status (Ativo/Inativo).

RF03 – Cadastrar Clientes: Permitir o cadastro dos clientes da ProGmud com os campos: id_cliente (PK), razao_social, cnpj, nome_contato_principal e email_contato.

RF04 – Gerenciar Projetos/Alocação: Permitir o cadastro e gestão dos períodos de alocação dos consultores, com os campos: id_alocacao (PK), id_consultor (FK), id_cliente (FK), data_inicio, data_fim e descricao_do_projeto.

Módulo de Agenda 📅
RF05 – Criar e Atribuir Agendas: Permitir que Techleads criem, editem e visualizem agendas, associando-as a um consultor e projeto. O sistema deve impedir conflitos de horários.

RF06 – Notificação Automática por E-mail: Enviar um e-mail de notificação para o email_profissional do consultor sempre que uma agenda for criada, alterada ou excluída.

RF07 – Visualização de Agenda Pessoal: Permitir que consultores autenticados visualizem apenas a sua própria agenda, sem permissão de edição.

Módulo de Autenticação e Perfis 🔐
RF08 – Autenticação de Usuários: Disponibilizar uma tela de login segura para autenticação via e-mail profissional e senha.

RF09 – Níveis de Permissão: Implementar pelo menos dois níveis de acesso:

Consultor: Acesso restrito à visualização da própria agenda e páginas informativas.

Techlead/Administrador: Acesso completo aos módulos de cadastro e gerenciamento de agendas.

Páginas Informativas 🌐
RF10 – Apresentação Institucional: Disponibilizar páginas estáticas (acessíveis sem login) com informações sobre a ProGmud, o sistema AGEN e uma página de créditos para os desenvolvedores.

🔧 Requisitos Não Funcionais
Definem os critérios de qualidade do sistema, garantindo uma experiência de usuário eficiente, segura e agradável.

RNF01 – Usabilidade: A interface deve ser intuitiva, limpa e de fácil utilização para minimizar a curva de aprendizado.

RNF02 – Desempenho: O tempo de resposta para carregamento de páginas e submissão de formulários não deve exceder 3 segundos em condições normais de rede.

RNF03 – Acessibilidade: Seguir as diretrizes de acessibilidade da WCAG para garantir o uso por pessoas com diferentes tipos de deficiências.

RNF04 – Compatibilidade: O sistema deve ser responsivo e funcionar corretamente nos principais navegadores (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari) em desktops e dispositivos móveis.

RNF05 – Segurança: Comunicações criptografadas com HTTPS. Senhas armazenadas com hash. Proteção contra vulnerabilidades comuns (SQL Injection, XSS).

💡 Estudo de Viabilidade
Infraestrutura: Computador pessoal e conexão à internet da faculdade.

Tecnologias: Ferramentas gratuitas (VS Code, Git, Figma) e bancos de dados gratuitos (SQLite, Firebase).

Hospedagem: GitHub Pages para o front-end.

Mão de obra: Desenvolvimento realizado por Luca Morato e Aquiles Galvão.

📈 Regras de Negócio
<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/800x450/EFEFEF/333333%3Ftext%3DFigura%2B1:%2BCanvas%2Bdo%2BModelo%2Bde%2BNeg%C3%B3cios" alt="Canvas do Modelo de Negócios" />
<p><em>Figura 1. Canvas do Modelo de Negócios. Fonte: Idealizado pela Equipe de Desenvolvimento (2025).</em></p>
</div>

🎨 Design
Paleta de Cores
A paleta em tons de azul foi escolhida para representar inovação, confiança e tecnologia.

<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/800x200/003366/FFFFFF%3Ftext%3DAzul%2BEscuro%2B%2523003366%26font%3Dopensans" alt="Paleta de Cor 1" />
<img src="https://www.google.com/search?q=https://placehold.co/800x200/00509E/FFFFFF%3Ftext%3DAzul%2BPrincipal%2B%252300509E%26font%3Dopensans" alt="Paleta de Cor 2" />
<img src="https://www.google.com/search?q=https://placehold.co/800x200/4D94DB/FFFFFF%3Ftext%3DAzul%2BClaro%2B%25234D94DB%26font%3Dopensans" alt="Paleta de Cor 3" />
<p><em>Figura 2. Paleta de Cores. Fonte: Idealizado pela Equipe de Desenvolvimento (2025).</em></p>
</div>

Tipografia
A fonte Open Sans foi selecionada por sua excelente legibilidade e versatilidade em diferentes dispositivos.

<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/800x300/EFEFEF/333333%3Ftext%3DOpen%2BSans%2B-%2BAaBbCc%26font%3Dopensans" alt="Fonte Open Sans" />
<p><em>Figura 3. Fonte Open Sans. Fonte: Google Fonts.</em></p>
</div>

Wireframe & Modelo de Navegação
🔗 Acessar Wireframe no Balsamiq

<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/800x450/EFEFEF/333333%3Ftext%3DFigura%2B5:%2BModelo%2Bde%2BNavega%C3%A7%C3%A3o" alt="Modelo de Navegação" />
<p><em>Figura 5. Modelo de Navegação. Fonte: Idealizado pela Equipe de Desenvolvimento (2025).</em></p>
</div>

📱 Protótipo
O protótipo interativo do projeto foi desenvolvido no Balsamiq e pode ser acessado no link abaixo.

🔗 Acessar Protótipo Interativo

<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/800x450/EFEFEF/333333%3Ftext%3DFigura%2B6:%2BProt%C3%B3tipo%2Bda%2BP%C3%A1gina%2BInicial" alt="Protótipo da Página Inicial" />
<p><em>Figura 6. Protótipo Da Página Inicial. Fonte: Idealizado pela Equipe de Desenvolvimento (2025).</em></p>
</div>

🚀 Aplicação
O código-fonte do projeto está hospedado no GitHub.

🔗 Acessar Repositório no GitHub

<div align="center">
<img src="https://www.google.com/search?q=https://placehold.co/800x450/EFEFEF/333333%3Ftext%3DFigura%2B7:%2BP%C3%A1gina%2BInicial%2B(Aplica%C3%A7%C3%A3o%2BReal)" alt="Screenshot da Página Inicial da Aplicação" />
<p><em>Figura 7. Página Inicial. Fonte: Idealizado pela Equipe de Desenvolvimento (2025).</em></p>
</div>

🏁 Considerações Finais
A criação do aplicativo Agen foi um exercício prático das metodologias aprendidas no curso, garantindo uma construção organizada e bem planejada. Apesar dos desafios, como o prazo limitado e a equipe pequena, a flexibilidade e a divisão de tarefas foram fundamentais para o sucesso do projeto.

📚 Referências Bibliográficas
Open Sans Font: Google Fonts

Balsamiq: balsamiq.com

GitHub: github.com

Figma: figma.com
