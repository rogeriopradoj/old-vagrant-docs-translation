Contribuindo com a tradução da documentação oficial do Vagrant:
===============================================================

Informando os documentos que deseja traduzir
--------------------------------------------

Para melhor organização, primeiro informar o(s) documento(s) que pretende ajudar na tradução e/ou revisão na planilha de tradutores/revisores:
https://docs.google.com/spreadsheet/ccc?key=0AjRfOAFDl97mdHN5ZVNyY0xOVkxXbG50Zy1IcG52UGc#gid=0

Se ainda não possuir acesso de edição nesta planilha, solicitar o acesso para rogeriopradoj at gmail dot com.

Utilizando o Git e o Github
---------------------------

1. Para começar, fazer o fork do repositório master da tradução para o português no github:

   1.1 Acessar o repositório master no github: https://github.com/rogeriopradoj/vagrant
   1.2 Clicar no botão fork

2. Agora, você irá "clonar" o projeto para a sua máquina local:
   
   2.1 Copiar a URL do repositório do seu fork, para utilizá-la com o comando git clone (por exemplo)::
    $ git clone git@github.com:seuusername/vagrant.git

   2.2 Após completar o clone do repositório, ele terá o nome remoto "origin". Não confundir, apesar do nome ser origin ele não está apontando para o repo master, mas sim para o seu fork no github.

3. Pronto, agora é só trabalhar na tradução do(s) documento(s).

4. Finalizadas as traduções e/ou revisões, faça o commit das alterações no seu repositório local::

    $ git commit –a –m "pt_BR translation"

5. Atualize o seu repositório no servidor github com as alterações realizadas localmente::

    $ git push origin master

6. O último passo é informar sobre as suas alterações ao responsável pelo repositório de origem para que ele faça um pull das alterações no repositório. Para isso, acesse a página do repositório original no github, em: https://github.com/rogeriopradoj/vagrant e envie um pull request (clicando no botão "Pull Request"):
   Mais informações sobre o [Pull Request][]


Mantendo seu repositório local atualizado
-----------------------------------------

Sempre antes de fazer as suas alterações locais, lembrar de executar o comando ``pull`` para manter atualizado o seu repositório local trazendo as alterações do repositório de origem (o repositório que você fez o fork)::

    $ git remote add upstream https://github.com/rogeriopradoj/vagrant.git
    $ git pull upstream master


Padrões a serem seguidos durante a tradução
-------------------------------------------

#### Mensagens dos Commits


As mensagens dos commits devem ser todas em INGLÊS e devem ter o seguinte prefixo:
[pt_BR][assunto][arquivo]seguido da mensagem do commit.
Ex.: Se você estiver traduzindo o arquivo ssh.md do getting-started, a mensagem do commit poderia ser semelhante a seguinte:
[pt-br][getting-started][ssh.md]Translate into Brazilian Portuguese

Dica: Escrevendo boas mensagens de commit:

[https://github.com/erlang/otp/wiki/Writing-good-commit-messages]
http://rogeriopradoj.com/2011/11/29/uma-nota-sobre-as-mensagens-do-git-commit/
http://blog.augustopascutti.com/Desenvolvimento/2012/07/17/Commit-messages.html

#### Formato da documentação

A documentação do Vagrant utiliza a linguagem Markdown juntamente com o Jekyll.

[Pull Request]: http://help.github.com/pull-requests/

Referências
-----------

- SSH issues: Guia contendo as soluções para os problemas mais comuns referentes a conexão SSH no GitHub (chave pública, ...): http://help.github.com/ssh-issues/
- Mencionar alguém em um ``pull request`` ou ``issue``: https://github.com/blog/1004-mention-autocompletion