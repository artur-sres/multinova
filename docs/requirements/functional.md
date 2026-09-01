# Requisitos Funcionais

## Autenticação e Usuários

| ID    | Requisito                    | Descrição                                                                                                                                                        | Prioridade     | Status | Observações |
| :---- | :--------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :------------- | :-- |
| RF001 | Cadastro de Usuário          | O sistema deve permitir o cadastro de usuários mediante o fornecimento de **nome, endereço de e-mail e senha**.                                                  | **Necessário** |✅Concluído| 
| RF002 | Verificação de E-mail        | O sistema deve exigir a verificação do endereço de e-mail do usuário por meio de um **código de verificação** antes de disponibilizar o acesso completo à conta. | **Necessário** | ✅Concluído |
| RF003 | Autenticação de Usuário      | O sistema deve permitir que usuários cadastrados e verificados realizem autenticação utilizando **e-mail e senha**.                                              | **Necessário** | ✅Concluído |
| RF004 | Controle de Sessão           | O sistema deve fornecer um **token de autenticação** após a autenticação bem-sucedida do usuário, permitindo o acesso aos recursos protegidos do sistema.        | **Necessário** | ✅Concluído |
| RF005 | Recuperação de Senha         | O sistema deve permitir que usuários solicitem a recuperação de senha por meio do endereço de e-mail associado à conta.                                          | **Necessário** | ✅Concluído |
| RF006 | Redefinição de Senha         | O sistema deve permitir a redefinição da senha mediante a validação do **e-mail, código de recuperação e nova senha**.                                           | **Necessário** | ✅Concluído |
| RF007 | Consulta de Dados do Usuário | O sistema deve permitir que usuários autenticados consultem os dados associados à sua conta.                                                                     | **Necessário** | ⏳Pendente |
| RF008 | Edição de Dados do Usuário   | O sistema deve permitir que usuários autenticados alterem os dados editáveis associados à sua conta.                                                             | **Necessário** | ⏳Pendente |

## Marcas

| ID    | Requisito          | Descrição                                                                                                                                                   | Prioridade     | Status | Observações |
| :---- | :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :-- | :-- |
| RF009 | Cadastro de Marcas | O sistema deve permitir que usuários autenticados cadastrem marcas para classificação dos produtos.                                                         | **Necessário** | ✅Concluído |
| RF010 | Consulta de Marcas | O sistema deve permitir que usuários autenticados consultem as marcas cadastradas em sua conta.                                                             | **Necessário** | ✅Concluído |
| RF011 | Edição de Marcas   | O sistema deve permitir que usuários autenticados alterem os dados de marcas previamente cadastradas.                                                       | **Necessário** | ✅Concluído |
| RF012 | Exclusão de Marcas | O sistema deve permitir que usuários autenticados excluam marcas cadastradas, desde que a operação não viole as regras de integridade dos dados associados. | **Necessário** | ✅Concluído |

## Categorias

| ID    | Requisito              | Descrição                                                                                                                                                       | Prioridade     | Status | Observações |
| :---- | :--------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :--| :-- |
| RF013 | Cadastro de Categorias | O sistema deve permitir que usuários autenticados cadastrem categorias para classificação dos produtos.                                                         | **Necessário** | ✅Concluído |
| RF014 | Consulta de Categorias | O sistema deve permitir que usuários autenticados consultem as categorias cadastradas em sua conta.                                                             | **Necessário** | ✅Concluído |
| RF015 | Edição de Categorias   | O sistema deve permitir que usuários autenticados alterem os dados de categorias previamente cadastradas.                                                       | **Necessário** | ✅Concluído |
| RF016 | Exclusão de Categorias | O sistema deve permitir que usuários autenticados excluam categorias cadastradas, desde que a operação não viole as regras de integridade dos dados associados. | **Necessário** | ✅Concluído |

## Produtos

| ID    | Requisito                         | Descrição                                                                                                                                                                                                                                                                                      | Prioridade     | Status| Observações |
| :---- | :-------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :-- | :-- |
| RF017 | Cadastro de Produtos              | O sistema deve permitir que usuários autenticados cadastrem produtos informando, obrigatoriamente, o **nome do produto** e, quando aplicável, **quantidade em estoque, preço de compra e preço de venda**. O cadastro poderá conter **descrição, imagem, categoria, marca e código da marca**. | **Necessário** | ⏳Pendente | Faltando somente o upload das imagens
| RF018 | Consulta de Produtos              | O sistema deve permitir que usuários autenticados consultem os produtos cadastrados em sua conta.                                                                                                                                                                                              | **Necessário** | ✅Concluído |
| RF019 | Consulta de Produto               | O sistema deve permitir que usuários autenticados consultem individualmente os dados de um produto cadastrado.                                                                                                                                                                                 | **Necessário** | ✅Concluído |
| RF020 | Edição de Produtos                | O sistema deve permitir que usuários autenticados alterem os dados cadastrais de produtos existentes, incluindo **nome, descrição, imagem, categoria, marca, código da marca e quantidade em estoque**.                                                                                        | **Necessário** | ⏳Pendente |  
| RF021 | Controle de Estoque               | O sistema deve manter a quantidade disponível em estoque para cada produto cadastrado e impedir o registro de valores negativos de estoque.                                                                                                                                                    | **Necessário** | ✅Concluído |
| RF022 | Exclusão de Produtos              | O sistema deve permitir a exclusão de produtos sem comprometer os registros históricos que façam referência ao produto, incluindo vendas e históricos de clientes.                                                                                                                             | **Necessário** | ✅Concluído |
| RF023 | Recuperação de Produtos Excluídos | O sistema deve permitir que usuários autenticados recuperem produtos previamente excluídos.                                                                                                                                                                                                    | **Desejável**  | ⏳Pendente |

## Preços

| ID    | Requisito                       | Descrição                                                                                                                                     | Prioridade     | Status | Observações |
| :---- | :------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :-- | :-- |
| RF024 | Registro de Preços              | O sistema deve permitir o registro do **preço de compra e preço de venda** associado a um produto.                                            | **Necessário** | ✅Concluído |
| RF025 | Histórico de Preços             | O sistema deve preservar os registros anteriores de preço de cada produto, mantendo um histórico das alterações realizadas ao longo do tempo. | **Necessário** | ✅Concluído |
| RF026 | Consulta do Histórico de Preços | O sistema deve permitir que usuários autenticados consultem o histórico de preços registrado para um produto.                                 | **Necessário** | ✅Concluído |
| RF027 | Consulta do Preço Atual         | O sistema deve permitir que usuários autenticados consultem o preço vigente de um produto.                                                    | **Necessário** | ✅Concluído |

## Clientes

| ID    | Requisito                      | Descrição                                                                                                                                                                                                                                                             | Prioridade     | Status | Observações |
| :---- | :----------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :-- | :-- |
| RF028 | Cadastro de Clientes           | O sistema deve permitir que usuários autenticados cadastrem clientes contendo, obrigatoriamente, **nome** e os dados financeiros necessários ao controle de débitos. O cadastro poderá incluir **endereço, telefone, data de nascimento, fotografia e preferências**. | **Necessário** | ⏳Pendente | Faltando somente upload das fotos
| RF029 | Consulta de Clientes           | O sistema deve permitir que usuários autenticados consultem os clientes cadastrados em sua conta.                                                                                                                                                                     | **Necessário** | ✅Concluído |
| RF030 | Consulta Individual de Cliente | O sistema deve permitir que usuários autenticados consultem individualmente os dados cadastrais e financeiros de um cliente.                                                                                                                                          | **Necessário** | ✅Concluído |
| RF031 | Edição de Clientes             | O sistema deve permitir que usuários autenticados alterem os dados cadastrais de clientes existentes.                                                                                                                                                                 | **Necessário** | ✅Concluído |
| RF032 | Controle de Débito do Cliente  | O sistema deve manter o saldo de débito associado a cada cliente para possibilitar o acompanhamento de valores pendentes.                                                                                                                                             | **Necessário** | ✅Concluído |
| RF033 | Exclusão de Clientes           | O sistema deve permitir a exclusão de clientes sem comprometer registros históricos relacionados às vendas realizadas.                                                                                                                                                | **Necessário** | ✅Concluído |

## Vendas

| ID    | Requisito                        | Descrição                                                                                                                                                        | Prioridade     | Status | Observações |
| :---- | :------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------- | :-- | :-- |
| RF034 | Registro de Venda                | O sistema deve permitir que usuários autenticados registrem uma venda associando-a a um **cliente** e a pelo menos **um produto**.                               | **Necessário** | ✅Concluído |
| RF035 | Registro de Itens da Venda       | O sistema deve registrar, para cada item de uma venda, o **produto, quantidade comercializada e preço unitário praticado no momento da venda**.                  | **Necessário** | ✅Concluído |
| RF036 | Cálculo do Valor da Venda        | O sistema deve calcular o subtotal de cada item e o valor total da venda a partir das quantidades e dos preços unitários registrados.                            | **Necessário** | ✅Concluído |
| RF037 | Preservação do Preço da Venda    | O sistema deve preservar o preço unitário praticado no momento da venda, independentemente de alterações posteriores realizadas no preço cadastrado do produto.  | **Necessário** | ✅Concluído |
| RF038 | Consulta de Vendas               | O sistema deve permitir que usuários autenticados consultem as vendas registradas, incluindo **cliente, itens, quantidades, valores, data e situação da venda**. | **Necessário** | ✅Concluído |
| RF039 | Filtragem de Vendas por Situação | O sistema deve permitir que as vendas sejam consultadas de acordo com sua situação, distinguindo ao menos vendas **concluídas** e **canceladas**.                | **Desejável**  | ⏳Pendente |
| RF040 | Cancelamento de Venda            | O sistema deve permitir o cancelamento de uma venda sem remover fisicamente seu registro, preservando-a para fins de histórico.                                  | **Necessário** | ✅Concluído |

## Contas

| ID    | Requisito                        | Descrição                                                                                                                | Prioridade     | Status | Observações |
| :---- | :------------------------------- | :----------------------------------------------------------------------------------------------------------------------- | :------------- | :-- | :-- |
| RF041 | Cadastro de Contas               | O sistema deve permitir que usuários autenticados cadastrem contas informando **descrição, valor e data de vencimento**. | **Necessário** | ✅Concluído |
| RF042 | Consulta de Contas               | O sistema deve permitir que usuários autenticados consultem as contas cadastradas em sua conta.                          | **Necessário** | ✅Concluído |
| RF043 | Consulta Individual de Conta     | O sistema deve permitir que usuários autenticados consultem individualmente os dados de uma conta cadastrada.            | **Necessário** | ✅Concluído |
| RF044 | Controle da Situação da Conta    | O sistema deve manter a situação de cada conta, distinguindo ao menos contas **pendentes** e **pagas**.                  | **Necessário** | ✅Concluído |
| RF045 | Registro de Pagamento            | O sistema deve permitir que usuários autenticados registrem uma conta pendente como paga.                                | **Necessário** | ✅Concluído |
| RF046 | Filtragem de Contas por Situação | O sistema deve permitir que as contas sejam consultadas de acordo com sua situação de pagamento.                         | **Desejável**  | ⏳Pendente |
| RF047 | Exclusão de Contas               | O sistema deve permitir que usuários autenticados excluam contas cadastradas.                                            | **Necessário** | ✅Concluído |
