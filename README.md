<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login </title>
<style>
    *{
        box-sizing: border-box;
    }

    body{
        width: 100%;
        height: 100%;
    }

    form{
        width: 300px;
        margin: 200px auto;
        text-align: center;
    }
    input{
        display: block;
        margin: 10px auto;
        width: 250px;
        height: 30px;
    }
</style>

</head>
<body>
    <form>
        <h3>Login</h3>
        <input type="text" placeholder="Login" id="login">
        <input type="password" placeholder="Senha" id="senha">
        <input type="submit" onclick="logar(); return false">

    </form>

   
</body>
</html>

 <script>
        function logar(){
            var login = document.getElementById('login').value;
            var senha = document.getElementById('senha').value;

            if(login == "Leonardo Fernandes" && senha == "29101812"){
                alert('Sucesso');
                location.href = "https://mail.google.com/mail/u/0/#inbox";
            }else{
                alert('Usuario ou senha incorretos');
            }
        }
    </script>
