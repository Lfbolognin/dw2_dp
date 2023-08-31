# dw2_dp

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js">  </script>
  <script>
   function funcaoNovo(){
   
            document.getElementById("btnAlter").disabled = true;
            document.getElementById("btnExcluir").disabled = true;
            document.getElementById("btnSalvar").disabled = false;
            document.getElementById("btnPesquisar").disabled = true;
            document.getElementById("btnCancelar").disabled = false;
            
            document.getElementById("txtNome").disabled = false;
            document.getElementById("txtCPF").disabled = false;
            document.getElementById("txtMatricula").disabled = false;
            document.getElementById("txtTurno").disabled = false;
            document.getElementById("txtRA").disabled = false;
            document.getElementById("txtCR").disabled = false;
            document.getElementById("txtEmail").disabled = false;
            document.getElementById("txtData_ingresso").disabled = false;
            
           document.getElementById("txtNome").value ="";
           document.getElementById("txtCPF").value ="";
           document.getElementById("txtMatricula").value ="";
           document.getElementById("txtTurno").value ="";
           document.getElementById("txtRA").value ="";
           document.getElementById("txtCR").value ="";
           document.getElementById("txtEmail").value ="";
           document.getElementById("txtData_ingresso").value ="";
           

            
        }
        
         function funcaoAlter(){
   
   			document.getElementById("btnNovo").disabled = false;
            document.getElementById("btnSalvar").disabled = true;
            document.getElementById("btnExcluir").disabled = true;
            document.getElementById("btnPesquisar").disabled = true;
            document.getElementById("btnCancelar").disabled = false;
        }
        
        function funcaoExcluir(){
   
   			document.getElementById("btnNovo").disabled = false;
            document.getElementById("btnAlter").disabled = true;
            document.getElementById("btnSalvar").disabled = true;
            document.getElementById("btnPesquisar").disabled = false;
            document.getElementById("btnCancelar").disabled = false;
        }
        
         function funcaoPesquisa(){
   
   			document.getElementById("btnNovo").disabled = false;
            document.getElementById("btnAlter").disabled = true;
            document.getElementById("btnExcluir").disabled = true;
            document.getElementById("btnSalvar").disabled = true;
            document.getElementById("btnCancelar").disabled = false;
        }
        
  function funcaoSalvar(){
   
   			document.getElementById("btnNovo").disabled = false;
            document.getElementById("btnAlter").disabled = true;
            document.getElementById("btnExcluir").disabled = true;
            document.getElementById("btnPesquisar").disabled = true;
            document.getElementById("btnCancelar").disabled = false;
            
            localStorage.setItem("nome", document.getElementById
            ("txtNome").value);
            
             localStorage.setItem("matricula", document.getElementById
            ("txtMatricula").value);
            
            localStorage.setItem("turno", document.getElementById
            ("txtTurno").value);
            
            localStorage.setItem("ra", document.getElementById
            ("txtRA").value);
            
            localStorage.setItem("cr", document.getElementById
            ("txtCR").value);
            
            localStorage.setItem("cpf", document.getElementById
            ("txtCPF").value);
            
            localStorage.setItem("email", document.getElementById
            ("txtEmail").value);
            
            localStorage.setItem("data_ingresso", document.getElementById
            ("txtData_ingresso").value);
            
            window.alert("NOME: " +localStorage.getItem("nome") + "\n"
            + "CPF: " +localStorage.getItem("cpf") + "\n"
            + "Matricula: " +localStorage.getItem("matricula") + "\n"
            + "Turno: " +localStorage.getItem("turno") + "\n"
            + "RA: " +localStorage.getItem("ra") + "\n"
            + "CR: " +localStorage.getItem("cr") + "\n"
            + "Email: " +localStorage.getItem("email") + "\n"
            + "Data de Ingresso: " +localStorage.getItem("data_ingresso") + "\n"

            
            
            
            
            );
            
            
        }
        
      
        
         function funcaoCancelar(){
   
   			document.getElementById("btnNovo").disabled = false;
            document.getElementById("btnAlter").disabled = true;
            document.getElementById("btnExcluir").disabled = true;
            document.getElementById("btnPesquisar").disabled = false;
            document.getElementById("btnSalvar").disabled = true;
        }
  </script>
</head>

<body>

<span> Nome: </span> <input type = "text" class = "form-control" id="txtNome" disabled >

<br>

<span> CPF: </span> <input type = "text" class = "form-control" id="txtCPF" disabled >
<br>

<span> Matricula: </span> <input type = "text" class = "form-control" id="txtMatricula" disabled >

<br>

<span> Turno: </span> <input type = "text" class = "form-control" id="txtTurno" disabled >

<br>

<span> RA: </span> <input type = "text" class = "form-control" id="txtRA" disabled >

<br>

<span> CR: </span> <input type = "text" class = "form-control" id="txtCR" disabled >

<BR>


<span> Email: </span> <input type = "text" class = "form-control" id="txtEmail" disabled >

<br>

<span> Data de ingresso: </span> <input type = "text" class = "form-control" id="txtData_ingresso" disabled >

<br>

 <button type="button" id="btnNovo" class="btn btn-primary"
    onclick="funcaoNovo()">Novo </button>

    <button type="button" id="btnAlter" class="btn btn-primary"
    onclick="funcaoAlter()">Alterar</button>
    
    <button type="button" id="btnExcluir" class="btn btn-primary"
    onclick="funcaoExcluir()">Excluir</button>
    
    <button type="button" id="btnPesquisar" class="btn btn-primary"
    onclick="funcaoPesquisa()">Pesquisar</button>
    
    <button type="button" id="btnSalvar" class="btn btn-primary"
    onclick="funcaoSalvar()">Salvar</button>
    
    <button type="button" id="btnCancelar" class="btn btn-primary"
    onclick="funcaoCancelar()">Cancelar</button>
    
    
    

</body>
</html>
