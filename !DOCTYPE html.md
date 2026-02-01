#   
  
<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<title>Be My Valentine 💖</title>  
<style>  
  body {  
    height: 100vh;  
    display: flex;  
    align-items: center;  
    justify-content: center;  
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);  
    font-family: Arial, sans-serif;  
    overflow: hidden;  
  }  
  
  .card {  
    background: white;  
    padding: 30px;  
    border-radius: 15px;  
    text-align: center;  
    box-shadow: 0 10px 30px rgba(0,0,0,0.2);  
  }  
  
  h1 {  
    color: #ff4d6d;  
  }  
  
  button {  
    padding: 10px 20px;  
    font-size: 18px;  
    border: none;  
    border-radius: 10px;  
    cursor: pointer;  
    margin: 10px;  
  }  
  
  #yesBtn {  
    background: #ff4d6d;  
    color: white;  
  }  
  
  #noBtn {  
    background: #ccc;  
    position: absolute;  
  }  
</style>  
</head>  
  
<body>  
  
<div class="card">  
  <h1>Will you be my Valentine? 💝</h1>  
  <button id="yesBtn" onclick="yesClicked()">YES 💕</button>  
  <button id="noBtn">NO 🙈</button>  
</div>  
  
<script>  
  const noBtn = document.getElementById("noBtn");  
  
  noBtn.addEventListener("mouseover", () => {  
    const x = Math.random() * (window.innerWidth - noBtn.offsetWidth);  
    const y = Math.random() * (window.innerHeight - noBtn.offsetHeight);  
    noBtn.style.left = x + "px";  
    noBtn.style.top = y + "px";  
  });  
  
  function yesClicked() {  
    document.body.innerHTML = `  
      <div style="text-align:center; margin-top:20%">  
        <h1 style="color:white; font-size:40px;">Yayyyy! 💖🥰</h1>  
        <p style="color:white; font-size:22px;">  
          Best Valentine ever 😘  
        </p>  
      </div>`;  
  }  
</script>  
  
</body>  
</html>  
  
