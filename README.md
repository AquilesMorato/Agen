AGENDA PROGMUD (AGEN)
Documento da Aplicação Web para Agendamento de consultores da ProGmud
Instituição: CENTRO PAULA SOUZA - FACULDADE DE TECNOLOGIA DE JAHU

Curso: TECNOLOGIA EM DESENVOLVimento DE SOFTWARE MULTIPLATAFORMA

Autores: Luca Morato & Aquiles Augusto

Local: Jahu, SP - 1º semestre/2025

Sumário
Resumo da Aplicação

Objetivos

Documento de Requisitos

Requisitos Funcionais (RF)

Requisitos Não Funcionais (RNF)

Estudo de Viabilidade

Regras de Negócio

Design

Protótipo

Aplicação

Considerações Finais

Referências

1. Resumo da Aplicação Web
Um sistema criado com o objetivo de otimizar a experiência dos colaboradores da ProGmud em seus trabalhos.

1.1. Objetivos
Objetivo Geral
Facilitar a transferência de informações entre os consultores e techleads, com a criação automática de agendas, envio delas individualmente por e-mail e organização de horários.

Objetivos Específicos
Mapear processos atuais: Identificar como consultores, empresas e agendas são cadastrados e gerenciados hoje, destacando a necessidade de automação.

Definir funcionalidades-chave: Listar as principais operações do Sistema, como agendamento automatizado, envio de e-mail e controle das permissões para techleads e consultores.

Propor uma arquitetura técnica: Sugerir uma estrutura básica (front-end e back-end) para viabilizar a transição dos processos manuais para a plataforma web.

2. Documento de Requisitos
O documento de requisitos de sistema detalha as funcionalidades, características e restrições que o software deve atender. Ele serve como um guia para a equipe de desenvolvimento e garante que o produto final esteja alinhado com as expectativas dos stakeholders.

2.1. Requisitos Funcionais
Os Requisitos Funcionais descrevem as funcionalidades específicas que o sistema deve ser capaz de executar, representando as principais interações do usuário com a aplicação.

Módulo de Cadastros e Gerenciamento (Core)
RF01 – Cadastrar Consultores: O sistema deve permitir que um usuário administrador (ou Techlead) cadastre novos consultores. As informações a serem armazenadas devem incluir: id_consultor (chave primária, gerada automaticamente), nome_completo, email_profissional, email_pessoal, cargo, especialidade_tecnica e status (Ativo/Inativo).

RF02 – Cadastrar Techleads: O sistema deve permitir o cadastro de Techleads, que terão permissões elevadas para gerenciar agendas. As informações devem incluir: id_techlead (chave primária), nome_completo, email_profissional e status (Ativo/Inativo).

RF03 – Cadastrar Clientes: O sistema deve permitir o cadastro dos clientes da ProGmud. As informações devem incluir: id_cliente (chave primária), razao_social, cnpj, nome_contato_principal e email_contato.

RF04 – Gerenciar Projetos/Períodos de Alocação: O sistema deve permitir o cadastro e a gestão dos períodos de atuação e alocação dos consultores em clientes. As informações devem incluir: id_alocacao (chave primária), id_consultor (chave estrangeira), id_cliente (chave estrangeira), data_inicio, data_fim e descricao_do_projeto.

Módulo de Agenda
RF05 – Criar e Atribuir Agendas: O sistema deve permitir que Techleads criem, editem e visualizem as agendas dos consultores. Ao criar uma nova agenda, o Techlead deverá associá-la a um consultor, cliente/projeto e definir data, hora_inicio, hora_fim e descricao_das_tarefas. O sistema deve impedir a alocação de um mesmo consultor em horários conflitantes.

RF06 – Notificação Automática por E-mail: Após a criação, alteração ou exclusão de uma agenda, o sistema deve enviar automaticamente um e-mail de notificação para o email_profissional do consultor, contendo os detalhes da agenda ou o aviso de cancelamento.

RF07 – Visualização de Agenda Pessoal: Consultores autenticados devem poder visualizar apenas a sua própria agenda (em formato de calendário ou lista cronológica), sem permissão de edição.

Módulo de Autenticação e Perfis
RF08 – Autenticação de Usuários: O sistema deve possuir uma tela de login segura onde consultores e techleads possam se autenticar usando seu e-mail profissional e uma senha.

RF09 – Níveis de Permissão: O sistema deve ter pelo menos dois níveis de permissão:

Consultor: Acesso restrito à visualização da própria agenda e páginas informativas.

Techlead/Administrador: Acesso completo aos módulos de cadastro e gerenciamento de agendas de todos os consultores.

Páginas Informativas (Conteúdo Estático)
RF10 – Apresentação Institucional: O sistema deve conter páginas estáticas acessíveis a todos (mesmo sem login) com informações sobre a ProGmud (missão, visão, valores), sobre o sistema "Agenda ProGmud" e uma página de créditos para os desenvolvedores (nome, foto, links para LinkedIn e GitHub).

2.2. Requisitos Não Funcionais
Os Requisitos Não Funcionais definem os critérios de qualidade do sistema, garantindo que a experiência do usuário seja eficiente, segura e agradável.

RNF01 – Usabilidade: A interface do sistema deve ser intuitiva, limpa e de fácil utilização, com formulários simplificados e elementos de navegação claramente identificáveis para minimizar a curva de aprendizado.

RNF02 – Desempenho: A aplicação web deve ter tempos de resposta rápidos. O carregamento de páginas e a submissão de formulários devem ser concluídos em, no máximo, 3 segundos sob condições normais de rede.

RNF03 – Acessibilidade: A solução deve seguir as diretrizes de acessibilidade da WCAG (Web Content Accessibility Guidelines), garantindo que seja utilizável por pessoas com diferentes tipos de deficiências.

RNF04 – Compatibilidade: O sistema deve ser responsivo e funcionar corretamente nos principais navegadores (Google Chrome, Mozilla Firefox, Microsoft Edge e Safari) em suas versões mais recentes, tanto em desktops quanto em dispositivos móveis.

RNF05 – Segurança: Todas as comunicações devem ser criptografadas via HTTPS. As senhas dos usuários devem ser armazenadas de forma criptografada (hashed). O sistema deve ser protegido contra vulnerabilidades comuns, como SQL Injection e Cross-Site Scripting (XSS).

3. Estudo de Viabilidade
Como estudantes, utilizaremos recursos gratuitos ou já disponíveis:

Infraestrutura: Computador pessoal e conexão à internet da faculdade.

Tecnologias: Ferramentas gratuitas (Visual Studio Code, Git, Figma, Balsamiq) e bancos de dados gratuitos (SQLite, Firebase).

Hospedagem: GitHub.

Mão de obra: Desenvolvimento realizado por Luca Morato e Aquiles Galvão, dividindo tarefas conforme as habilidades (ex.: front-end/back-end).

4. Regras de Negócio
Figura 1. Canvas do Modelo de Negócios. Fonte: Idealizado pela Equipe de Desenvolvimento (Luca & Aquiles Galvão) utilizando Sebrae Canvas (2025).

5. Design
Paleta de Cores
As cores escolhidas seguem um esquema monocromático em tons de azul, buscando representar inovação e tecnologia.

Figura 2. Paleta de Cores. Fonte: Idealizado pela Equipe de Desenvolvimento (Luca & Aquiles Galvão) utilizando Ibis Paint X (2025).

Tipografia
A fonte selecionada foi a Open Sans, uma fonte sem serifa altamente versátil e com excelente legibilidade em diferentes telas e meios.

Figura 3. Fonte Open Sans. Fonte: Open Sans, obtida no repositório do Google Fonts.

Logo
O logo é um Isotipo que mistura a tipografia Open Sans com um símbolo formado pela sobreposição das letras que compõem o nome "AGEN".

Figura 4. Logo da aplicação AGEN. Fonte: Idealizado pela Equipe de Desenvolvimento (Luca & Aquiles Galvão) utilizando Figma (2025).

Wireframe
O wireframe, que serve como estrutura inicial da aplicação, pode ser acessado no link abaixo:
Acessar Wireframe no Balsamiq

Modelo de Navegação
Figura 5. Modelo de Navegação. Fonte: Idealizado pela Equipe de Desenvolvimento (Luca & Aquiles Galvão) utilizando Ibis Paint X (2025).

6. Protótipo
O protótipo do projeto foi criado na plataforma Figma e pode ser acessado através do link a seguir. A imagem abaixo representa a página inicial do protótipo.

Acessar Protótipo Interativo

Figura 6. Protótipo Da Página Inicial. Fonte: Idealizado pela Equipe de Desenvolvimento (Luca & Aquiles Galvão) utilizando Balsamiq (2025).

7. Aplicação
O repositório do projeto no GitHub pode ser encontrado no link abaixo:

https://github.com/AquilesMorato/P.I-FATEC

Figura 7. Página Inicial. Fonte: Idealizado pela Equipe de Desenvolvimento (Luca & Aquiles Galvão) utilizando Visual Studio Code (2025).

8. Considerações Finais
Durante a criação do aplicativo Agen, foram aplicadas várias metodologias aprendidas no curso de Desenvolvimento de Software Multiplataforma, assegurando uma construção organizada e bem planejada. O projeto encontrou obstáculos importantes, principalmente devido ao prazo limitado e à equipe pequena, demandando muita flexibilidade para superar essas dificuldades.

A divisão de tarefas foi fundamental para o andamento do projeto. Embora ambos os desenvolvedores tenham participado de todas as etapas, houve uma especialização: Luca focou mais no design, documentação, wireframe e protótipo, enquanto Aquiles concentrou-se no desenvolvimento do código.

Referências Bibliográficas
MATTESON, Steve. Open Sans. Disponível em: https://fonts.google.com/specimen/Open+Sans. Acessado em 26 de maio de 2025.

Balsamiq. Disponível em: balsamiq.com. Acessado em 21 de maio de 2025.

GitHub. Disponível em: Github.com. Acessado em 20 de maio de 2025.

WeHandle. Disponível em: https://wehandle.com.br. Acessado em 15 de maio de 2025.

TRELLO. Disponível em: Trello.com. Acessado em 20 de maio de 2025.

FIGMA. Disponível em: Figma.com. Acessado em 18 de maio de 2025.
