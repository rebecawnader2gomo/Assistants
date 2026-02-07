
---

Projeto base em Zend
====================

Apresentação
------------
Estrutura MVC do framework Zend, versão 2, sem firulas: só o necessário para
começar um sistema novo sem arrastar configuração demais.

Itens que acrescentei no pacote:

- Módulo principal trazendo
    - acesso a tabela via TableGateway
    - cobertura de testes com PHPUnit
    - representação da entidade
    - camada de serviço
    - fábrica de adaptador que lê a configuração de banco declarada no módulo

- Módulo auxiliar de esqueleto

Preparando o ambiente
---------------------

Via Composer (caminho aconselhado)
----------------------------------
O jeito mais confortável de ter uma cópia rodando é puxar o código do remoto e
deixar o gerenciador baixar as bibliotecas, nesta ordem: entrar no diretório do
projeto, clonar o repositório desta aplicação e, já dentro da pasta, rodar a
instalação das dependências.

Apontamento de domínio local
----------------------------

Bloco de configuração do servidor web, usando um domínio fictício de
desenvolvimento. Aponte o DocumentRoot para a pasta pública da aplicação,
ative o modo de ambiente de desenvolvimento, informe a raiz do projeto numa
variável própria e libere o diretório público com index.php como índice,
sobrescrita de regras permitida e acesso aberto.