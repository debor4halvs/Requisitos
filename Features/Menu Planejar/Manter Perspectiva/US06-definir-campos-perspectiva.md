h1. US006 Definir Campos Perspectiva

h2. +Campos do Cadastro+

|_.Nome do Campo   |_.Tipo do Campo |_.Obrigatório|_.Observação                                       |_.Tabela BD               |_.Coluna BD                   |_.Comentário                                                         |
|ID                |Auto increment  |Sim          |Não visível ao usuário.                            |sig_tb_pe_perspectiva     |id_perspectiva BIGINT         |Refere-se ao identificador único do registro da perspectiva.         |
|Plano Estratégico |Lista           |Sim          |[[RN002_-_Obrigar_Selecionar_Plano_Estratégico]]   |sig_tb_pe_plano           |ds_nome VARCHAR (255)         
                                                                                                                                  ds_sigla VARCHAR (9)          |Refere-se ao plano estratégico em que será cadastrada a perspectiva. |                                                           
|Código            |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |cd_perspectiva VARCHAR (9)    |Refere-se ao código da perspectiva.                                  |  
|Sigla             |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |sg_perspectiva VARCHAR (9)    |Refere-se a forma abreviada e conveniente de se referir a algo mais 
                                                                                                                                                                 longo. Neste contexto é a sigla da perspectiva.                      |                                           
|Ordem             |Alfanumérico    |Sim          |Somente números                                    |sig_tb_pe_perspectiva     |vl_ordem INT (9)              |Refere-se a ordem da perspectiva. Permitem aos usuários especificar 
                                                                                                                                                                 a ordem desejada para a apresentação das perspectivas.               |                                                                                                                                                                           
|Nome              |Alfanumérico    |Sim          |Somente letras e números                           |sig_tb_pe_perspectiva     |ds_nome VARCHAR (255)         |Refere-se ao nome da perspectiva.                                    
                                                                                                                                                                 No contexto de um planejamento estratégico as perspectivas são
                                                                                                                                                                 diferentes dimensões ou áreas-chave que são consideradas ao 
                                                                                                                                                                 desenvolver e implementar estratégias organizacionais. Ela ajuda a 
                                                                                                                                                                 organizar e estruturar os objetivos estratégicos em categorias que 
                                                                                                                                                                 refletem diferentes aspectos da operação ou do ambiente de uma 
                                                                                                                                                                 organização. Exemplos: Financeira, Cliente, Aprendizado etc.         |                                                                                     
|Descrição         |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |ds_perspectiva VARCHAR (3000) |Refere-se relato que busca transmitir informações detalhadas sobre a 
                                                                                                                                                                 perspectiva.                                                         |  
|Salvar            |Botão           | -           | -                                                 | -                        | -                            |Permite ao usuário do sistema gravar o registro da perspectiva.      |                                                        
|Cancelar          |Botão           | -           | -                                                 | -                        | -                            |Permite ao usuário do sistema retornar a uma tela anterior.          |                                                              
|Limpar            |Botão           | -           | -                                                 | -                        | -                            |Permite ao usuário apagar as informações inseridas.                  |                                                                        
     
----

h2. +Campos do Filtrar+


|_.Nome do Campo       |_.Tipo do Campo |_.Obrigatório|_.Observação                                       |_.Tabela BD               |_.Coluna BD                 |_.Comentário                                                         |
|Sigla da Perspectiva  |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |cd_nivel_plano VARCHAR (9)  |Refere-se a forma abreviada e conveniente de se referir a algo mais
                                                                                                                                                                   longo. Neste contexto é a sigla da perspectiva.                      | 
|Nome da Perspectiva   |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |cd_nivel_plano VARCHAR (9)  |Refere-se ao nome da perspectiva.                                    
                                                                                                                                                                   No contexto de um planejamento estratégico as perspectivas são
                                                                                                                                                                   diferentes dimensões ou áreas-chave que são consideradas ao 
                                                                                                                                                                   desenvolver e implementar estratégias organizacionais. Ela ajuda a 
                                                                                                                                                                   organizar e estruturar os objetivos estratégicos em categorias que 
                                                                                                                                                                   refletem diferentes aspectos da operação ou do ambiente de uma 
                                                                                                                                                                   organização. Exemplos: Financeira, Cliente, Aprendizado etc.         |                                                                                                                                                               
|Filtrar               |Botão           | -           | -                                                | -                         | -                          |Permite ao usuário selecionar critérios específicos para restringir 
                                                                                                                                                                   ou limitar os dados apresentados.                                    |                                                              
|Limpar                |Botão           | -           | -                                                | -                         | -                          |Permite ao usuário apagar as informações inseridas.                  | 

----

h2. +Campos do Resultado do Listar+

|_.Nome do Campo       |_.Tipo do Campo |_.Obrigatório|_.Observação                                       |_.Tabela BD               |_.Coluna BD                 |_.Comentário                                                         |
|Código                |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |cd_nivel_plano VARCHAR (9)  |Refere-se ao código da perspectiva.                                  |  
|Sigla                 |Alfanumérico    |Não          |Somente letras e números                           |sig_tb_pe_perspectiva     |sg_perspectiva VARCHAR (9)  |Refere-se a forma abreviada e conveniente de se referir a algo mais 
                                                                                                                                                                   longo. Neste contexto é a sigla da perspectiva.                      | 
|Nome                  |Alfanumérico    |Sim          |Somente letras e números                           |sig_tb_pe_perspectiva     |ds_nome VARCHAR (255)       |Refere-se ao nome da perspectiva.                                    
                                                                                                                                                                   No contexto de um planejamento estratégico as perspectivas são
                                                                                                                                                                   diferentes dimensões ou áreas-chave que são consideradas ao 
                                                                                                                                                                   desenvolver e implementar estratégias organizacionais. Ela ajuda a 
                                                                                                                                                                   organizar e estruturar os objetivos estratégicos em categorias que 
                                                                                                                                                                   refletem diferentes aspectos da operação ou do ambiente de uma 
                                                                                                                                                                   organização. Exemplos: Financeira, Cliente, Aprendizado etc.         |                                                                                                                                                               
|Visualizar            |Botão           | -           | -                                                | -                         | -                          |Permite ao usuário explorar detalhes de um item sem comprometer a 
                                                                                                                                                                   experiência geral do usuário.                                        |                                                           
|Editar                |Botão           | -           | -                                                | -                         | -                          |Permite ao usuário modificar ou ajustar informações existentes.      |
|Excluir               |Botão           | -           | -                                                | -                         | -                          |Permite ao usuário remover permanentemente um item, dado ou conteúdo 
                                                                                                                                                                   da interface.                                                        |