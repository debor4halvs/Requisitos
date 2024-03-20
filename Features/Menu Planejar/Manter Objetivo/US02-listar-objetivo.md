h1. US002 Listar Objetivo 

*Como* usuário SIG que possui permissão no módulo "Planejamento Estratégico" 
*Quero* listar os objetivos
*Para* visualizar todas os objetivos cadastrados.

----
 
 *Cenário 1:"Apresentar Breadcrumbs"*   

*Dado* que sistema apresenta uma navegação estruturada: _Página inicial>Nome do Módulo>Menu>Nome da funcionalidade_
*Quando* usuário clica em link apresentado na estrutura
*Então* sistema retorna aos passos anteriores, conforme escolha do usuário.

----

 *Cenário 2:"Selecionar Plano Estratégico"*   

*Dado* que sistema apresenta campo plano estratégico, vide [[US006_Definir_Campos_Objetivo_]] 
*Quando* usuário seleciona um plano estratégico
*Então* sistema inclui perspectiva, somente para o plano estratégico informado.

----

 *Cenário 3:"Filtrar por Sigla do Objetivo"*   

*Dado* que sistema apresenta filtros 
*Quando* usuário escolhe uma sigla na lista gerada, vide [[US006_Definir_Campos_Objetivo_]] 
*E* clica em filtrar
*Então* sistema recupera e exibe somente os registros para a sigla informada.

----

 *Cenário 4:"Filtrar por Nome do Objetivo"*   

*Dado* que sistema apresenta filtros
*Quando* usuário escolhe um nome na lista recuperada, vide [[US006_Definir_Campos_Objetivo_]] 
*E* clica em filtrar
*Então* sistema recupera e exibe somente os registros para o nome do objetivo informado.

----
 
 *Cenário 5:"Filtrar por Sigla da Perspectiva"*   

*Dado* que sistema apresenta filtros 
*Quando* usuário escolhe uma sigla de perspectiva
*Então* sistema recupera e exibe somente os registros para sigla da perspectiva informada.


----

 *Cenário 6:"Filtrar por Nome da Perspectiva"*   

*Dado* que sistema apresenta filtros 
*Quando* usuário escolhe um nome de perspectiva
*Então* sistema recupera e exibe somente os registros para o nome da perspectiva informada.

----

 *Cenário 7:"Limpar Filtros"*   

*Dado* que usuário preencheu ao menos um filtro exibido
*Quando* usuário clica em "Limpar"
*Então* sistema desfaz todas as seleções existentes.

----

 *Cenário 8:"Apresentar Opção Adicionar Objetivo"*   

*Dado* que sistema apresenta botão "Adicionar"
*Quando* usuário clica na opção Adicionar
*Então* sistema direciona usuário para interface [[US001_Incluir_Objetivo_]] 

----

 *Cenário 9:"Apresentar Opção Detalhar Objetivo"*   

*Dado* que usuário cadastrou ao menos um objetivo
*Quando* usuário clica na opção visualizar representada pelo ícone !https://hom-redmine.cade.gov.br/attachments/download/472/T028-icone-visualizar-list.png!
*Então* sistema direciona usuário para interface [[US005_Visualizar_Objetivo_]] 

----

 *Cenário 10:"Apresentar Opção Editar Objetivo"*   

*Dado* que usuário cadastrou ao menos um objetivo
*Quando* usuário clica na opção editar representada pelo ícone !https://hom-redmine.cade.gov.br/attachments/download/471/T029-icone-editar-list.png!
*Então* sistema direciona usuário para interface [[US003_Editar_Objetivo_]] 

----

 *Cenário 11:"Apresentar Opção Excluir Objetivo"*   

*Dado* que usuário cadastrou ao menos um objetivo
*Quando* usuário clica na opção excluir representada pelo ícone !https://hom-redmine.cade.gov.br/attachments/download/473/T030-icone-lixeira-list.png!
*Então* sistema direciona usuário para interface [[US004_Excluir_Objetivo_]] 

----


 *Cenário 12:"Listar 10 Primeiros Registros por Padrão"*   

*Dado* que sistema apresenta lista de objetivos
*Quando* usuário entra na interface
*Então* sistema apresenta por padrão os 10 primeiros registros cadastrados 
*E* pagina os demais.


----

 *Cenário 13:"Ordenar Alfabeticamente Resultado da Lista"*   

*Dado* que o usuário cadastrou dois ou mais objetivos
*Quando* a lista for apresentada
*Então* o sistema ordena a lista alfabeticamente pelo Nome do objetivo.

----

 *Cenário 14:"Resultado da Listagem"*   

*Dado* que usuário cadastrou ao menos um objetivo
*Quando* o usuário entra na lista
*Então* o sistema exibe as informações, vide [[US006_Definir_Campos_Objetivo_]] 

----

 *Cenário 15:"Apresentar Cabeçalho da Tabela por Padrão"*   

*Dado* que usuário ainda não cadastrou um objetivo
*Quando* o usuário entra no Listar
*Então* o sistema exibe as informações de cabeçalho por padrão.

----
 
h2. Protótipos


!https://hom-redmine.cade.gov.br/attachments/download/1072/T013%20-%20Manter%20Objetivo%20-%20Listar.png!



