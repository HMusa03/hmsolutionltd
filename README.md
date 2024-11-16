<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HM Solutions Ltd</title>
  <style>
    /* General styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background-color: #f5f5f5;
      color: #333;
    }

    /* Header */
    header {
      background: linear-gradient(to right, green, red);
      color: white;
      padding: 10px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      display: flex;
      align-items: center;
      cursor: pointer;
    }

    .logo img {
      height: 40px;
      margin-right: 10px;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 15px;
    }

    nav ul li {
      position: relative;
    }

    nav ul li a {
      text-decoration: none;
      color: white;
      font-size: 16px;
      padding: 8px 12px;
      transition: background 0.3s;
    }

    nav ul li a:hover {
      background: rgba(255, 255, 255, 0.2);
      border-radius: 4px;
    }

    nav ul li ul {
      position: absolute;
      top: 40px;
      left: 0;
      background: white;
      color: #333;
      display: none;
      list-style: none;
      box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
    }

    nav ul li:hover ul {
      display: block;
    }

    nav ul li ul li a {
      color: #333;
      padding: 8px 12px;
      display: block;
    }

    nav ul li ul li a:hover {
      background: #ddd;
    }

    /* Slideshow */
    .slideshow {
      position: relative;
      max-width: 100%;
      height: 500px;
      overflow: hidden;
    }

    .slides {
      position: absolute;
      width: 100%;
      height: 100%;
      display: none;
    }

    .slides img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .active {
      display: block;
      animation: fade 1s;
    }

    @keyframes fade {
      from {
        opacity: 0.4;
      }
      to {
        opacity: 1;
      }
    }

    .caption {
      position: absolute;
      bottom: 20px;
      left: 20px;
      color: pink;
      font-size: 24px;
      font-weight: bold;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
    }

    /* Footer */
   /* Footer Styling */
   footer {
            background-color:green;
            color: white;
            padding: 2rem 0;
            margin-top: auto;
        }
    
        .footer-container {
            width: 80%;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2rem;
        }

        .footer-section h3 {
            color: #99bbff;
            margin-bottom: 1rem;
        }

        .footer-section ul {
            list-style: none;
            padding: 0;
        }

        .footer-section ul li {
            margin-bottom: 0.5rem;
        }

        .social-links {
            display: flex;
            gap: 1rem;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            font-size: 1.2em;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: #99bbff;
        }

        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #1a53ff;
            margin-top: 2rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                flex-direction: column;
                gap: 1rem;
                margin-top: 1rem;
            }

            .footer-container {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .social-links {
                justify-content: center;
            }
        }
  .prev, .next {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    padding: 10px;
    margin-top: -22px;
    color: green;
    font-weight: bold;
    font-size: 24px;
    transition: 0.6s ease;
    user-select: none;
    z-index: 1000;
  }

  .prev {
    left: 10px;
  }

  .next {
    right: 10px;
  }

  .prev:hover, .next:hover {
    background-color: rgba(0, 0, 0, 0.8);
    border-radius: 50%;
  }
  </style>
</head>

<body>
  <!-- Header -->
  <header>
    <div class="logo" onclick="location.reload()">
      <img src="IT_LOGO.png" alt="HM Solutions Logo">
      <span>HM Solutions Ltd</span>
    </div>
    <nav>
      <ul>
        <li><a href="#">About</a></li>
        <li>
          <a href="#">Services</a>
          <ul>
            <li><a href="#">IT Consulting</a></li>
            <li><a href="#">System Integration</a></li>
          </ul>
        </li>
        <li>
          <a href="#">Products</a>
          <ul>
            <li><a href="#">Hardware Solutions</a></li>
            <li><a href="#">Software Tools</a></li>
          </ul>
        </li>
        <li><a href="#">Articles</a></li>
      </ul>
    </nav>
  </header>

  <!-- Slideshow -->
  <div class="slideshow">
    <div class="slides active">
      <img src="HP EliteBook 840 G5 005.jpg" alt="Service 1">
      <div class="caption">We sell all kinds of London Used Computers. -  Laptops, All-In-One Computer, Chromebook etc. <br> To get one or more, <a href="https://wa.me/+2348053579779">Click</a></div>
    </div>
    <div class="slides">
      <img src="NIN04.png" alt="Service 2">
      <div class="caption">To Register and get your premium NIN Card, <a href="https://wa.me/+2348053579779">Click</a></div>
    </div>
    <div class="slides">
      <img src="SCHOOLS.png" alt="Service 3">
      <div class="caption">We are involved in all levels of FCT Schools online Application for Admission. Primary, Junior or Seniour Secondary. <br>To Apply for any Level of FCT Schools, <a href="https://wa.me/+2348053579779">Click</a></div>
    </div>
    <div class="slides">
      <img src="NAME.png" alt="Service 4">
      <div class="caption">We also do Newspaper Publication for Change of Name and the likes of it. <br> To get your <b>New Name</b> published, <a href="https://wa.me/+2348053579779">Click</a></div>
    </div>
    <div class="slides">
      <img src="AFFIDAVIT.png" alt="Service 5">
      <div class="caption">We do all kinds of eAffidavits. i.e. Statutory Declaration of Age, Marriage Certificate, Change of Name, Reconciliation of Name, <br>Correction of Name, Loss of Particulars etc.<br> To get you an Affidavit, <a href="https://wa.me/+2348053579779">Click</a></div>
    </div>
    <div class="slides">
      <img src="GRAPHIC.png" alt="Service 6">
      <div class="caption">We are also involved in all kinds of Graphic Designs. i.e. ID Card, Wedding Invitation, Jotter, Calender, Photo-Album etc.<br> To get the best Design, <a href="https://wa.me/+2348053579779">Click</a></div>
    </div>
    <div class="slides">
      <img src="CLICK02.png" alt="Service 6">
      <div class="caption"><h3></h3><a href="https://wa.me/+2348053579779">Click me</a></div>
    </div>

      <!-- Add your other slides here -->
      
      <!-- Navigation Buttons -->
      <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
      <a class="next" onclick="changeSlide(1)">&#10095;</a>
    </div>
    
  </div>

  <!-- Footer -->
  <footer>
    <div class="footer-container">
      <div class="footer-section">
          <h3>Contact Us</h3>
          <p>Email: info@legendspikers.com</p>
          <p>Phone: +234 123 456 7890</p>
          <p>Address: Kubwa, Abuja</p>
      </div>
      <div class="footer-section">
          <h3>Quick Links</h3>
          <ul>
              <li><a href="teams.html">Our Teams</a></li>
              <li><a href="schedule.html">Match Schedule</a></li>
              <li><a href="gallery.html">Photo Gallery</a></li>
          </ul>
      </div>
      <div class="footer-section">
          <h3>Follow Us</h3>
          <div class="social-links">
              <a href="https://web.facebook.com/HMTelecoms" target="_blank" title="Facebook">
                  <i class="fab fa-facebook"></i> Facebook
              </a>
              <a href="https://x.com/HMusa3" target="_blank" title="Twitter">
                  <i class="fab fa-twitter"></i> Twitter
              </a>
              <a href="https://www.instagram.com/hmtelecoms0/" target="_blank" title="Instagram">
                  <i class="fab fa-instagram"></i> Instagram
              <a href="https://www.linkedin.com/in/hussaini-musa-68614283/" target="_blank" title="LinkedIn">
                  <i class="fab fa-instagram"></i> LinkedIn
              <a href="https://wa.me/+2348053579779" target="_blank" title="WhatsApp">
                  <i class="fab fa-instagram"></i> WhatsApp
              </a>
          </div>
      </div>
  </div>
  <div class="copyright">
      <p>&copy; 2024 HM Solutions Limited. All rights reserved.</p>

  <!-- JavaScript -->
  <script>
   let slideIndex = 0;
let slideInterval;

function showSlides() {
  const slides = document.querySelectorAll('.slides');
  slides.forEach((slide, index) => {
    slide.style.display = 'none';
    slide.classList.remove('active');
  });
  slideIndex++;
  if (slideIndex > slides.length) slideIndex = 1;
  slides[slideIndex - 1].style.display = 'block';
  slides[slideIndex - 1].classList.add('active');
}

function changeSlide(n) {
  const slides = document.querySelectorAll('.slides');
  slides[slideIndex - 1].style.display = 'none';
  slideIndex += n;
  if (slideIndex > slides.length) slideIndex = 1;
  if (slideIndex < 1) slideIndex = slides.length;
  slides[slideIndex - 1].style.display = 'block';
  slides[slideIndex - 1].classList.add('active');
}

function startSlideshow() {
  slideInterval = setInterval(() => changeSlide(1), 5000);
}

function stopSlideshow() {
  clearInterval(slideInterval);
}

// Initialize the slideshow
showSlides();
startSlideshow();

// Add event listeners for hover
const slideshow = document.querySelector('.slideshow');
slideshow.addEventListener('mouseenter', stopSlideshow);
slideshow.addEventListener('mouseleave', startSlideshow);

  </script>
</body>

</html>
