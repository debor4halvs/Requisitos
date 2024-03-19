h1. US003 Editar Perspectiva 

*Como* usuário SIG que possui permissão no módulo "Planejamento Estratégico" 
*Quero* editar perspectiva
*Para* manter lista de perspectiva atualizada.

----
 
 *Cenário 1:"Apresentar Breadcrumbs"*   

*Dado* que sistema apresenta uma navegação estruturada: _Página inicial>Nome do Módulo>Nome da funcionalidade_
*Quando* usuário clica em link apresentado na estrutura
*Então* sistema retorna aos passos anteriores, conforme escolha do usuário.

----

 *Cenário 2:"Editar Perspectiva"*   

*Dado* que usuário entra na interface Listar
*E* informa um plano estratégico
*E* clica na opção editar, representada pelo ícone !https://hom-redmine.cade.gov.br/attachments/download/471/T029-icone-editar-list.png!
*E* modifica uma ou mais informações
*Quando* usuário clica em "Salvar"
*Então* sistema verifica se todos os campos obrigatórios foram preenchidos, vide [[US006_Definir_Campos_Perspectiva]] 
*E* atualiza o registro da perspectiva do plano estratégico escolhido, em um banco de dados.
*E* apresenta mensagem ao usuário MSG001, vide [[15_-_Mensagens]] 

----

 *Cenário 3:"Limpar Campos"*   

*Dado* que usuário preencheu ao menos um campo
*Quando* usuário clica em "Limpar" 
*Então* sistema desfaz preenchimento no formulário
*E* mantém usuário na mesma interface.

----

 *Cenário 4:"Cancelar"*   

*Dado* que usuário preencheu nenhum, um ou mais campos
*Quando* usuário clica em "Cancelar"
*Então* sistema direciona usuário ao passo anterior de onde foi chamado.


----

 *Cenário 5:"Guardar Ação do Usuário em Histórico"*   

*Dado* que o usuário editou perspectiva
*Quando* usuário conclui ação
*Então* sistema registra as informações em um banco de dados, vide regra [[RN001_-_Registrar_Histórico_(log)]] 

----


h2. Protótipos

!https://hom-redmine.cade.gov.br/attachments/download/1069/T011%20-%20Manter%20Perspectiva%20-%20Editar.png!