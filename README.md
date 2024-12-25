# Project Responsive Web Design using Bootstrap
## Date:25.12.24

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            font-family: Arial, sans-serif;
        }

        /* Hero Section Styling */
        .hero {
            background: linear-gradient(to bottom, #fff, #fce4ec);
            padding: 100px 20px;
            text-align: center;
        }
        .hero h1 {
            font-size: 3rem;
            font-weight: bold;
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            color: #555;
        }
        .hero .btn-primary {
            background-color: #ff4081;
            border: none;
            padding: 12px 24px;
            font-size: 1rem;
            border-radius: 25px;
        }

        /* Card Hover Effect */
        .card-hover {
            transition: transform 0.3s ease;
        }
        .card-hover:hover {
            transform: scale(1.05);
        }

        /* Footer Styling */
        footer {
            background-color: #f8f9fa;
            color: #6c757d;
            padding: 40px 0;
        }
        footer h6 {
            font-weight: bold;
            margin-bottom: 15px;
        }
        footer a {
            color: #6c757d;
            text-decoration: none;
            display: block;
            margin-bottom: 5px;
        }
        footer a:hover {
            text-decoration: underline;
        }
        footer .footer-bottom {
            border-top: 1px solid #dee2e6;
            padding-top: 20px;
            margin-top: 20px;
            font-size: 0.9rem;
        }

        /* Navbar Search */
        .navbar-search {
            max-width: 300px;
        }
    </style>
</head>
<body>

<!-- Navigation Bar -->
<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
        <a class="navbar-brand text-danger fw-bold" href="#">dribbble</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto">
                <li class="nav-item">
                    <a class="nav-link" href="#">Inspiration</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Find Work</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Learn Design</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Go Pro</a>
                </li>
            </ul>
            <form class="d-flex ms-3">
                <input class="form-control navbar-search" type="search" placeholder="Search" aria-label="Search">
            </form>
            <a class="btn btn-primary ms-3" href="#">Sign Up</a>
        </div>
    </div>
</nav>

<!-- Hero Section -->
<section class="hero">
    <div class="container">
        <h1>Discover the world’s top designers & creatives</h1>
        <p>Dribbble is the leading destination to find & showcase creative work and home to the world's best design professionals.</p>
        <a href="#explore" class="btn btn-primary">Sign up to continue</a>
    </div>
</section>

<!-- Explore Section -->
<section id="explore" class="py-5">
    <div class="container">
        <h2 class="text-center mb-4">Explore Creative Projects</h2>
        <div class="row">
            <div class="col-md-4 mb-4">
                <div class="card card-hover">
                    <img src="download.jpeg" class="card-img-top rounded" alt="Project 1">
                    <div class="card-body">
                        <h5 class="card-title">UI Design Collection</h5>
                        <p class="card-text">by Sarah Wilson</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-4">
                <div class="card card-hover">
                    <img src="download (1).jpeg" class="card-img-top rounded" alt="Project 2">
                    <div class="card-body">
                        <h5 class="card-title">Website Redesign</h5>
                        <p class="card-text">by John Smith</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-4">
                <div class="card card-hover">
                    <img src="OIP.jpeg" class="card-img-top rounded" alt="Project 3">
                    <div class="card-body">
                        <h5 class="card-title">Brand Identity</h5>
                        <p class="card-text">by Alex Johnson</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Community Section -->
<section id="community" class="py-5 bg-light">
    <div class="container">
        <h2 class="text-center mb-4">Join Our Creative Community</h2>
        <p class="text-center">Be part of a vibrant community of designers and creatives worldwide. Showcase your work, connect with others, and get inspired.</p>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="container">
        <div class="row">
            <div class="col-md-3 mb-4">
                <h6>FOR DESIGNERS</h6>
                <a href="#">Go Pro!</a>
                <a href="#">Explore design work</a>
                <a href="#">Design blog</a>
            </div>
            <div class="col-md-3 mb-4">
                <h6>HIRE DESIGNERS</h6>
                <a href="#">Post a job opening</a>
                <a href="#">Post a freelance project</a>
                <a href="#">Search for designers</a>
            </div>
            <div class="col-md-3 mb-4">
                <h6>COMPANY</h6>
                <a href="#">About</a>
                <a href="#">Careers</a>
                <a href="#">Support</a>
            </div>
            <div class="col-md-3 mb-4">
                <h6>DIRECTORIES</h6>
                <a href="#">Design jobs</a>
                <a href="#">Designers for hire</a>
                <a href="#">Tags</a>
            </div>
        </div>
        <div class="footer-bottom text-center">
            &copy; 2024 Dribbble. This is a clone created for demonstration purposes only.
        </div>
    </div>
</footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>


## OUTPUT:
![Screenshot 2024-12-25 114920](https://github.com/user-attachments/assets/f9dea0fb-53d3-4fd6-b42c-87c0eb27f159)
![Screenshot 2024-12-25 114939](https://github.com/user-attachments/assets/2ae69480-5b89-4657-8e4c-7e53002547a1)
![Screenshot 2024-12-25 114948](https://github.com/user-attachments/assets/43ab789e-2278-48ed-a37b-8416bdf9dd5f)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
