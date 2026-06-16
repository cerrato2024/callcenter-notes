<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>William's Sam's Club Toolkit</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

body{
  font-family:Arial, sans-serif;
  background:#f4f6f9;
}

header{
  background:#0057b8;
  color:white;
  text-align:center;
  padding:25px;
  font-size:32px;
  font-weight:bold;
}

.container{
  max-width:1200px;
  margin:auto;
  padding:20px;
}

.search{
  width:100%;
  padding:15px;
  font-size:16px;
  border:1px solid #ccc;
  border-radius:10px;
  margin-bottom:20px;
}

.section{
  background:white;
  padding:20px;
  border-radius:12px;
  margin-bottom:25px;
  box-shadow:0 2px 8px rgba(0,0,0,.1);
}

.section h2{
  color:#0057b8;
  margin-bottom:15px;
  border-bottom:2px solid #0057b8;
  padding-bottom:10px;
}

.card{
  background:#f8f9fa;
  padding:15px;
  margin-bottom:15px;
  border-left:5px solid #0057b8;
  border-radius:8px;
}

.copy-btn{
  background:#0057b8;
  color:white;
  border:none;
  padding:8px 12px;
  border-radius:5px;
  cursor:pointer;
  margin-top:10px;
}

.copy-btn:hover{
  background:#003f85;
}
</style>

</head>

<body>

<header>
William's Sam's Club Toolkit
</header>

<div class="container">

<input type="text" class="search" id="searchInput" placeholder="Search scripts...">

<!-- GREETING -->
<div class="section">
<h2>🤝 Greeting</h2>

<div class="card">
<p>Hello! Thank you for contacting Sam's Club. I hope you're doing well today. My name is William, and I'll be assisting you. To get started, could you please provide the phone number and email address?</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>
</div>

<!-- EMPATHY -->
<div class="section">
<h2>❤️ Empathy Statements</h2>

<div class="card">
<p>I completely understand your concern, and I sincerely apologize for any frustration this situation may have caused.</p>
<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p>I completely understand how concerning this situation must be for you, and I sincerely apologize for the inconvenience.</p>
<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

</div>

<!-- HOLD -->
<div class="section">
<h2>⏳ Hold Scripts</h2>

<div class="card">
<p>Please allow me a couple of minutes while I carefully review the order details.</p>
<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>
</div>

<!-- SOLUTIONS -->
<div class="section">
<h2>🛠️ Solutions</h2>

<div class="card">
<p>I can either process a replacement or a refund. Please let me know which option you prefer.</p>
<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>
</div>

<!-- CLOSING -->
<div class="section">
<h2>✅ Closings</h2>

<div class="card">
<p>Thank you for contacting Sam's Club. It was my pleasure assisting you. Have a wonderful day.</p>
<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>
</div>

</div>

<script>
function copyCard(button){
  let text = button.parentElement.querySelector("p").innerText;
  navigator.clipboard.writeText(text);

  button.innerText = "✅ Copied!";
  setTimeout(() => {
    button.innerText = "📋 Copy";
  }, 2000);
}
</script>

</body>
</html>
