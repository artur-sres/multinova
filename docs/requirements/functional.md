# Requisitos Funcionais

Template de linha:
| RFXXX | Nome do Requisito | Descrição do requisito, explicando o que o sistema deve fazer. | Necessário | ⏳Pendente | |

## Autenticação e Usuários

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF001 | Cadastro de Usuário | O sistema deve permitir o cadastro de usuários mediante o fornecimento de nome, endereço de e-mail e senha. | Necessário | ✅Concluído | |
| RF002 | Verificação de E-mail | O sistema deve exigir a verificação do endereço de e-mail do usuário por meio de um código de verificação antes de disponibilizar o acesso completo à conta. | Necessário | ✅Concluído | |
| RF003 | Autenticação de Usuário | O sistema deve permitir que usuários cadastrados e verificados realizem autenticação utilizando e-mail e senha. | Necessário | ✅Concluído | |
| RF004 | Controle de Sessão | O sistema deve fornecer um token de autenticação após a autenticação bem-sucedida do usuário, permitindo o acesso aos recursos protegidos do sistema. | Necessário | ✅Concluído | |
| RF005 | Recuperação de Senha | O sistema deve permitir que usuários solicitem a recuperação de senha por meio do endereço de e-mail associado à conta. | Necessário | ✅Concluído | |
| RF006 | Redefinição de Senha | O sistema deve permitir a redefinição da senha mediante a validação do e-mail, código de recuperação e nova senha. | Necessário | ✅Concluído | |
| RF007 | Consulta de Dados do Usuário | O sistema deve permitir que usuários autenticados consultem os dados associados à sua conta. | Necessário | ⏳Pendente | |
| RF008 | Edição de Dados do Usuário | O sistema deve permitir que usuários autenticados alterem os dados editáveis associados à sua conta. | Necessário | ⏳Pendente | |

## Marcas

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF009 | Cadastro de Marcas | O sistema deve permitir que usuários autenticados cadastrem marcas para classificação dos produtos. | Necessário | ✅Concluído | |
| RF010 | Consulta de Marcas | O sistema deve permitir que usuários autenticados consultem as marcas cadastradas em sua conta. | Necessário | ✅Concluído | |
| RF011 | Edição de Marcas | O sistema deve permitir que usuários autenticados alterem os dados de marcas previamente cadastradas. | Necessário | ✅Concluído | |
| RF012 | Exclusão de Marcas | O sistema deve permitir que usuários autenticados excluam marcas cadastradas, desde que a operação não viole as regras de integridade dos dados associados. | Necessário | ✅Concluído | |

## Categorias

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF013 | Cadastro de Categorias | O sistema deve permitir que usuários autenticados cadastrem categorias para classificação dos produtos. | Necessário | ✅Concluído | |
| RF014 | Consulta de Categorias | O sistema deve permitir que usuários autenticados consultem as categorias cadastradas em sua conta. | Necessário | ✅Concluído | |
| RF015 | Edição de Categorias | O sistema deve permitir que usuários autenticados alterem os dados de categorias previamente cadastradas. | Necessário | ✅Concluído | |
| RF016 | Exclusão de Categorias | O sistema deve permitir que usuários autenticados excluam categorias cadastradas, desde que a operação não viole as regras de integridade dos dados associados. | Necessário | ✅Concluído | |

## Produtos

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF017 | Cadastro de Produtos | O sistema deve permitir que usuários autenticados cadastrem produtos informando, obrigatoriamente, o nome do produto e, quando aplicável, quantidade em estoque, preço de compra e preço de venda. O cadastro poderá conter descrição, imagem, categoria, marca e código da marca. | Necessário | ⏳Pendente | Faltando somente o upload das imagens |
| RF018 | Consulta de Produtos | O sistema deve permitir que usuários autenticados consultem os produtos cadastrados em sua conta. | Necessário | ✅Concluído | |
| RF019 | Consulta de Produto | O sistema deve permitir que usuários autenticados consultem individualmente os dados de um produto cadastrado. | Necessário | ✅Concluído | |
| RF020 | Edição de Produtos | O sistema deve permitir que usuários autenticados alterem os dados cadastrais de produtos existentes, incluindo nome, descrição, imagem, categoria, marca, código da marca e quantidade em estoque. | Necessário | ⏳Pendente | |
| RF021 | Controle de Estoque | O sistema deve manter a quantidade disponível em estoque para cada produto cadastrado e impedir o registro de valores negativos de estoque. | Necessário | ✅Concluído | |
| RF022 | Exclusão de Produtos | O sistema deve permitir a exclusão de produtos sem comprometer os registros históricos que façam referência ao produto, incluindo vendas e históricos de clientes. | Necessário | ✅Concluído | |
| RF023 | Recuperação de Produtos Excluídos | O sistema deve permitir que usuários autenticados recuperem produtos previamente excluídos. | Desejável | ⏳Pendente | |
| RF048 | Histórico de Movimentação de Estoque | O sistema deve manter um histórico cronológico das movimentações de entrada e saída de estoque de cada produto. | Importante | ⏳Pendente | |
| RF049 | Busca de Produtos | O sistema deve permitir a busca de produtos por nome e código de identificação de marca. | Necessário | ⏳Pendente | |
| RF050 | Filtragem de Produtos | O sistema deve permitir a filtragem de produtos por marca, categoria e faixa de preço. | Importante | ⏳Pendente | |
| RF051 | Promoções | O sistema deve permitir a definição de preços promocionais para produtos sem alterar os preços registrados em vendas anteriores. | Desejável | ⏳Pendente | |
| RF052 | Período de Promoção | O sistema deve permitir que uma promoção possua data de início e término, retornando automaticamente ao preço regular após o encerramento. | Necessário | ⏳Pendente | Depende de RF051. Obrigatório caso promoções sejam implementadas. |

## Preços

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF024 | Registro de Preços | O sistema deve permitir o registro do preço de compra e preço de venda associado a um produto. | Necessário | ✅Concluído | |
| RF025 | Histórico de Preços | O sistema deve preservar os registros anteriores de preço de cada produto, mantendo um histórico das alterações realizadas ao longo do tempo. | Necessário | ✅Concluído | |
| RF026 | Consulta do Histórico de Preços | O sistema deve permitir que usuários autenticados consultem o histórico de preços registrado para um produto. | Necessário | ✅Concluído | |
| RF027 | Consulta do Preço Atual | O sistema deve permitir que usuários autenticados consultem o preço vigente de um produto. | Necessário | ✅Concluído | |

## Clientes

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF028 | Cadastro de Clientes | O sistema deve permitir que usuários autenticados cadastrem clientes contendo, obrigatoriamente, nome e os dados financeiros necessários ao controle de débitos. O cadastro poderá incluir endereço, telefone, data de nascimento, fotografia e preferências. | Necessário | ⏳Pendente | Faltando somente upload das imagens |
| RF029 | Consulta de Clientes | O sistema deve permitir que usuários autenticados consultem os clientes cadastrados em sua conta. | Necessário | ✅Concluído | |
| RF030 | Consulta Individual de Cliente | O sistema deve permitir que usuários autenticados consultem individualmente os dados cadastrais e financeiros de um cliente. | Necessário | ✅Concluído | |
| RF031 | Edição de Clientes | O sistema deve permitir que usuários autenticados alterem os dados cadastrais de clientes existentes. | Necessário | ✅Concluído | |
| RF032 | Controle de Débito do Cliente | O sistema deve manter o saldo de débito associado a cada cliente para possibilitar o acompanhamento de valores pendentes. | Necessário | ✅Concluído | |
| RF033 | Inativação de Clientes | O sistema deve permitir que clientes sejam marcados como inativos sem que seus registros históricos sejam removidos. | Necessário | ✅Concluído | |
| RF053 | Busca de Clientes | O sistema deve permitir a busca de clientes pelo nome. | Necessário | ⏳Pendente | |
| RF054 | Histórico do Cliente | O sistema deve manter o histórico de operações relacionadas ao cliente, incluindo compras, pagamentos e cancelamentos. | Necessário | ⏳Pendente | Parcialmente feito |
| RF055 | Pagamentos Parciais | O sistema deve permitir o registro de pagamentos parciais sobre valores devidos por um cliente. | Necessário | ⏳Pendente | |
| RF056 | Relatório Individual do Cliente | O sistema deve permitir a geração de relatório contendo dados cadastrais, histórico de compras, pagamentos e saldo do cliente. | Desejável | ⏳Pendente | |
| RF057 | Exportação de Relatório do Cliente | O sistema deve permitir a exportação do relatório individual do cliente em formato PDF. | Desejável | ⏳Pendente | |
| RF058 | Lembrete de Aniversário | O sistema deve gerar um lembrete antecipado para aniversários de clientes cadastrados. | Desejável | ⏳Pendente | |
| RF059 | Lembrete de Débito | O sistema deve gerar um alerta quando o débito de um cliente permanecer pendente por determinado período. | Importante | ⏳Pendente | |

## Vendas

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF034 | Registro de Venda | O sistema deve permitir que usuários autenticados registrem uma venda associando-a a um cliente e a pelo menos um produto. | Necessário | ✅Concluído | |
| RF035 | Registro de Itens da Venda | O sistema deve registrar, para cada item de uma venda, o produto, quantidade comercializada e preço unitário praticado no momento da venda. | Necessário | ✅Concluído | |
| RF036 | Cálculo do Valor da Venda | O sistema deve calcular o subtotal de cada item e o valor total da venda a partir das quantidades e dos preços unitários registrados. | Necessário | ✅Concluído | |
| RF037 | Preservação do Preço da Venda | O sistema deve preservar o preço unitário praticado no momento da venda, independentemente de alterações posteriores realizadas no preço cadastrado do produto. | Necessário | ✅Concluído | |
| RF038 | Consulta de Vendas | O sistema deve permitir que usuários autenticados consultem as vendas registradas, incluindo cliente, itens, quantidades, valores, data e situação da venda. | Necessário | ✅Concluído | |
| RF039 | Filtragem de Vendas por Situação | O sistema deve permitir que as vendas sejam consultadas de acordo com sua situação, distinguindo ao menos vendas concluídas e canceladas. | Desejável | ⏳Pendente | |
| RF040 | Cancelamento de Venda | O sistema deve permitir o cancelamento de uma venda sem remover fisicamente seu registro, preservando-a para fins de histórico. | Necessário | ✅Concluído | |
| RF060 | Desconto em Venda | O sistema deve permitir a aplicação de desconto sobre uma venda ou sobre itens específicos da venda. | Desejável | ⏳Pendente | |
| RF061 | Edição do Preço na Venda | O sistema deve permitir que o preço de venda de um produto seja alterado durante o registro da venda sem modificar seu preço cadastrado. | Desejável | ⏳Pendente | |
| RF062 | Forma de Pagamento | O sistema deve registrar, para cada venda, a forma de pagamento utilizada. | Necessário | ⏳Pendente | |
| RF063 | Devolução de Produtos | O sistema deve permitir registrar a devolução de produtos vendidos e realizar os ajustes correspondentes no estoque. | Desejável | ⏳Pendente | |
| RF064 | Histórico Detalhado de Vendas | O sistema deve permitir consultar vendas por período e forma de pagamento, por clientes, com acesso aos detalhes de cada venda. | Desejável | ⏳Pendente | |

## Despesas

| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF041 | Cadastro de Contas | O sistema deve permitir que usuários autenticados cadastrem contas informando descrição, valor e data de vencimento. | Necessário | ✅Concluído | |
| RF042 | Consulta de Contas | O sistema deve permitir que usuários autenticados consultem as contas cadastradas em sua conta. | Necessário | ✅Concluído | |
| RF043 | Consulta Individual de Conta | O sistema deve permitir que usuários autenticados consultem individualmente os dados de uma conta cadastrada. | Necessário | ✅Concluído | |
| RF044 | Controle da Situação da Conta | O sistema deve manter a situação de cada conta, distinguindo ao menos contas pendentes e pagas. | Necessário | ✅Concluído | |
| RF045 | Registro de Pagamento | O sistema deve permitir que usuários autenticados registrem uma conta pendente como paga. | Necessário | ✅Concluído | |
| RF046 | Filtragem de Contas por Situação | O sistema deve permitir que as contas sejam consultadas de acordo com sua situação de pagamento. | Desejável | ⏳Pendente | |
| RF047 | Exclusão de Contas | O sistema deve permitir que usuários autenticados excluam contas cadastradas. | Necessário | ✅Concluído | |
| RF065 | Registro de Receitas | O sistema deve permitir o registro de receitas financeiras. | Necessário | ⏳Pendente | |
| RF066 | Registro de Despesas | O sistema deve permitir o registro de despesas financeiras. | Necessário | ⏳Pendente | |
| RF067 | Alerta de Vencimento | O sistema deve gerar alertas para contas de fornecedores próximas do vencimento. | Necessário | ⏳Pendente | |

## Catálogo
| ID | Requisito | Descrição | Prioridade | Status | Observações |
|---|---|---|---|---|---|
| RF068 | Catálogo Público | O sistema deve disponibilizar um catálogo público contendo os produtos com pelo menos uma unidade em estoque. | Desejável | ⏳Pendente | |
| RF069 | Consulta sem Autenticação | O sistema deve permitir que o catálogo público seja acessado sem autenticação. | Necessário | ⏳Pendente | Depende de RF068. Obrigatório caso o catálogo seja implementado. |
| RF070 | Estoque no Catálogo | O catálogo deve refletir a disponibilidade atual dos produtos. | Necessário | ⏳Pendente | Depende de RF068. Obrigatório caso o catálogo seja implementado. |
| RF071 | Organização do Catálogo | O sistema deve permitir organizar ou consultar os produtos do catálogo por marca e categoria. | Importante | ⏳Pendente | Depende de RF068. |
| RF072 | Busca no Catálogo | O catálogo deve permitir a busca de produtos. | Importante | ⏳Pendente | Depende de RF068. |
| RF073 | Compartilhamento do Catálogo | O sistema deve fornecer um endereço compartilhável para acesso ao catálogo. | Necessário | ⏳Pendente | Depende de RF068. Obrigatório caso o catálogo seja implementado. |

