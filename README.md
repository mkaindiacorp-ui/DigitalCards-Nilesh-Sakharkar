<!DOCTYPE html>
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
        <div class="logo"><img src="crop.png" width = "360" height= " 100"></div>

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

    <!-- MAP -->
    <div class="map">
        <iframe 
        src="https://maps.google.com/maps?q=Nagpur&t=&z=13&ie=UTF8&iwloc=&output=embed">
        </iframe>
    </div>
	
	<!--footer-->
	<div class="footer">
		<img src="Untitled-4 (1) (2).png" width="80" height="80" >
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
window.location.href = "https://www.google.com/maps/dir//MADHU+KUSUM+AND+ASSOCIATES,+Gurukrupa+Housing+Society,+Plot+No.+15,+Wathoda+Rd,+near+NMC+School,+Vathoda,+Wathoda+Layout,+Nagpur,+Maharashtra+440008/@21.1104057,79.0983953,15z/data=!4m8!4m7!1m0!1m5!1m1!1s0x3bd4c790f55bf6fd:0x14540d25b9f2578!2m2!1d79.1430648!2d21.1343434?entry=ttu&g_ep=EgoyMDI2MDQwNS4wIKXMDSoASAFQAw%3D%3D";
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

</body>
</html>
