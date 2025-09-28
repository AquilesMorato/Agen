# AGENDA PROGMUD (AGEN)

Sua plataforma inteligente para otimizar a gestão de agendas e a colaboração. Transforme a organização do seu dia a dia com eficiência e praticidade.

![Logo da aplicação AGEN](https://i.imgur.com/k2o2a1X.png)

## 🎯 Sobre o Projeto

[cite_start]AGEN é um sistema de agendamento criado para otimizar a experiência dos colaboradores da ProGmud[cite: 42]. [cite_start]O objetivo é facilitar a transferência de informações entre consultores e techleads, com a criação automática de agendas, envio individual por e-mail e organização de horários[cite: 47, 48].

[cite_start]Este projeto foi desenvolvido como parte do curso de Tecnologia em Desenvolvimento de Software Multiplataforma da FATEC Jahu[cite: 3].

### Principais Objetivos:
* [cite_start]**Mapear Processos Atuais:** Identificar como consultores, empresas e agendas são gerenciados para destacar a necessidade de automação[cite: 51].
* [cite_start]**Definir Funcionalidades-Chave:** Listar as operações essenciais do sistema, como agendamento automatizado e controle de permissões[cite: 53].
* [cite_start]**Propor uma Arquitetura Técnica:** Sugerir uma estrutura básica (front-end e back-end) para a transição de processos manuais para a plataforma web[cite: 55].

## ✨ Funcionalidades (Requisitos Funcionais)

### Módulo de Cadastros e Gerenciamento (Core)
* [cite_start]**RF01 - Cadastrar Consultores:** Permite que um administrador (Techlead) cadastre novos consultores no sistema[cite: 63].
* [cite_start]**RF02 - Cadastrar Techleads:** Permite o cadastro de Techleads com permissões elevadas[cite: 68].
* [cite_start]**RF03 - Cadastrar Clientes:** Permite o cadastro dos clientes da ProGmud[cite: 71].
* [cite_start]**RF04 - Gerenciar Projetos/Períodos de Alocação:** Permite o cadastro e a gestão dos períodos de atuação dos consultores em clientes[cite: 73].

### Módulo de Agenda
* [cite_start]**RF05 - Criar e Atribuir Agendas:** Techleads podem criar, editar e visualizar as agendas dos consultores [cite: 77][cite_start], com o sistema impedindo alocações em horários conflitantes[cite: 79].
* [cite_start]**RF06 - Notificação Automática por E-mail:** O sistema envia um e-mail de notificação para o consultor sempre que uma agenda é criada, alterada ou excluída[cite: 80].
* [cite_start]**RF07 - Visualização de Agenda Pessoal:** Consultores podem visualizar sua própria agenda em formato de calendário ou lista cronológica, sem permissão de edição[cite: 82, 83].

### Módulo de Autenticação e Perfis
* [cite_start]**RF08 - Autenticação de Usuários:** Tela de login segura para consultores e techleads[cite: 85].
* [cite_start]**RF09 - Níveis de Permissão:** [cite: 86]
    * [cite_start]**Consultor:** Acesso restrito à visualização da própria agenda[cite: 87].
    * [cite_start]**Techlead/Administrador:** Acesso completo aos módulos de cadastro e gerenciamento de agendas[cite: 88].

### Páginas Informativas
* [cite_start]**RF10 - Apresentação Institucional:** Páginas estáticas com informações sobre a ProGmud, o sistema e os desenvolvedores[cite: 91, 94, 95].

## 🎨 Design

O design do projeto foi pensado para ser moderno e intuitivo.

* [cite_start]**Paleta de Cores:** Utiliza um esquema de cores monocromáticas com tons de azul para representar inovação e tecnologia[cite: 181, 182].

    ![Paleta de Cores](https://i.imgur.com/xTztj9E.png)

* [cite_start]**Tipografia:** A fonte escolhida foi a **Open Sans**, por sua versatilidade e excelente legibilidade em diversas telas[cite: 208, 209].

    ![Fonte Open Sans](https://i.imgur.com/WJ8u1s1.png)

## 🛠️ Tecnologias Utilizadas

[cite_start]Para o desenvolvimento deste projeto, foram utilizadas as seguintes ferramentas gratuitas[cite: 115]:
* [cite_start]**Design e Prototipagem:** Figma, Balsamiq [cite: 117]
* [cite_start]**Desenvolvimento:** Visual Studio Code, Git [cite: 117]
* [cite_start]**Banco de Dados:** SQLite, Firebase [cite: 117]
* [cite_start]**Hospedagem:** GitHub [cite: 118]

## 🚀 Protótipo e Aplicação

[cite_start]Um protótipo navegável foi criado para demonstrar a estrutura e o fluxo da aplicação[cite: 249].

* [cite_start]**Link do Protótipo:** [https://balsamiq.cloud/sfh5gws/pqjpwco/r46FF](https://balsamiq.cloud/sfh5gws/pqjpwco/r46FF) [cite: 251]

### Página Inicial

![Protótipo da Página Inicial](https://i.imgur.com/8Qe5lM1.png)

## 🧑‍💻 Desenvolvedores

[cite_start]Este projeto foi idealizado e desenvolvido por[cite: 119]:

* [cite_start]**Luca Morato** [cite: 8]
* [cite_start]**Aquiles Augusto** [cite: 9]

[cite_start]A divisão de tarefas focou Luca na parte de design, documentação, wireframe e protótipo, enquanto Aquiles trabalhou no código de programação[cite: 295].

---
[cite_start]*Este README foi gerado com base no documento de especificação do projeto, datado do 1º semestre de 2025[cite: 11].*
