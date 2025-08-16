# mileskdi.github.io
Welcome to the homepage of KDI Custom Builds!!

<title>KDI Custom Builds</title>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css" />
<style>
body { padding-bottom: 2rem; }
iframe { width: 100%; height: 300px; border: none; border-radius: 8px; margin-top: 1rem; }
.review-box { background: #f5f5f5; padding: 1rem; border-radius: 8px; margin-top: 0.5rem; }
</style>
</head>
<body>
<nav class="container-fluid">
<ul><li><strong>KDI Custom Builds</strong></li></ul>
<ul>
<li><a href="#home">Home</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#contact" role="button">Contact</a></li>
</ul>
</nav>

<main class="container" id="home">
<div class="grid">
<section>
<hgroup>
<h2>Expert Computer & Phone Repair</h2>
<h3>Reliable. Custom. Local.</h3>
</hgroup>
<p>At KDI Custom Builds, we specialize in computer and cell phone repair with a custom, high-precision touch. Whether it's water damage, broken screens, virus removal, or custom PC builds — we've got you covered.</p>
<figcaption><a href="#contact">Book a repair today</a></figcaption>
<h3 id="services">What We Repair</h3>
<p>Desktops, laptops, Android phones, iPhones, and tablets. We use high-end tools and professional methods to diagnose and repair fast.</p>
<h3>Why Choose Us?</h3>
<p>We're a local shop with custom craftsmanship, fast turnarounds, and a dedication to your satisfaction. "BELLICI • FIDEL" — loyalty in every repair.</p>
</section>
</div>
</main>

<section class="container" id="appointment">
<hgroup>
<h2>Request an Appointment</h2>
<h3>Tell us when you’d like to come in</h3>
</hgroup>
<form class="grid" onsubmit="event.preventDefault()">
<input type="text" name="name" placeholder="Your Name" required />
<input type="email" name="email" placeholder="Email Address" required />
<input type="date" name="date" required />
<input type="time" name="time" required />
<textarea name="notes" placeholder="Describe the issue or request"></textarea>
<button type="submit">Request Appointment</button>
</form>
</section>

<section class="container" id="contact">
<hgroup>
<h2>Contact Us</h2>
<h3>Reach out with any questions</h3>
</hgroup>
<form class="grid" onsubmit="event.preventDefault()">
<input type="text" name="name" placeholder="Full Name" required />
<input type="email" name="email" placeholder="Email Address" required />
<input type="tel" name="phone" placeholder="Phone Number" />
<textarea name="message" placeholder="Your Message" required></textarea>
<input type="file" name="file" />
<button type="submit">Send Message</button>
</form>
<iframe title="Map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3271.537628257857!2d-86.1670142848011!3d35.24956578028324!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8863baf89972009f%3A0x994b2de5ad9f9e09!2s116%20Morris%20Ford%20Rd%2C%20Estill%20Springs%2C%20TN%2037330!5e0!3m2!1sen!2sus!4v1716841588573!5m2!1sen!2sus" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
</section>

<section class="container" id="reviews">
<hgroup>
<h2>Customer Reviews</h2>
<h3>What our customers are saying</h3>
</hgroup>
<form id="review-form" class="grid" onsubmit="event.preventDefault(); addReview();">
<input type="text" id="reviewer" placeholder="Your Name" required />
<textarea id="review-text" placeholder="Leave your review here" required></textarea>
<button type="submit">Submit Review</button>
</form>
<div id="review-list">
<div class="review-box"><strong>Emily R.:</strong> Quick turnaround and honest service. Highly recommend KDI!</div>
<div class="review-box"><strong>James P.:</strong> My laptop was dead — now it runs like new. Incredible!</div>
<div class="review-box"><strong>Linda S.:</strong> Very respectful, affordable, and thorough. Support local!</div>
</div>
</section>

<section class="container" id="veterans">
<hgroup>
<h2>Honoring Our Veterans</h2>
<h3>Supporting those who’ve served</h3>
</hgroup>
<p>At KDI Custom Builds, we are proud to donate a percentage of our profits to organizations that support veterans, including the <strong>Wounded Warrior Project</strong>. Your support helps make a difference. Please consider giving generously to veteran charities.</p>
<p><strong>To all our veterans: Thank you for your courage, your sacrifice, and your service.</strong></p>
<a href="https://support.woundedwarriorproject.org" target="_blank" role="button">Donate to Wounded Warriors</a>
</section>

<footer class="container">
<small><a href="#">Privacy Policy</a> • <a href="#">Terms & Conditions</a></small>
</footer>

<script>
function addReview() {
const name = document.getElementById('reviewer').value.trim();
const text = document.getElementById('review-text').value.trim();
if (name && text) {
const box = document.createElement('div');
box.className = 'review-box';
box.innerHTML = `<strong>${name}:</strong> ${text}`;
document.getElementById('review-list').prepend(box);
document.getElementById('review-form').reset();
}
}
</script>
</body>
</html>
