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

<div class="section">

<h2>🤝 Greeting</h2>

<div class="card">
<p>Hello! Thank you for contacting Sam's Club. I hope you're doing well today. My name is William, and I'll be assisting you. To get started, could you please provide the phone number and email address, please?</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>

</div>

</div>

</div>
<div class="section">

<h2>❤️ Empathy Statements</h2>

<div class="card">
<p>I completely understand your concern, and I sincerely apologize for any frustration or inconvenience this situation may have caused. I can certainly understand how important it is to have this resolved as quickly as possible. Please rest assured that I'm here to assist you, and I'll do my best to review the details thoroughly and determine the best available resolution for you today.</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p>I completely understand how concerning this situation must be for you, and on behalf of Sam's Club, I sincerely apologize for the inconvenience. This is certainly not the experience we want for our valued members. Please rest assured that I am here to help, and I will take full ownership of reviewing the details and exploring the best available solution for you.</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p><strong>Damaged Item:</strong><br><br>
I completely understand how frustrating and disappointing this situation must be for you. Receiving a damaged item is certainly not the experience we want for our valued members at Sam's Club. On behalf of Sam's Club, I sincerely apologize for the inconvenience this has caused. Please rest assured that I am here to assist you. Let me take a closer look at your order details so I can determine the best available resolution and make this right for you.</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p><strong>Missing Item:</strong><br><br>
I completely understand your concern, and I sincerely apologize for the frustration this situation may have caused. I can certainly understand how important it is to receive every item you purchased. At Sam's Club, we strive to provide a seamless shopping experience, and this is certainly not the experience we want for our valued members. Please rest assured that I am here to help. Let me review the order and shipment details to determine what happened and identify the best available resolution for you today.</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p><strong>Order Delay:</strong><br><br>
I completely understand your concern, and I sincerely apologize for the frustration this delay may have caused. I can certainly appreciate how important it is to receive your order on time. At Sam's Club, we value our members and understand the importance of a reliable delivery experience. Please rest assured that I am here to help. Let me investigate the order and shipment details, review the most recent tracking information, and explore the best available options to assist you today.</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

</div>
<script>

function copyCard(button){

let text = button.parentElement.querySelector("p").innerText;

navigator.clipboard.writeText(text);

button.innerText = "✅ Copied!";

setTimeout(function(){
button.innerText = "📋 Copy";
},2000);

}
<div class="section">

<h2>⏳ Hold Scripts</h2>

<div class="card">
<p><strong>Request Hold:</strong><br><br>
Please allow me a couple of minutes while I carefully review the order details and investigate this matter further. I want to ensure I provide you with the most accurate information and the best available resolution. I'll be back with an update shortly.
</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p><strong>After Hold:</strong><br><br>
Thank you for your patience while I reviewed the details. I appreciate you taking the time to wait. I have completed my review, and I'd be happy to share the information I found and discuss the next available steps with you.
</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

</div>

<div class="section">

<h2>🛠️ Solutions</h2>

<div class="card">
<p><strong>Available Options:</strong><br><br>
I reviewed the details. Based on my review, I do have a couple of options available for you. I can either process a replacement order so that a new item can be shipped to you, or I can process a refund back to your original method of payment. Please let me know which option works best for you, and I'll be happy to assist you further.
</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p><strong>Refund Approved:</strong><br><br>
Thank you for confirming your preference. I have successfully submitted the refund request of XXXX. You will receive a confirmation email shortly, and the funds will typically be reflected in your account within the next 5 to 7 business days, depending on your financial institution. Is there anything else I can assist you with today?
</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

<div class="card">
<p><strong>Replacement Approved:</strong><br><br>
Thank you for confirming that you would like a replacement. I have successfully submitted the replacement request for you. On behalf of Sam's Club, we appreciate the opportunity to resolve this matter. You should receive a confirmation email shortly, and tracking information will become available once the replacement shipment is processed. Please let me know if there is anything else I can assist you with today.
</p>

<button class="copy-btn" onclick="copyCard(this)">📋 Copy</button>
</div>

</div>
</script>

</body>
</html>
