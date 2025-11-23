# NAME: DEEPIKA G
# REG.NO: 212224040060
# Ex.08 Design of Interactive Image Gallery
## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>INTERACTIVE GALLERY</title>
  <link href="https://fonts.googleapis.com/css2?family=Exo+2:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, #0f2027, #203a43, #2c5364);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: white;
    }

    .container {
      text-align: center;
      padding: 40px 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    h1 {
      font-size: 2.5rem;
      color: #00f5ff;
      text-shadow: 0 0 15px #00f5ff, 0 0 25px #00f5ff;
      margin-bottom: 40px;
      font-family: 'Exo 2', sans-serif;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(4, 1fr); /* Fixed 4 columns per row */
      gap: 20px;
    }

    .card {
      background-color: #1e2f3f;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 0 15px rgba(0, 255, 255, 0.2);
      transition: transform 0.3s ease;
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      display: block;
    }

    .card:hover {
      transform: scale(1.05);
      box-shadow: 0 0 25px rgba(0, 255, 255, 0.6);
    }

    .signature {
      margin-top: 60px;
      padding: 20px;
      text-align: center;
      font-size: 1.6rem;
      font-family: 'Exo 2', sans-serif;
      background: linear-gradient(90deg, #ff0080, #7928ca, #00ffff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-size: 200% auto;
      animation: colorChange 3s ease-in-out infinite;
      text-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
    }

    @keyframes colorChange {
      0% {
        background-position: 0% 50%;
      }
      100% {
        background-position: 100% 50%;
      }
    }

    /* Responsive for small screens (phones/tablets) */
    @media (max-width: 992px) {
      .gallery {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 600px) {
      .gallery {
        grid-template-columns: 1fr;
      }
    }

    /* Modal styles */
    .modal {
      display: none;
      position: fixed;
      z-index: 1;
      padding-top: 100px;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgb(0,0,0);
      background-color: rgba(0,0,0,0.9);
    }

    .modal-content {
      margin: auto;
      display: block;
      width: 80%;
      max-width: 700px;
    }

    .close {
      position: absolute;
      top: 15px;
      right: 35px;
      color: #f1f1f1;
      font-size: 40px;
      font-weight: bold;
      transition: 0.3s;
    }

    .close:hover,
    .close:focus {
      color: #bbb;
      text-decoration: none;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>INTERACTIVE ARTISTIC GALLERY</h1>
    <div class="gallery">
      <div class="card"><img src="c:\Users\admin\Downloads\download.jpg" alt="Image 1" /></div>
      <div class="card"><img src="c:\Users\admin\Downloads\Human Creativity vs_ Technology.jpg" alt="Image 2" /></div>
      <div class="card"><img src="c:\Users\admin\Downloads\a.jpg" alt="Image 3" /></div>
      <div class="card"><img src="c:\Users\admin\Downloads\WhatsApp Image 2025-10-14 at 5.20.40 AM.jpeg" alt="Image 4" /></div>
      <div class="card"><img src="c:\Users\admin\Pictures\Screenshots\Screenshot 2025-11-13 102501.png" alt="Image 5" /></div>
      <div class="card"><img src="c:\Users\admin\Downloads\Unleash Your Creativity & Self-Discovery with Mindful Moments Art Therapy Cards.jpg" alt="Image 6" /></div>
    </div>

    <div class="signature">
      <p>✨ DONE BY <strong> DEEPIKA G </strong> (212224040060) ✨</p>
    </div>
  </div>

  <!-- Modal popup for image enlarge -->
  <div id="modal" class="modal">
    <span class="close">&times;</span>
    <img class="modal-content" id="modalImage">
  </div>

  <!-- JavaScript for interaction -->
  <script>
    const modal = document.getElementById("modal");
    const modalImg = document.getElementById("modalImage");
    const closeBtn = document.getElementsByClassName("close")[0];

    document.querySelectorAll('.card img').forEach(img => {
      img.addEventListener('click', () => {
        modal.style.display = "block";
        modalImg.src = img.src;
      });
    });

    closeBtn.onclick = function() {
      modal.style.display = "none";
    };

    window.onclick = function(event) {
      if (event.target == modal) {
        modal.style.display = "none";
      }
    };
  </script>
</body>
</html>
```

## OUTPUT

<img width="1918" height="1109" alt="image" src="https://github.com/user-attachments/assets/dceeef11-ed78-4ef8-9905-a593ad9c67ba" />

<img width="1919" height="1135" alt="image" src="https://github.com/user-attachments/assets/8a37c758-5ffb-4e1e-a6f4-435617bed2ac" />

<img width="1919" height="1135" alt="image" src="https://github.com/user-attachments/assets/b4b025b8-2173-4d51-89a2-226eceb29e5f" />

<img width="1919" height="1139" alt="image" src="https://github.com/user-attachments/assets/b4d6fecb-e39f-4ca2-8fc6-68ff40359eef" />

<img width="1919" height="1141" alt="image" src="https://github.com/user-attachments/assets/2cb08f6d-1dd7-4177-b6c9-702088905965" />

<img width="1919" height="1136" alt="image" src="https://github.com/user-attachments/assets/fd2f3e5a-2078-4c47-a679-d46d2ea6a25b" />

<img width="1919" height="1131" alt="image" src="https://github.com/user-attachments/assets/6e993859-97e7-4bf8-9928-7f41ae7275bc" />

## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
