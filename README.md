# aulajovander8-8
# Lista de Clientes (Azure SQL + PHP)

## Descrição
Projeto de exemplo para listar registros da tabela `Clientes` hospedada em Azure SQL Database usando PHP (PDO).

## Como configurar o banco na Azure
1. No portal.azure.com → Create resource → SQL Database.
2. Criar servidor SQL com login e senha.
3. No SQL Server → Networking → Add client IP (adicionar seu IP).
4. No Database → Query editor: executar o script `script.sql` para criar a tabela e inserir 30 registros.

## Como configurar o PHP local (XAMPP)
1. Instale XAMPP e inicie o Apache.
2. Instale Microsoft ODBC Driver e os drivers `php_sqlsrv` / `php_pdo_sqlsrv` compatíveis com sua versão do PHP.
3. Copie `config.sample.php` para `config.php` e preencha `server`, `database`, `username`, `password`.
4. Abra `http://localhost/clientes_azure/index.php`.

## Observações
- Não incluir `config.php` no repositório (arquivo está no .gitignore).
- Se tiver problema de conexão, verifique se o IP foi liberado no Firewall do servidor SQL.
