## US001 Incluir Perspectiva 

*Como* usuário SIG que possui permissão no módulo "Planejamento Estratégico" 
*Quero* cadastrar perspectiva
*Para* manter lista de perspectiva atualizada.

----
 
 *Cenário 1:"Apresentar Breadcrumbs"*   

*Dado* que sistema apresenta uma navegação estruturada: _Página inicial>Nome do Módulo>Menu>Nome da funcionalidade_
*Quando* usuário clica em link apresentado na estrutura
*Então* sistema retorna aos passos anteriores, conforme escolha do usuário.

----

 *Cenário 2:"Selecionar Plano Estratégico"*   

*Dado* que sistema apresenta campo plano estratégico, vide [[US006_Definir_Campos_Perspectiva]] 
*Quando* usuário seleciona um plano estratégico
*Então* sistema inclui perspectiva, somente para o plano estratégico informado.

----

 *Cenário 3:"Cadastrar Perspectiva"*   

*Dado* que usuário preenche todos o campos obrigatórios, vide [[US006_Definir_Campos_Perspectiva]] 
*Quando* usuário clica em "Salvar"
*Então* sistema guarda o registro em um banco de dados
*E* apresenta ao usuário MSG001, vide [[15_-_Mensagens]] 

----

 
 *Cenário 4:"Limpar Campos"*   

*Dado* que usuário preencheu ao menos um campo
*Quando* usuário clica em Limpar .
*Então* sistema desfaz preenchimento no formulário
*E* mantém usuário na mesma interface.

----

 *Cenário 5:"Cancelar Campos Preenchidos"*   

*Dado* que usuário preencheu ao menos um campo
*Quando* usuário clica em "Cancelar"
*Então* sistema limpa os campos 
*E* direciona usuário ao passo anterior de onde foi chamado.


----

 *Cenário 6:"Cancelar Campos Em Branco"*   

*Dado* que usuário não preencheu campo(s)
*Quando* usuário clica em "Cancelar"
*Então* sistema direciona usuário ao passo anterior de onde foi chamado.


----

 *Cenário 7:"Guardar Ação do Usuário em Histórico"*   

*Dado* que o usuário cadastrou perspectiva
*Quando* usuário conclui ação
*Então* sistema registra as informações em um banco de dados, vide regra [[RN001_-_Registrar_Histórico_(log)]] 

----

h2. Protótipos

!https://hom-redmine.cade.gov.br/attachments/download/1065/T008%20-%20Manter%20Perspectiva%20-%20Incluir.png!
 <p align="center"><img alt="VS Code in action" src="C:\Requisitos\Features\Menu Planejar\Manter Perspectiva\Protótipos\T007 - Manter Perspectiva - Listar.png"></p>