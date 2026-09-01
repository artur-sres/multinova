# Requisitos Funcionais

## Autenticação e Usuários

| ID    | Requisito                    | Descrição                                                                                                                                                        | Prioridade     |
| :---- | :--------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF001 | Cadastro de Usuário          | O sistema deve permitir o cadastro de usuários mediante o fornecimento de **nome, endereço de e-mail e senha**.                                                  | **Necessário** |
| RF002 | Verificação de E-mail        | O sistema deve exigir a verificação do endereço de e-mail do usuário por meio de um **código de verificação** antes de disponibilizar o acesso completo à conta. | **Necessário** |
| RF003 | Autenticação de Usuário      | O sistema deve permitir que usuários cadastrados e verificados realizem autenticação utilizando **e-mail e senha**.                                              | **Necessário** |
| RF004 | Controle de Sessão           | O sistema deve fornecer um **token de autenticação** após a autenticação bem-sucedida do usuário, permitindo o acesso aos recursos protegidos do sistema.        | **Necessário** |
| RF005 | Recuperação de Senha         | O sistema deve permitir que usuários solicitem a recuperação de senha por meio do endereço de e-mail associado à conta.                                          | **Necessário** |
| RF006 | Redefinição de Senha         | O sistema deve permitir a redefinição da senha mediante a validação do **e-mail, código de recuperação e nova senha**.                                           | **Necessário** |
| RF007 | Consulta de Dados do Usuário | O sistema deve permitir que usuários autenticados consultem os dados associados à sua conta.                                                                     | **Necessário** |
| RF008 | Edição de Dados do Usuário   | O sistema deve permitir que usuários autenticados alterem os dados editáveis associados à sua conta.                                                             | **Necessário** |

## Marcas

| ID    | Requisito          | Descrição                                                                                                                                                   | Prioridade     |
| :---- | :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF009 | Cadastro de Marcas | O sistema deve permitir que usuários autenticados cadastrem marcas para classificação dos produtos.                                                         | **Necessário** |
| RF010 | Consulta de Marcas | O sistema deve permitir que usuários autenticados consultem as marcas cadastradas em sua conta.                                                             | **Necessário** |
| RF011 | Edição de Marcas   | O sistema deve permitir que usuários autenticados alterem os dados de marcas previamente cadastradas.                                                       | **Necessário** |
| RF012 | Exclusão de Marcas | O sistema deve permitir que usuários autenticados excluam marcas cadastradas, desde que a operação não viole as regras de integridade dos dados associados. | **Necessário** |

## Categorias

| ID    | Requisito              | Descrição                                                                                                                                                       | Prioridade     |
| :---- | :--------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF013 | Cadastro de Categorias | O sistema deve permitir que usuários autenticados cadastrem categorias para classificação dos produtos.                                                         | **Necessário** |
| RF014 | Consulta de Categorias | O sistema deve permitir que usuários autenticados consultem as categorias cadastradas em sua conta.                                                             | **Necessário** |
| RF015 | Edição de Categorias   | O sistema deve permitir que usuários autenticados alterem os dados de categorias previamente cadastradas.                                                       | **Necessário** |
| RF016 | Exclusão de Categorias | O sistema deve permitir que usuários autenticados excluam categorias cadastradas, desde que a operação não viole as regras de integridade dos dados associados. | **Necessário** |

## Produtos

| ID    | Requisito                         | Descrição                                                                                                                                                                                                                                                                                      | Prioridade     |
| :---- | :-------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF017 | Cadastro de Produtos              | O sistema deve permitir que usuários autenticados cadastrem produtos informando, obrigatoriamente, o **nome do produto** e, quando aplicável, **quantidade em estoque, preço de compra e preço de venda**. O cadastro poderá conter **descrição, imagem, categoria, marca e código da marca**. | **Necessário** |
| RF018 | Consulta de Produtos              | O sistema deve permitir que usuários autenticados consultem os produtos cadastrados em sua conta.                                                                                                                                                                                              | **Necessário** |
| RF019 | Consulta de Produto               | O sistema deve permitir que usuários autenticados consultem individualmente os dados de um produto cadastrado.                                                                                                                                                                                 | **Necessário** |
| RF020 | Edição de Produtos                | O sistema deve permitir que usuários autenticados alterem os dados cadastrais de produtos existentes, incluindo **nome, descrição, imagem, categoria, marca, código da marca e quantidade em estoque**.                                                                                        | **Necessário** |
| RF021 | Controle de Estoque               | O sistema deve manter a quantidade disponível em estoque para cada produto cadastrado e impedir o registro de valores negativos de estoque.                                                                                                                                                    | **Necessário** |
| RF022 | Exclusão de Produtos              | O sistema deve permitir a exclusão de produtos sem comprometer os registros históricos que façam referência ao produto, incluindo vendas e históricos de clientes.                                                                                                                             | **Necessário** |
| RF023 | Recuperação de Produtos Excluídos | O sistema deve permitir que usuários autenticados recuperem produtos previamente excluídos.                                                                                                                                                                                                    | **Desejável**  |

## Preços

| ID    | Requisito                       | Descrição                                                                                                                                     | Prioridade     |
| :---- | :------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF024 | Registro de Preços              | O sistema deve permitir o registro do **preço de compra e preço de venda** associado a um produto.                                            | **Necessário** |
| RF025 | Histórico de Preços             | O sistema deve preservar os registros anteriores de preço de cada produto, mantendo um histórico das alterações realizadas ao longo do tempo. | **Necessário** |
| RF026 | Consulta do Histórico de Preços | O sistema deve permitir que usuários autenticados consultem o histórico de preços registrado para um produto.                                 | **Necessário** |
| RF027 | Consulta do Preço Atual         | O sistema deve permitir que usuários autenticados consultem o preço vigente de um produto.                                                    | **Necessário** |

## Clientes

| ID    | Requisito                      | Descrição                                                                                                                                                                                                                                                             | Prioridade     |
| :---- | :----------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF028 | Cadastro de Clientes           | O sistema deve permitir que usuários autenticados cadastrem clientes contendo, obrigatoriamente, **nome** e os dados financeiros necessários ao controle de débitos. O cadastro poderá incluir **endereço, telefone, data de nascimento, fotografia e preferências**. | **Necessário** |
| RF029 | Consulta de Clientes           | O sistema deve permitir que usuários autenticados consultem os clientes cadastrados em sua conta.                                                                                                                                                                     | **Necessário** |
| RF030 | Consulta Individual de Cliente | O sistema deve permitir que usuários autenticados consultem individualmente os dados cadastrais e financeiros de um cliente.                                                                                                                                          | **Necessário** |
| RF031 | Edição de Clientes             | O sistema deve permitir que usuários autenticados alterem os dados cadastrais de clientes existentes.                                                                                                                                                                 | **Necessário** |
| RF032 | Controle de Débito do Cliente  | O sistema deve manter o saldo de débito associado a cada cliente para possibilitar o acompanhamento de valores pendentes.                                                                                                                                             | **Necessário** |
| RF033 | Exclusão de Clientes           | O sistema deve permitir a exclusão de clientes sem comprometer registros históricos relacionados às vendas realizadas.                                                                                                                                                | **Necessário** |

## Vendas

| ID    | Requisito                        | Descrição                                                                                                                                                        | Prioridade     |
| :---- | :------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF034 | Registro de Venda                | O sistema deve permitir que usuários autenticados registrem uma venda associando-a a um **cliente** e a pelo menos **um produto**.                               | **Necessário** |
| RF035 | Registro de Itens da Venda       | O sistema deve registrar, para cada item de uma venda, o **produto, quantidade comercializada e preço unitário praticado no momento da venda**.                  | **Necessário** |
| RF036 | Cálculo do Valor da Venda        | O sistema deve calcular o subtotal de cada item e o valor total da venda a partir das quantidades e dos preços unitários registrados.                            | **Necessário** |
| RF037 | Preservação do Preço da Venda    | O sistema deve preservar o preço unitário praticado no momento da venda, independentemente de alterações posteriores realizadas no preço cadastrado do produto.  | **Necessário** |
| RF038 | Consulta de Vendas               | O sistema deve permitir que usuários autenticados consultem as vendas registradas, incluindo **cliente, itens, quantidades, valores, data e situação da venda**. | **Necessário** |
| RF039 | Filtragem de Vendas por Situação | O sistema deve permitir que as vendas sejam consultadas de acordo com sua situação, distinguindo ao menos vendas **concluídas** e **canceladas**.                | **Desejável**  |
| RF040 | Cancelamento de Venda            | O sistema deve permitir o cancelamento de uma venda sem remover fisicamente seu registro, preservando-a para fins de histórico.                                  | **Necessário** |

## Contas

| ID    | Requisito                        | Descrição                                                                                                                | Prioridade     |
| :---- | :------------------------------- | :----------------------------------------------------------------------------------------------------------------------- | :------------- |
| RF041 | Cadastro de Contas               | O sistema deve permitir que usuários autenticados cadastrem contas informando **descrição, valor e data de vencimento**. | **Necessário** |
| RF042 | Consulta de Contas               | O sistema deve permitir que usuários autenticados consultem as contas cadastradas em sua conta.                          | **Necessário** |
| RF043 | Consulta Individual de Conta     | O sistema deve permitir que usuários autenticados consultem individualmente os dados de uma conta cadastrada.            | **Necessário** |
| RF044 | Controle da Situação da Conta    | O sistema deve manter a situação de cada conta, distinguindo ao menos contas **pendentes** e **pagas**.                  | **Necessário** |
| RF045 | Registro de Pagamento            | O sistema deve permitir que usuários autenticados registrem uma conta pendente como paga.                                | **Necessário** |
| RF046 | Filtragem de Contas por Situação | O sistema deve permitir que as contas sejam consultadas de acordo com sua situação de pagamento.                         | **Desejável**  |
| RF047 | Exclusão de Contas               | O sistema deve permitir que usuários autenticados excluam contas cadastradas.                                            | **Necessário** |
