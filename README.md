# Receipts-Generator

# Receipt Generator (Web + Image Export)

This project is a simple **responsive receipt generator** for PC and Mobile.  
It allows you to input **Name, Amount, Email, Phone**, and automatically converts the amount into words.  
Your **signature image** and the **JIS College of Engineering logo watermark** are automatically added.  

---

## ✨ Features
- Responsive **PC + Mobile compatible** design (auto adjusts layout).
- Automatically converts **numbers to words**.
- Includes **signature block** (customizable).
- Adds a **transparent watermark logo** in the background.
- Generates a **downloadable PNG image** of the receipt (instead of PDF).

---

## 📂 Project Structure

---

## ⚙️ Setup Instructions

1. Clone or download the project.
2. Place your own **signature.png** and **watermark.png** inside the project folder.
3. Open `index.html` in any modern browser.

---

## 🖼️ How to Generate Receipt Image

1. Fill in the form (Name, Amount, Email, Phone).  
2. Click **Generate Receipt**.  
3. A styled receipt with watermark + signature will appear.  
4. Click **Download as Image** to save it as PNG.

---

## 📱 Responsive Design
- On **PC**: Receipt is centered and uses full width.  
- On **Mobile**: Layout adjusts and content stays readable.  
- Signature auto-scales to fit small screens.

---

## 🖊️ Signature Section
```html
<div class="signature">
  <p>Signature of Receiver:</p>
  <img src="signature.png" alt="Signature">
</div>

.signature {
  margin-top: 20px;
  text-align: left;
}

.signature img {
  display: block;
  margin-top: 5px;
  max-width: 40%; /* responsive scaling */
  height: auto;
}

<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>
