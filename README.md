VHost
=====

Gerenciador de Hosts Virtuais no Apache

O VHost é uma ferramenta que gerencia os hosts virtuais do servidor Apache na plataforma Linux. Com ele você consegue de forma simples e intuitiva visualizar seus domínios virtuais ativos,  adicionar novos domínios, editar um host já existente(criado por 
ele ou não) ou até mesmo excluir um host.
Crie ambientes de desenvolvimento para aplicações web em questão de segundos. Customize atributos de sua aplicação como IP, Port, Alias, além de poder inserir outras diretivas do Apache, mas vale lembrar que para criar um host apenas duas (2) informações são necessárias : o nome do novo domínio virtual e o local que seu projeto se encontra.
Recarregue o servidor Apache ou visite um host existente com um simples clique. Crie arquivos específicos de Logs (logs de acesso e logs de erro) para cada host existente, e assim gerencie sua aplicação de forma prática e objetiva.

Utilizando o VHost
------------------

Para que consiga utilizar o VHost, você precisa ter o Java (JRE) instalado. Sem você ainda não têm, acesso o site abaixo :
[Java](http://www.java.com/pt_BR/download/manual.jsp) - Downloads do Java para Todos os Sistemas Operacionais

Com ele (JRE) instalado, faça o seguinte :

1º – Clique no link abaixo e faça o download do VHost.

[VHost](http://bandodedados.com.br/downloads/VHost.zip) - Download do programa VHost.

2º – Após baixar o arquivo (.zip), descompacte-o e você terá em mãos o arquivo (VirtualHost.jar). Clique com o botão direito do mouse e escolha a opção abrir como, e em seguida escolha o Java para executá-lo.

A primeira tela que você verá será a seguinte :

[![Senha](http://i.imgur.com/CKZieNI.png)](http://bandodedados.com.br)

Você deverá informar sua senha de usuário do sistema (não precisa ser a senha do root).

3º – Feito isto, verá terá acesso a seguinte tela :

[![Vhost](http://i.imgur.com/z31r36B.png)](http://bandodedados.com.br)

Nela, podemos observar no seu canto esquerdo uma lista com todos os Hosts já existentes no Apache, e do outro lado na parte superior, temos alguns botões que possuem as seguintes funções :

Adicionar novo Host;
Remover um Host;
Recarregar o Apache;
Botão para ir direto ao browser, visualizar o Host que estiver selecionado;
E por fim, um botão com os créditos do programa.

Logo abaixo dos botões, dividimos as tarefas em 3 partes : Configurações Básicas (que já é o suficiente para criarmos um Virtual Host), Logs, Configurações Avançadas ( IP, Portas, Alias) e Detalhes (área para adicionar outras opções no arquivo de configuração do Virtual Host).

No primeiro campo (Domínio), insira o endereço que sua aplicação terá no servidor local, exemplo : vhost.local , e no campo abaixo, selecione o diretório aonde a mesma se encontra, exemplo : /var/www/vhost .
Estas informações já seriam suficientes para criamos o Virtual Host, mas como já mencionei acima, ainda temos a opção de :

Apontarmos um caminho tanto para os logs de acesso à sua aplicação, como para os logs de erro da mesma.
Definirmos um IP diferente do default (127.0.0.1) e uma outra porta também diferente da padrão (80), além de podermos adicionar um outro alias (apelido) para nossa aplicação.
Vale lembrar, que o VHost já cria automaticamente um alias pra gente, inserindo o “www” na frente do nosso domínio escolhido.

E mais abaixo, temos uma caixa de texto onde você poderá informar outras opções ao Apache. Para mais informações sobre estas, visite o site do Apache e veja na documentação.

[Apache](http://httpd.apache.org/docs/current/vhosts/examples.html) - Documentação Oficial do Apache.

Agora, basta clicar no botão salvar, e você receberá a informação de que seu arquivo foi criado com sucesso, porém, para ativá-lo, será necessário recarregar o Apache.

[![Save](http://i.imgur.com/4V1xLbm.png)](http://bandodedados.com.br)

Observe na imagem acima, que o terceiro botão na parte superior mudou de cor, ficando com uma parte “em vermelho” , só para nos lembrar que precisamos clicar nele para finalizarmos o processo.

Após clicarmos no botão, veremos a exibição da seguinte informação : Configurações Ativadas. Agora é só clicar no botão para visualizar no browser a sua aplicação rodando através de uma requisição feita pelo domínio que acabamos de criar.

[![Resultado](http://i.imgur.com/l1j4L32.png)](http://bandodedados.com.br)

No meu caso, criei um arquivos chamado ‘index.php’, e nele invoquei a função ‘phpinfo()’, que exibe as configurações do meu ambiente local.

E é isso aí. Espero que este programa possa te ajudar da mesma forma que me têm feito.


Sobre o VHost
-------------

Esta ferramenta também está sendo divulgada e recomendada nos seguintes sites :

[iMasters](http://imasters.com.br/box/ferramenta/vhost/) - iMasters Box - Ferramentas para Desenvolvedores

[Viva o Linux](http://vivaolinux.com.br/artigo/Criando-Virtual-Host-no-Apache-simples-assim/) - Porque nós amamos a liberdade

[Asterisk Docs](http://www.asteriskdocs.com.br/blog/administrador-de-hosts-virtuais-no-apache/) - A vontade de ensinar com o desejo de aprender!

[Bando de Dados](http://bandodedados.com.br/?p=152) - Site Oficial do Projeto VHost.
