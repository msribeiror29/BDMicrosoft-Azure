# BDMicrosoft-Azure
Projeto: Processo de configuração de uma instância de Banco de Dados na plataforma Microsoft Azure
Configuração de uma instância de Banco de Dados na plataforma Microsoft Azure.

Descrição do Desafio.

Este laboratório tem como objetivo praticar o processo de configuração de uma instância de Banco de Dados na plataforma Microsoft Azure. Como entregável, o desafio proposto é a criação de um repositório contendo resumos, anotações e dicas sobre o uso da Azure, servindo como material de apoio para estudos e futuras implementações.
O que é o Banco de Dados SQL do Azure?
A Instância Gerenciada de SQL do Azure é um serviço de banco de dados em nuvem escalonável que está sempre em execução na versão estável mais recente do mecanismo de banco de dados do Microsoft SQL Server e em um sistema operacional com aplicação de patch com 99,99% de alta disponibilidade interna, oferecendo quase 100% de compatibilidade de recursos com o SQL Server. As capacidades de PaaS incorporados ao SQL do Azure gerenciado permitem que você se concentre em atividades de administração e otimização de banco de dados específicas do domínio que são críticas para seus negócios, enquanto a Microsoft lida com backups, bem como a aplicação de patches e a atualização do SQL e do código do sistema operacional, o que elimina a carga sobre o gerenciamento da infraestrutura subjacente

Pré-requisitos.

Uma assinatura do Azure. Se você não tem uma assinatura do Azure, crie uma conta gratuita
- O módulo Az.SQL mais recente para a versão atual do PowerShell ou a versão mais recente da CLI do Azure.

Para obter as especificações, confira Regiões compatíveis e Tipos de assinatura compatíveis.

1 Criar uma Instância Gerenciada de SQL do Azure.

Criaremos uma implantação de Instância Gerenciada de SQL do Azure usando o portal do Azure usando o passo a passo da documentação do Microsoft Azure.

Para sua instância, siga estas etapas:

1.1 - Entre no portal do Azure.

1.2 - No menu esquerdo do portal do Azure, selecione SQL do Azure. Se SQL do Azure não estiver na lista, selecione Todos os serviços e, em seguida, digite SQL do Azure na caixa de pesquisa.

1.3 - Selecione + Criar para abrir a página Selecionar opção de implantação do SQL. Veja mais informações sobre a Instância Gerenciada de SQL do Azure selecionando Mostrar detalhes no bloco Instâncias gerenciadas de SQL.

1.4 - Escolha Instância única na lista suspensa e depois selecione Criar para abrir a página Criar instância gerenciada de SQL do Azure.
![Capture primeira](https://github.com/user-attachments/assets/855a3e2e-31ef-4aa8-89c4-1c2ab1eaf18d)

2 Guia Básico.

2.1 Preencha as informações obrigatórias solicitadas no guia Básico, que é o requisito mínimo para provisionar uma Instância Gerenciada de SQL.

A tabela a seguir fornece detalhes para as informações necessárias no guia Básico:
![Capture 0](https://github.com/user-attachments/assets/02805a78-52f0-4c7e-a4af-aa532c0b7c80)

2.2 Em Detalhes da instância gerenciada, selecione Configurar instância gerenciada na seção Computação + armazenamento para abrir a página Computação + armazenamento.

2.3 A tabela a seguir fornece recomendações para a computação e o armazenamento para sua instância gerenciada SQL de exemplo:
![Capture 5](https://github.com/user-attachments/assets/d33e8d4d-d15a-46bc-888c-e4108a75fd10)

2.4 Podemos ver que aqui foi criado o nome do banco de dados.
![Capture 34](https://github.com/user-attachments/assets/44cfa413-e786-4691-ac63-1b81d9bc764f)

2.5 Vejamos a criação do Servidor e sua localização
![Capture 2](https://github.com/user-attachments/assets/62fd15da-c82a-4987-84f6-24fc8977811f)

2.6 Para concluir é necessário selecionar o usuário.
![Capture 3](https://github.com/user-attachments/assets/61762aad-0dae-4032-8f08-ac6bf51298c4)

2.7 Depois de projetar sua Configuração de Computação + Armazenamento, use Aplicar para salvar suas configurações e navegar de volta para a página Criar Instância Gerenciada SQL do Azure.

3 Examinar + criar

3.1 Selecione o guia Examinar + criar, examine suas escolhas e selecione Criar para implantar sua instância gerenciada.
![Capture 4](https://github.com/user-attachments/assets/290a9ae1-d0a5-48ea-8baf-992ce890d115)

4 Monitorar o progresso da implantação.

4.1 Selecione o ícone Notificações para exibir o status da implantação.

![Capture antes do 6](https://github.com/user-attachments/assets/3fd7939e-c0a9-4577-b832-799729d48854)

4.2 Selecione Implantação em andamento na notificação para abrir a janela da Instância Gerenciada de SQL e monitorar mais detalhadamente o progresso da implantação.

Após a conclusão da implantação, navegue até o grupo de recursos para gerenciar a instância gerenciada:
![Capture 6](https://github.com/user-attachments/assets/e560cfb4-d914-4917-92f8-6915ad5544e2)

5 Revisar configurações de rede.

5.1 Selecione o recurso Tabela de rotas em seu grupo de recursos para examinar o objeto padrão de tabela de rotas definido pelo usuário e as entradas para rotear o tráfego de e dentro da rede virtual da Instância Gerenciada de SQL. Para alterar ou adicionar rotas, abra Rotas nas configurações da tabela de rotas.

5.2 Selecione o objeto do Grupo de segurança de rede para examinar as regras de segurança de entrada e saída. Para alterar ou adicionar regras, abra Regras de Segurança de Entrada e Regras de Segurança de Saída nas configurações do grupo de segurança de rede.

Fim.













