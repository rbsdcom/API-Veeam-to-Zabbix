# Tutorial de Configuração: Conexão do Template Veeam Backup and Replication by HTTP no Zabbix através da API do Veeam

Bem-vindo ao tutorial de configuração para conectar o Veeam Enterprise Manager no Zabbix utilizando a API do Veeam. Neste guia passo a passo, você aprenderá como configurar a integração entre o Veeam Enterprise Manager e o Zabbix, permitindo monitorar e gerenciar as suas infraestruturas de backup do Veeam por meio do Zabbix.

## Pré-requisitos

Antes de começar, verifique se você possui os seguintes requisitos:

1. Uma instância do Veeam Enterprise Manager em execução.
2. Uma instância do Zabbix configurada e em funcionamento.
3. Acesso administrativo ao servidor do Zabbix e ao servidor do Veeam Enterprise Manager.
4. Conhecimento básico do Zabbix e da API do Veeam.

## Passo 1: Obter o Veeam Backup and Replication by HTTP

1. Faça o download do Template Veeam Enterprise Manager para o Zabbix. Você pode encontrá-lo no repositório oficial do Zabbix ou em outros repositórios da comunidade. <a href="https://www.zabbix.com/br/integrations/veeam">Veja mais em, Avalable Solutions</a>
2. Extraia o conteúdo do arquivo ZIP do template para uma localização acessível no servidor do Zabbix. 



## Passo 2: Configurar o Veeam Enterprise Manager

1. Faça login no servidor do Veeam Enterprise Manager com privilégios administrativos.
2. Abra o console do Veeam Enterprise Manager.
3. Navegue até a seção "Configurações" ou "Settings" no console do Veeam Enterprise Manager.
4. Selecione "API" ou "API Configuration" nas opções disponíveis.
5. Certifique-se de que a opção "Enable RESTful API Service" ou "Ativar serviço da API RESTful" esteja marcada.
6. Anote o URL da API, o nome de usuário e a senha do Veeam Enterprise Manager, pois você precisará dessas informações para configurar o Zabbix.

## Passo 3: Importar o Veeam Backup and Replication by HTTP no Zabbix

1. Acesse o painel de administração do Zabbix.
2. Navegue até "Configuration" ou "Configuração" no menu principal.
3. Selecione "Templates" ou "Modelos".
4. Clique no botão "Import" ou "Importar" para importar um novo template.
5. Localize o arquivo XML do Veeam Backup and Replication by HTTP que você baixou anteriormente e selecione-o.
6. Clique em "Upload" ou "Enviar" para importar o template para o Zabbix.

## Passo 4: Configurar a Integração no Zabbix

1. Após a importação bem-sucedida, acesse a página do Veeam Backup and Replication by HTTP no Zabbix.
2. Clique no botão "Configuration" ou "Configuração" na barra de navegação lateral.
3. Selecione "Templates" ou "Modelos" e localize o Template Veeam Enterprise Manager.
4. Clique no nome do Templates para acessar as opções de configuração.
5. Em Macros, insira o URL da API, o nome de usuário e a senha do Veeam Enterprise Manager que você anotou anteriormente.
6. Personalize as configurações adicionais conforme necessário, como intervalos de coleta, alertas e filtros.
7. Clique em "Update" ou "Atualizar" para salvar as configurações.

## Passo 5: Verificar a Integração

1. Crie um Host e vincule o Template Veeam Backup and Replication by HTTP.
2. Aguarde alguns minutos para que o Zabbix colete os dados do Veeam Enterprise Manager.
3. Volte para o painel principal do Zabbix e navegue até as seções "Monitoring" ou "Monitoramento".
4. Explore as opções disponíveis no Template Veeam Enterprise Manager para visualizar e gerenciar as métricas e eventos do Veeam.
5. Verifique se os dados estão sendo atualizados corretamente e se os alertas estão funcionando conforme o esperado.

Pronto, você configurou com sucesso a integração entre o Template Veeam Enterprise Manager e o Zabbix usando a API do Veeam. Agora você pode monitorar e gerenciar suas infraestruturas de backup do Veeam diretamente no Zabbix.

Lembre-se de consultar a documentação oficial do Zabbix e do Veeam para obter mais informações sobre as configurações avançadas e as possíveis personalizações.