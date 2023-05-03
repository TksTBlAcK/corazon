<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>corazonlatiendo</title>
</head>
<style>
body{
    margin:0;
    padding:0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #0b1522;
}

.heart {
    height: 150px;
    width: 150px;
    background-color:red;
    position: relative;
    transform: rotate(45deg);
    box-shadow: -20px  20px 150px #f20044;
    animation: palpitar 0.5s linear infinite alternate;
    
}
.contenido {
     position: fixed;
     margin-bottom: 50px;
     text-align: center;
     
}
h1 {
    color: white
}
h2 { color : white
}

@keyframes palpitar{
    0%{
        transform: rotate(45deg) scale(1.10);
    }
    80%{
        transform: rotate(45deg) scale(1.0);
    }
    100%{
        transform: rotate(45deg) scale(0.8);
    } 
}
.heart::before{
    content: "";
    position: absolute;
    height: 150px;
    width: 150px;
    background: red;
    top: -50%;
    border-radius: 50%;
    box-shadow: 10px  20px 150px #f20044;
}
.heart::after{
    content: "";
    position: absolute;
    height: 150px;
    width: 150px;
    background: red;
    right: 50%;
    border-radius: 50%;
    box-shadow: 20px  20px 150px #f20044;
}

</style>
<body>
    <div class="heart"></div>

    <div class="contenido"><h1>Te Amo</h1><h2>Camilinda</h2></div>

  
      
</body>
</html>
