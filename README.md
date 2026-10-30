# Webhook
Formulário de Captação de Clientes - Setor Automóvel
Este projeto consiste num formulário web desenvolvido em HTML e CSS, desenhado para simular a estrutura de uma tabela de registo. O seu principal objetivo é facilitar a captação de clientes (leads) interessados na compra de veículos e o registo de chamados técnicos associados, enviando os dados diretamente para um fluxo de automação no n8n.

Funcionalidades
Estrutura em Tabela (CSS Grid): Layout limpo e organizado em duas colunas, onde os rótulos e os campos de preenchimento estão perfeitamente alinhados, garantindo a estética de um sistema de gestão.

Campos Específicos para Vendas: Inclui dados do consultor, informações do cliente (Lead), veículo de interesse, origem da captação e detalhes do chamado.

Integração com n8n: Configurado para enviar os dados de formulário via método HTTP (POST ou GET) diretamente para um Webhook.

Como Utilizar
Faça o download ou copie o código fonte para um ficheiro com a extensão .html (por exemplo, index.html).

Abra o ficheiro em qualquer navegador web moderno.

Preencha os dados do cliente e da negociação.

Clique em "Enviar Chamado" para transmitir as informações para o endpoint configurado.

Configuração do Webhook (n8n)
Por predefinição, o formulário está configurado para enviar os dados através do método POST, garantindo maior segurança e ocultando os parâmetros na transmissão de informações.

Caso encontre o erro 404: This webhook is not registered for POST requests, proceda da seguinte forma no seu n8n:

Abra o seu workflow.

Dê um duplo clique no nó Webhook.

Altere a configuração HTTP Method de GET para POST.

Clique em "Listen for Test Event" e faça um novo envio pelo formulário.

Se o workflow precisar de ser mantido obrigatoriamente como GET, edite o ficheiro HTML na linha referente à tag <form> e altere o atributo method="POST" para method="GET".

Tecnologias Utilizadas
HTML5: Estruturação semântica e campos de entrada de dados.

CSS3: Estilização, tipografia e layout organizado utilizando display: grid.
