# Sistema Bancário V5

Projeto do Curso Python da DIO

Novas funções:
* Modificar o atual decorador de log que imprime informações no console, para que salve as informações em um arquivo de log.
    * Requisitos:
        * Data e hora atuais;
        * Nome da função;
        * Argumentos da função;
        * Valor Retornado pela função;
        * O arquivo log deve se chamar log.txt;
        * Se o arquivo log.txt já existir, os novos logs devem ser adicionados no final do arquivo;
        * Cada entrada de log deve estar em uma nova linha.



## Regras de cada função
### Depósito
* Todos os depósitos devem ser registrados em uma váriavel;
* O valor não pode ser negativo;
* Todas operações devem ser registradas em Extrato.

### Saque
*  O Sistema permite três saques por dia;
* Limite de saque de R$ 500 por dia;
* Caso uma das opções acima apresentar erro, exibir mensagem;
* Caso não tenha saldo apresentar mensagem de saldo insuficiente;
* Todas as operações devem ser registradas em Extrato.

### Extrato
* Deve listar todas as operações;
* No final Mostrar o saldo atual da conta;
* Se não não tiver movimentações, exibir (*Não foram realizadas movimentações.*)

### Criar usuário
* O Programa deve armazenar os usuários em lista;
* Composição do usuário:
    * Nome;
    * Data de nascimento;
    * CPF;
    * Endereço: (Logradouro, nro, bairro, cidade/sigla estado);
* Não pode cadastrar 2 usuários com o mesmo CPF.

### Criar Conta
* O Programa deve armazenar contas em lista;
* Composição da conta:
    * Agência;
    * Número da conta;
    * Usuário.
* Número da conta é sequencial;
* Número da agência é fixo.
* Um usuário pode ter mais de uma conta, mas uma conta pertence somente a um usuário.

### Listar conta
* Exibir lista de contas;
* Composição da lista:
    * Agência;
    * Número da conta;
    * Nome do titular.

### Decorador de log:
 * Esse decorador deve registra data e hora de cada transação (depósito, saque, criação de conta, etc);
### Gerador de Relatórios
* Permitir iterar sobre as transações de uma conta e retornar uma a uma as transações realizados;
* Ter uma forma de filtrar as transações baseado no tipo (apenas deposito ou saques).
### Iterador personalizado
* Implementar um iterador personalizado que permita iterar sobre todas as contas do banco retornando informações básicas de cada conta (número, saldo atual, etc).
* Estabelecer um limite de 10 transações diárias para uma conta;
* Se o usuário tentar fazer uma transação após atingir o limite, deve ser informado que ele execeu o número de transações permitidas para aquele dia;

### Observações
* É possível um usuário ter mais de uma conta, porém no momento das transações não é possível especificar a conta.
* Dados de clientes e contas são armazenados em objetos ao invés de dicionário.