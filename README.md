# Sistema de Registro de Músicas em Banco de Dados, com interface!

### Use xampp para hospedar o site, caso queira fazer upload para um servidor, modifique os arquivos com usuário, senha e nome do banco de dados para o funcionamento correto

### Código de conexão com banco de dados (conexao.php)
```
<?php
try {
    $servername = "localhost"; //Geralmente é padrão, caso de erro use 127.0.0.1
    $username = "SEU USUÁRIO";
    $password = "SUA SENHA";
    $dbname = "SEU BANCO DE DADOS";
    $conn = new mysqli($servername, $username, $password, $dbname);
    //echo "Top";
} catch ( mysqli_sql_exception $e ){
    echo "Erro de conexão:" . $e->getMessage();
}
```
