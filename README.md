# Sistema de Gerenciamento de Agendamentos – _Deia Ateliê_

## Sobre o Projeto

Este projeto tem como objetivo implantar um sistema de gerenciamento de clientes e serviços no **Deia Ateliê**, um ateliê de consertos de roupas localizado em Joinville. A iniciativa visa facilitar o agendamento de horários, melhorar a organização interna e tornar o atendimento ao cliente mais ágil, prático e eficiente.

Além de beneficiar diretamente os clientes e a gestão do ateliê, o projeto também proporciona aos estudantes envolvidos a aplicação prática dos conhecimentos em desenvolvimento de software, por meio do programa **PAC Extensionista**, que conecta soluções acadêmicas a problemas reais da comunidade.

---

## Público Beneficiado

O sistema foi desenvolvido pensando nos clientes do **Deia Ateliê**, que buscam ajustes e reparos em roupas. Este público é diversificado em idade e perfil socioeconômico e frequentemente enfrenta dificuldades na hora de agendar atendimentos e descrever os serviços necessários. Com este sistema, os clientes ganham em praticidade, enquanto o ateliê melhora sua organização e produtividade.

---

## Objetivo Geral

Implantar um sistema digital que otimize o processo de agendamento de horários e serviços no **Deia Ateliê**, garantindo um atendimento mais organizado, eficiente e satisfatório, tanto para os clientes quanto para o profissional do ateliê.

---

## Tecnologias Utilizadas

- **Frontend**:
  - **HTML**: Utilizado para estruturar a interface de usuário.
  - **CSS**: Responsável pela estilização da interface, criando um layout responsivo.
  - **JavaScript**: Usado para a criação de funcionalidades e puxar informações da API.

- **Backend**:
  - **Node.js**: Framework para o desenvolvimento da API, lógica de negócios, criação de endpoints e integração com banco de dados.

- **Banco de Dados**:
  - **PostgreSQL**: Banco de dados relacional, que vai armazenar dados dos clientes, agendamentos e serviços oferecidos pela estética automotiva, escolhido pela escalabilidade e confiabilidade.

---

## Arquitetura MVP

- A arquitetura Model-View-Presenter (MVP) foi escolhida por ser ideal para aplicações com uma interface de usuário interativa e de fluxo simples, como sistemas de agendamento e gestão

---

## Escopo

O sistema do **Deia Ateliê** tem como objetivo resolver os principais problemas enfrentados por clientes e pela administração do ateliê, trazendo mais organização, praticidade e agilidade no atendimento.

### Sistema:

- **Horários Disponíveis:** O sistema mostra os horários livres para agendamento, com base na agenda do ateliê.
- **Histórico de Agendamentos:** O sistema guarda um histórico de todos os serviços que o cliente agendou.
- **Evitar Conflitos:** O sistema bloqueia horários já agendados para não sobrecarregar a agenda.
- **Lembretes Automáticos:** O sistema manda lembretes para o cliente um dia antes do agendamento.
- **Relatórios de Serviços:** O sistema gera relatórios sobre quais serviços são mais procurados.

### Para os Clientes:

- **Login:** O usuário pode entrar no sistema usando seu e-mail e senha
- **Escolha de Serviço:** O cliente poderá agendar o tipo de serviço que deseja, escolhendo o tipo de conserto ou ajuste.
- **Descrição do Problema:** O cliente pode explicar o que precisa ser feito na peça em um campo de texto.
- **Cancelamento ou Remarcação:** O cliente pode cancelar ou remarcar um agendamento facilmente.

### Para os Administradores (Donos do Ateliê):

- **Gerenciamento pelo Administrador:** O dono do ateliê pode editar ou desativar contas de usuários.
- **Cadastro de Serviços:** O dono do ateliê pode cadastrar, editar ou remover os serviços oferecidos.
- **Definição de Horários:** O dono do ateliê pode definir os horários e dias em que os serviços podem ser agendados.
- **Visão Geral da Agenda:** O dono pode ver todos os agendamentos do dia ou da semana.
- **Mensagens Personalizadas:** O dono do ateliê pode enviar mensagens ao cliente sobre o status do serviço.
- **Histórico de Agendamentos:** O dono pode ver todos os agendamentos passados de um cliente.

---

## Qualidade e Desempenho do Sistema.

## Desempenho:

- O sistema deve carregar os horários disponíveis em até 3 segundos.
- O sistema deve ser capaz de lidar com pelo menos 20 agendamentos ao mesmo tempo sem ficar lento

## Segurança:

- O sistema precisa de uma forma de verificar a identidade do usuário quando ele acessar.
- O sistema deve bloquear tentativas de login repetidas para evitar ataques.
- O sistema deve ser protegido contra falhas de segurança, como a injeção de códigos maliciosos.

## Usabilidade:

- A interface do sistema para o dono do ateliê deve ser fácil de usar e bem desenhada.
- O sistema deve funcionar bem em celulares, tablets e computadores.

## Disponibilidade:

- O sistema deve estar disponível para uso pelo menos 99% do tempo.
- O sistema deve fazer backup automático dos dados toda madrugada para garantir a segurança da informação.

## Integração

- O sistema precisa se conectar ao WhatsApp para permitir que os cliente agendem serviços e interajam com o bot automaticamente.
- O sistema deve enviar confirmações de agendamento via WhatsApp.

  ---

## Como a arquitetura MVP atende os Requisitos Funcionais:

- Permite que Views (interfaces) sejam facilmente alteradas ou adaptadas sem afetar a lógica de negócio.
- O Presenter gerencia toda a lógica de fluxo: cadastro, agendamento, geração de relatórios, controle de agenda, envio de notificações etc.
- O Model lida com o acesso e manipulação de dados (usuários, serviços, horários), garantindo a integridade dos dados mesmo com múltiplas ações simultâneas.

  ---

## Como ela atende os Requisitos Não Funcionais:

- Desempenho: separação clara de responsabilidades evita sobrecarga na interface e torna o carregamento mais rápido.
- Segurança: lógica de segurança fica centralizada no Presenter e Model, tornando a proteção de dados mais confiável.
- Usabilidade: a View pode ser otimizada para diferentes dispositivos sem interferir no restante do sistema.
- Escalabilidade e integração com APIs (WhatsApp): facilitada por módulos independentes, podendo conectar o Presenter a serviços externos.

---

**Trello:** https://trello.com/b/Ht7yfPSk/pac-v-vi
