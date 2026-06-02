
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MKA Digital Card</title>

<!-- Google Font -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background: linear-gradient(135deg,#d3d3d3,#f5f5f5);
    display: flex;
    justify-content: center;
    padding: 15px;
}

/* CARD */
.card {
    width: 100%;
    max-width: 400px;
    border-radius: 20px;
    overflow: hidden;
    animation: fadeIn 1s ease;
}

/* HEADER */
.header {
    background: #000;
    padding: 20px;
    border-radius: 20px;
    position: relative;
    color: white;
}

.logo {
    text-align: center;
    margin-bottom: 10px;
    font-weight: bold;
    color: gold;
}

.profile {
    display: flex;
    align-items: center;
    gap: 15px;
}

.profile img {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    border: 2px solid white;
}

.info h2 {
    font-size: 16px;
}

.info p {
    font-size: 14px;
    opacity: 0.8;
}

/* BUTTON */
.save-btn {
    margin-top: 15px;
    background: #777;
    color: white;
    text-align: center;
    padding: 10px;
    border-radius: 10px;
    cursor: pointer;
    transition: 0.3s;
}

.save-btn:hover {
    background:#46c34c;
}



/* LIST ITEMS */
.list {
    margin-top: 20px;
}

.item {
    background: #000;
    color: white;
    padding: 15px;
    border-radius: 10px;
    margin-bottom: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
	

    /* animation */
    transform: translateY(0);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
	 
}

.item:hover {
    transform: translateY(-8px);
    box-shadow: 0 10px 20px rgba(212,175,55,0.35);
}

.item:active {
    transform: translateY(-3px) scale(0.97);
}

.item.call-highlight {
    border: 1px solid gold;
    box-shadow: 0 0 10px rgba(212,175,55,0.25);
}


/* MAP */
.map {
    margin-top: 10px;
}

.map iframe {
    width: 100%;
    height: 200px;
    border-radius: 10px;
}
/*footer*/
.footer {
margin-bottom:10px;
background:#000;
    display: flex;
    justify-content: center;
    padding: 15px;
}

/* ANIMATIONS */
@keyframes fadeIn {
    from {opacity:0;}
    to {opacity:1;}
}

@keyframes slideUp {
    to {
        transform: translateY(0);
        opacity: 1;
    }
}
</style>
</head>

<body>

<div class="card">

    <!-- HEADER -->
    <div class="header">
        <div class="logo"><img src="Gold geometric symbol on black.png" width = "380" height= "150"></div>

        <div class="profile">
            <img src="Nilesh S.png" alt="profile">

            <div class="info">
                <h2>Mr. Nilesh Narendra Sakarkar</h2>
                <p>Founder & Director</p>
                <p>Madhu Kusum Associates</p>
            </div>
        </div>

        <div class="save-btn" onclick="saveContact()">Save Contact</div>
    </div>


	
	<br>
	<div class="item call-highlight" onclick="callNow()">
    <span>
        <i class="fa-solid fa-phone-volume" style="color:gold;"></i>
        Call 
    </span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>
    <div class="item call-highlight" onclick="whatsapp()">
    <span><i class="fa-brands fa-whatsapp" style="color:gold;"></i> WhatsApp</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="instagram()">
    <span><i class="fa-brands fa-instagram" style="color:gold;"></i> Instagram</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="linkedin()">
    <span><i class="fa-brands fa-linkedin" style="color:gold;"></i> LinkedIn</span>
   <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="email()">
    <span><i class="fa-solid fa-envelope" style="color:gold;"></i> Email</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="website()">
    <span><i class="fa-solid fa-globe" style="color:gold;"></i> Website</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>

<div class="item call-highlight" onclick="map()">
    <span><i class="fa-solid fa-map" style="color:gold;"></i> LOCATION</span>
    <i class="fa-solid fa-angle-right" style="color:gold;"></i>
</div>
    <!-- MAP -->
    <div class="map">
       <iframe src="https://www.google.com/maps/embed?pb=!1m23!1m12!1m3!1d12268.959012656296!2d79.14356385!3d21.1368559!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!4m8!3e6!4m0!4m5!1s0x3bd4c790f55bf6fd%3A0x14540d25b9f2578!2sMADHU%20KUSUM%20AND%20ASSOCIATES%2C%20Gurukrupa%20Housing%20Society%2C%20Plot%20No.%2015%2C%20Wathoda%20Rd%2C%20near%20NMC%20School%2C%20Vathoda%2C%20Wathoda%20Layout%2C%20Nagpur%2C%20Maharashtra%20440008%2C%20India!3m2!1d21.1343434!2d79.14306479999999!5e1!3m2!1sen!2sin!4v1776774380539!5m2!1sen!2sin" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
	
	<!--footer-->
	<div class="footer">
		<img src="Untitled design.jpg" width="80" height="80" >
	</div>


<script>


// ACTIONS
function callNow() {
    window.location.href = "tel:+918007725090";
}

function whatsapp() {
    window.location.href = "https://wa.me/918007725090";
}

function instagram() {
    window.location.href = "https://instagram.com/mka.india.corp";
}

function linkedin() {
    window.location.href = "#";
}

function email() {
    window.location.href = "mailto:info.madhukusumassociates.com";
}

function website() {
    window.location.href = "https://www.madhukusumassociates.com";
}

function map() {
window.location.href = "https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d12268.959012656296!2d79.14356385!3d21.1368559!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e1!3m2!1sen!2sin!4v1776776041739!5m2!1sen!2sin";
}

// VCARD DOWNLOAD
function saveContact() {
    const vcard = `
BEGIN:VCARD
VERSION:3.0
FN:Nilesh Narendra Sakarkar
ORG:Madhu Kusum Associates
TEL:+918007725090
EMAIL:info.madhukusumassociates.com
END:VCARD
`;

    const blob = new Blob([vcard], { type: "text/vcard" });
    const url = URL.createObjectURL(blob);

    const a = document.createElement("a");
    a.href = url;
    a.download = "contact.vcf";
    a.click();
}

</script>

