<style>
body {
  background-image: url('../resources/image/background.png');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>

<html>
    <head>
        <script type="text/javascript">
            function checkPass() {
                var confirmPassword = "teste";
                var password = document.getElementById("pswd").value;
                var content = document.getElementById("content");
                var form = document.getElementById("form");
                if (password == confirmPassword) {
                    form.setAttribute("hidden", "true");
                    content.removeAttribute("hidden");
                }
                else{
                    alert("SENHA INCORRETA!");
                }
            }
        </script>
    </head>
    <body>
        <h1 style="font-size:30px;color:orange;text-align:center"><b>STAFF</b></h1>
        <form style="text-align:center" id='form'>
            <label for="pswd">Coloque sua senha:<br> </label>
            <input style="color:black" type="password" id="pswd">
            <input style="color: white;background: #1d1e26;" type="button" value="ENVIAR" onclick="checkPass();" />
        </form>   
        <div id='content' hidden>
            <p>teste</p>
        </div>
    </body>
</html>