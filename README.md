<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My First Website</title>

    <!-- Link to Bootstrap (for Cards and Grid Layout) -->
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">

    <!-- Link to Font Awesome (for Social Media Icons) -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" rel="stylesheet">

    <style>
        /* Global Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background-color: #f9f9f9;
            margin-top: 60px; /* To make space for the fixed navbar */
        }

        h1, h2 {
            color: #333;
        }

        /* Navbar Styles */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: #333;
            color: white;
            padding: 5px 4%;
            margin: 6px 8px;
            z-index: 500;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: space-around;
            align-items: center;
        }

        nav ul li {
            padding: 10px 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            padding: 10px;
            display: block;
            transition: background-color 0.3s;
        }

        nav ul li a:hover {
            background-color: #555;
        }

        /* Mobile-Friendly Styles */
        .menu-toggle {
            display: none;
            background: #333;
            color: white;
            border: none;
            padding: 10px;
            font-size: 20px;
            cursor: pointer;
        }

        /* Responsive Layout: Mobile View */
        @media (max-width: 768px) {
            nav ul {
                display: none;
                flex-direction: column;
                width: 100%;
                text-align: center;
            }

            nav ul li {
                width: 100%;
            }

            .menu-toggle {
                display: block;
            }

            nav ul.show {
                display: flex;
            }

            nav ul li a {
                padding: 15px;
                background-color: #444;
                border-top: 1px solid #fff;
            }

            nav ul li a:hover {
                background-color: #666;
            }
        }

        /* Main Content Styles */
        main {
            padding: 20px;
            margin-top: 20px; /* Avoid content being covered by navbar */
        }

        section {
            margin-bottom: 40px;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #333;
            color: white;
        }

        footer .social-icons {
            margin-top: 10px;
        }

        footer .social-icons a {
            color: white;
            margin: 0 10px;
            font-size: 24px;
            text-decoration: none;
        }

        footer .social-icons a:hover {
            color: #ddd;
        }
    </style>
</head>
<body>

    <!-- Navbar Section -->
    <nav>
        <!-- Hamburger icon for mobile -->
        <button class="menu-toggle" id="menu-toggle">☰</button>

        <!-- Navbar Links -->
        <ul id="nav-list">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Main Content -->
    <main>
        <section id="home">
            <h1>Home</h1>
            <p>Welcome to Cups & Coffee
                There's nothing quite like the warm embrace of a freshly brewed cup of coffee. Whether you're a seasoned coffee enthusiast or someone just discovering the magic of the bean, you've come to the right place. At Cups & Coffee, we celebrate the rich flavors, aromas, and culture that make coffee more than just a drink—it's a lifestyle.
                
                t.</p>
                

        <section id="contact">
            <h2>Contact</h2>
            <p>Our Location
                Come visit us and experience the magic of freshly brewed coffee! We’re located in the heart of the city, and our doors are always open to coffee enthusiasts, casual drinkers, and newcomers alike.
                <br>
                <h2></h2>Address</h2>
                <br>
                <h2>Cups & Coffee</h2>
                123 Brew Street<br>
                Coffee City, CC 98765<br><br>
                
               <h2>Our Hours</h2><br>
                Monday - Friday: 7:00 AM - 7:00 PM<br>
                Saturday: 8:00 AM - 6:00 PM<br>
                Sunday: Closed<br>
                Contact Details<br>
                Phone: +1 (123) 456-7890<br>
                Email: info@cupsandcoffee.com<br<
                </p>
        </section>

        <!-- Bootstrap Cards Section -->
        <section id="cards" class="container">
            <h2>My Projects</h2>
            <div class="row">
                <!-- Card 1 -->
                <div class="col-md-4">
                    <div class="card">
                        <img src="https://cdn.pixabay.com/photo/2015/05/31/10/54/coffee-791045_640.jpg" class="card-img-top" alt="Project 1">
                        <div class="card-body">
                            <h5 class="card-title">Project 1</h5>
                            <p class="card-text">"Coffee is a hug in a mug."</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="col-md-4">
                    <div class="card">
                        <img src="https://cdn.pixabay.com/photo/2016/11/21/13/09/caffeine-1845314_640.jpg" class="card-img-top" alt="Project 2">
                        <div class="card-body">
                            <h5 class="card-title">Project 2</h5>
                            <p class="card-text">"From Bean to Cup, With Love."
                            </p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="col-md-4">
                    <div class="card">
                        <img src="https://cdn.pixabay.com/photo/2017/10/13/15/29/coffee-2847957_640.jpg" class="card-img-top" alt="Project 3">
                        <div class="card-body">
                            <h5 class="card-title">Project 3</h5>
                            <p class="card-text">"The Art of Coffee, Perfected."</p>
                            <a href="#" class="btn btn-primary">View Project</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <p><h2>Our Story</h2>
            At Cups & Coffee, we're passionate about creating the perfect cup of coffee. Our journey began with a simple idea: to bring people together over a cup of expertly crafted coffee. Whether it's your first morning brew or your afternoon pick-me-up, we believe that every cup has a story to tell. With a focus on quality, sustainability, and community, we're here to offer more than just coffee—we’re serving experiences.
            
            </p>
</section>

<section id="about">
    <h2>About</h2>
    <p>At Cups & Coffee, we offer more than just great coffee—we offer an experience. Whether you're stopping by for your daily brew or enjoying a leisurely afternoon with friends, our space is designed to provide a warm, welcoming atmosphere. Our offerings include:
<br>
        Freshly Roasted Coffee: We source our beans from some of the best coffee-growing regions around the world, and roast them to perfection to highlight their unique flavors.
        Specialty Drinks: From rich espressos to creamy lattes and bold pour-overs, our menu offers a variety of drinks to suit every taste.
        Workshops & Events: We’re passionate about sharing our knowledge. Join us for coffee workshops, tastings, and events that explore the world of coffee, from bean to cup.
        Coffee Subscriptions: Get your favorite coffee delivered to your doorstep! Our subscription service brings the best of Cups & Coffee right to you, so you can enjoy fresh, expertly roasted beans whenever you want.
        </p>
</section>

    </main>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 My First Website. All rights reserved.</p>

        <!-- Social Media Icons -->
        <div class="social-icons">
            <a href="https://facebook.com" target="_blank" class="fab fa-facebook-f"></a>
            <a href="https://twitter.com" target="_blank" class="fab fa-twitter"></a>
            <a href="https://linkedin.com" target="_blank" class="fab fa-linkedin-in"></a>
            <a href="https://github.com" target="_blank" class="fab fa-github"></a>
        </div>
    </footer>

    <!-- Bootstrap & FontAwesome JS (optional) -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.3/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

    <!-- JavaScript for Toggle Menu (Mobile) -->
    <script>
        // Selecting elements
        const menuToggle = document.getElementById('menu-toggle');
        const navList = document.getElementById('nav-list');

        // Event listener to toggle the navbar on small screens
        menuToggle.addEventListener('click', () => {
            navList.classList.toggle('show'); // This adds/removes the 'show' class
        });
    </script>

</body>
</html>
