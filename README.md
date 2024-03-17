# Catalogo-Digital-PHP
Catalogo Digital 

Intalação: 

Pré Instalação

1. subir todos arquivos para a pasta public_html e criar o banco de dados para o script

2.Acessar seu cpanel e em subdominio criar um subdominio *.seudominio.com, no local da pasta colocar a pasta public_html

3. Criar um subdominio conheca.seudominio.com e na pasta colocar public_html/conheca

#INSTALAÇÃO
1. Alterar URL's no arquivo
_core/includes/config.php linha 30 a 36 substituir todas URL pela a do dominio onde foi instalado

2. No mesmo arquivo de configuração alterar as linha 58 á 61 com as informações do banco de dados

3. no arquivo .htaccess dentro de public_html alterar a url seudominio.com.br 

4. No arquivo index.php na public_html na linha 197 onde esta https://conheca.veloximports.com.br colocar o seu na frente de conheca.

#CRONJOB:

Crie uma tarefa agendada de 15 em 15 minutos com o comando:

wget -q -O /dev/null "https://seudominio.com/cron.php?token=LfBMLcUA4BR3A1AAAALxKYfylrPMhMMg35IskTG4R7jYw181120&acao=sync" > /dev/null 2>&1 

Outra tarefa agendada para 1 em 1 minuto com o comando:

wget -q -O /dev/null "https://seudominio.com/cron.php?token=LfBMLcUA4BR3A1AAAALxKYfylrPMhMMg35IskTG4R7jYw181120&acao=agendamentos" > /dev/null 2>&1 

External token padrão: LfBMLcUA4BR3A1AAAALxKYfylrPMhMMg35IskTG4R7jYw181120

Você deve mudar esse token trocando as letras e numero sempre mantendo a mesma quantidade de caracteres.

#SMTP:

Crie um e-mail e configure as informaÁ„o de SMTP de envio de e-mails no arquivo CONFIG.


=============================================

login do sistema multilojas


https://seudominio.com.br/login/

admin@admin.com
Mudar1010*

demofeminino@demo.com
Mudar1010*

demomasculino@demo.com
Mudar1010*

============================================

* Antes de fazer qualquer alteração faça backup dos arquivos e bando de dados!

