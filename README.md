﻿# Diagrama MVC

Este diagrama ilustra a arquitetura de um sistema baseado no padrão Modelo-Visão-Controlador (MVC), que é um padrão de projeto de software comumente usado para desenvolver interfaces de usuário que separa a lógica da aplicação em três componentes interconectados. 

**Usuário:**
- Interage com o sistema através de um navegador.

**Servidor:**
Divide-se em três componentes principais: View, Controller e Model.

1. **View:**
   - **List:**
     - Login: Tela para autenticação de usuário.
     - Cadastro: Tela para registro de novo usuário.
     - Dashboard: Painel principal após o login.
     - Pesquisa de manuais: Interface de busca por manuais.
     - Admins: Área de gerenciamento para administradores.
     - Cadastro de manuais: Tela para adicionar novos manuais.
     - Manuais: Visualização dos manuais disponíveis.
     - Notificações: Sistema para exibir avisos e alertas aos usuários.

2. **Controller:**
   - **Usuários:**
     - Listar, Guardar, Deletar e Procurar: Funcionalidades para manipulação de dados dos usuários.
     - Favoritar: Permitir que usuários marquem itens como favoritos.

   - **Manuais:**
     - Listar, Guardar, Deletar e Procurar: Funcionalidades para gerenciar os manuais.
     - Favoritar: Permitir que manuais sejam adicionados como favoritos.

3. **Model:**
   - **Usuários:**
     - emails: Campo para armazenar os e-mails dos usuários.
     - senhas: Campo para armazenar as senhas.
     - cadastro da DELL: Específico para o cadastro associado à DELL, possivelmente um tipo de parceria ou integração.
     - nome e idade: Armazenamento dos nomes e idades dos usuários.

   - **Manuais:**
     - qual peça: Informações sobre a peça a qual o manual se refere.
     - modelo/versão da peça: Detalhes sobre o modelo ou versão da peça.
     - vídeos ensinando: Conteúdo de mídia com instruções.
     - docs: Documentos relacionados.
     - ano de atualização: Data de quando o manual foi atualizado.
     - verificação de dados: Processo de garantir a precisão das informações dos manuais.

**Banco de Dados:**
- Utiliza PostgreSQL como sistema de gerenciamento de banco de dados.
- Recebe e armazena informações dos Modelos.

**Sails.js:**
- Indica que a aplicação utiliza o framework Sails.js, que é um framework MVC de tempo real para Node.js, e auxilia no roteamento entre o Model, Views e Controllers.

Diante disso tudo que foi mostrado a arquitetura MVC oferece uma estrutura organizacional eficaz para aplicações, segmentando-as em três componentes principais que gerenciam diferentes aspectos do processo. A "View" é responsável pela apresentação visual dos dados ao usuário. O "Controller" administra as interações do usuário, a lógica de negócios e o fluxo da aplicação. Por fim, o "Model" cuida da manipulação e armazenamento dos dados. Esse modelo permite uma clara separação de responsabilidades, facilitando a manutenção e a expansão do sistema.
