h1. US004 Excluir Perspectiva

*Como* usuário SIG que possui permissão no módulo "Planejamento Estratégico" 
*Quero* excluir perspectiva
*Para* manter lista de perspectiva atualizada.

----
 
 *Cenário 1:"Apresentar Breadcrumbs"*   

*Dado* que sistema apresenta uma navegação estruturada: _Página inicial>Nome do Módulo>Nome da funcionalidade_
*Quando* usuário clica em link apresentado na estrutura
*Então* sistema retorna aos passos anteriores, conforme escolha do usuário.


----

 *Cenário 2:"Excluir Perspectiva Botão Excluir"*   

*Dado* que usuário entra no Listar Perspectiva
*E* informa um plano estratégico
*E* clica na opção excluir, representado pelo ícone !https://hom-redmine.cade.gov.br/attachments/download/473/T030-icone-lixeira-list.png!
*E* que sistema apresenta mensagem MSG002, vide [[15_-_Mensagens]] 
*Quando* usuário clica no botão excluir 
*Então* sistema apaga o registro na base de dados
*E* sistema apresenta ao usuário mensagem MSG001, vide [[15_-_Mensagens]] 


----

 *Cenário 3:"Excluir Plano Botão Cancelar"*   

*Dado* que usuário entra no Listar Perspectiva
*E* informa um plano estratégico
*E* clica na opção excluir, representado pelo ícone !https://hom-redmine.cade.gov.br/attachments/download/473/T030-icone-lixeira-list.png!
*E* que o sistema apresenta mensagem MSG002, vide [[15_-_Mensagens]] 
*Quando* usuário clica no botão cancelar
*Então* sistema fecha caixa de mensagem 
*E* retorna ao passo anterior.

----


 *Cenário 4:"Guardar Ação do Usuário em Histórico"*   

*Dado* que o usuário excluiu perspectiva
*Quando* usuário conclui ação
*Então* sistema registra as informações em um banco de dados, vide regra [[RN001_-_Registrar_Histórico_(log)]] 

----


h2. Protótipos

!https://hom-redmine.cade.gov.br/attachments/download/658/T007%20-%20Manter%20Perspectiva%20-%20Excluir.png!

----

!https://hom-redmine.cade.gov.br/attachments/download/659/T008%20-%20Manter%20Perspectiva%20-%20Excluir%20-%20MSG.png!
