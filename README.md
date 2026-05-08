CSE-project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Damodar Educational Institutes</title>
    <!-- Internal CSS starts here -->
    <style>
        :root {
            --main-blue: #2362c7;
            --light-blue: #e3ecfa;
            --button-blue: #357ae8;
            --white: #fff;
            --gray: #f5f5f5;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: var(--gray);
            color: #222;
        }

        /* Header and Navigation */
        header {
            background: var(--main-blue);
            color: var(--white);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .container {
            max-width: 1000px;
            margin: auto;
            padding: 0 16px;
        }
        .header-flex {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        .school-name {
            font-size: 2rem;
            font-weight: bold;
            letter-spacing: 2px;
        }
        nav {
            display: flex;
            gap: 18px;
        }
        nav a {
            color: var(--white);
            text-decoration: none;
            font-size: 1.1rem;
            transition: color 0.2s;
            padding: 4px 8px;
            border-radius: 4px;
        }
        nav a:hover {
            background: var(--button-blue);
        }

        /* Responsive Navigation */
        @media (max-width: 600px) {
            .header-flex {
                flex-direction: column;
                align-items: flex-start;
                gap: 12px;
            }
            nav {
                width: 100%;
                flex-wrap: wrap;
                gap: 8px;
            }
        }

        /* Sections */
        section {
            background: var(--white);
            margin: 24px 0;
            padding: 32px 18px 28px 18px;
            border-radius: 10px;
            box-shadow: 0 3px 10px rgba(35,98,199,0.07);
        }
        @media (max-width: 600px) {
            section {
                padding: 22px 7px 15px 7px;
                margin: 16px 0;
            }
        }

        /* Home Banner */
        .home-banner {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 18px;
        }
        .welcome-msg {
            flex: 1 1 260px;
        }
        .banner-img {
            flex: 1 1 180px;
            min-width: 180px;
            text-align: right;
        }
        .banner-img img {
            max-width: 220px;
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 3px 8px #00226e20;
        }
        @media (max-width: 800px) {
            .home-banner {
                flex-direction: column;
                align-items: flex-start;
                gap: 28px;
            }
            .banner-img {
                text-align: left;
            }
        }

        /* Buttons */
        .blue-btn {
            background: var(--main-blue);
            color: var(--white);
            border: none;
            padding: 10px 24px;
            border-radius: 5px;
            font-size: 1.1em;
            cursor: pointer;
            transition: background 0.2s;
            margin-top: 18px;
        }
        .blue-btn:hover {
            background: var(--button-blue);
        }

        /* About Section */
        .about-text {
            font-size: 1.15em;
            line-height: 1.7;
        }

        /* Courses Section */
        .courses-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
            gap: 21px;
        }
        .course-card {
            background: var(--light-blue);
            border-radius: 8px;
            box-shadow: 0 2px 8px #2362c730;
            padding: 20px 14px;
            text-align: center;
        }
        .course-title {
            font-size: 1.16em;
            font-weight: bold;
            color: var(--main-blue);
            margin-bottom: 8px;
        }

        /* Contact Section */
        .contact-form {
            max-width: 420px;
            margin: auto;
            display: flex;
            flex-direction: column;
            gap: 14px;
        }

        .contact-label {
            font-weight: 500;
        }
        .contact-input, .contact-textarea {
            padding: 9px 10px;
            font-size: 1em;
            border: 1px solid #bdd2ef;
            border-radius: 5px;
            outline: none;
            resize: none;
            transition: border-color 0.2s;
        }
        .contact-input:focus, .contact-textarea:focus {
            border-color: var(--main-blue);
        }
        .contact-error {
            color: #df2222;
            font-size: 0.98em;
            min-height: 18px;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 16px 0;
            background: var(--main-blue);
            color: var(--white);
            font-size: 1em;
            border-top-left-radius: 15px;
            border-top-right-radius: 15px;
            margin-top: 35px;
        }
    </style>
</head>
<body>
    <!-- Header with School Name and Navigation Menu -->
    <header>
        <div class="container header-flex">
            <div class="school-name">Damodar Educational Institutes</div>
            <nav>
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#courses">Courses</a>
                <a href="#contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="container">
        <!-- Home Section -->
        <section id="home">
            <div class="home-banner">
                <div class="welcome-msg">
                    <h1>Welcome to Damodar Educational Institutes!</h1>
                    <p>Your path to knowledge, creativity, and growth begins here.</p>
                    <button class="blue-btn" id="welcomeBtn">Click Me!</button>
                </div>
                <div class="banner-img">
                    <!-- Banner Image (royalty free simple illustration from unsplash) -->
                    <img src="https://images.unsplash.com/photo-1503676382389-4809596d5290?auto=format&fit=crop&w=600&q=80" alt="School Banner">
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about">
            <h2>About Us</h2>
            <p class="about-text">
                Damodar Educational Institutes has been dedicated to providing quality education since 1995.  
                We focus on inspiring curiosity, fostering creativity, and empowering students for a successful future.  
                Our experienced faculty and state-of-the-art campus ensure every child gets the best start in life.
            </p>
        </section>

        <!-- Courses Section -->
        <section id="courses">
            <h2>Our Courses</h2>
            <div class="courses-list">
                <div class="course-card">
                    <div class="course-title">Mathematics</div>
                    <div>Explore the wonders of numbers, logic, and problem-solving from basic arithmetic to advanced calculus.</div>
                </div>
                <div class="course-card">
                    <div class="course-title">Science</div>
                    <div>Dive into Biology, Physics, and Chemistry through interactive labs, experiments, and practical learning.</div>
                </div>
                <div class="course-card">
                    <div class="course-title">Computer Science</div>
                    <div>Learn essential digital skills, programming, robotics, and the latest in technology for all ages.</div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact">
            <h2>Contact Us</h2>
            <form class="contact-form" id="contactForm" autocomplete="off">
                <div>
                    <label class="contact-label" for="name">Name</label><br>
                    <input class="contact-input" type="text" id="name" name="name">
                    <div class="contact-error" id="nameError"></div>
                </div>
                <div>
                    <label class="contact-label" for="email">Email</label><br>
                    <input class="contact-input" type="email" id="email" name="email">
                    <div class="contact-error" id="emailError"></div>
                </div>
                <div>
                    <label class="contact-label" for="message">Message</label><br>
                    <textarea class="contact-textarea" id="message" name="message" rows="4"></textarea>
                    <div class="contact-error" id="messageError"></div>
                </div>
                <button type="submit" class="blue-btn">Send Message</button>
            </form>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        &copy; 2026 Damodar Educational Institutes. All rights reserved.
    </footer>

    <!-- JavaScript for interactivity and validation -->
    <script>
        // --- Navigation Smooth Scroll for better UX (optional) ---
        // All internal links will scroll smoothly
        document.querySelectorAll('nav a').forEach(link => {
            link.addEventListener('click', function(e) {
                const targetId = this.getAttribute('href');
                if (targetId.startsWith('#')) {
                    const section = document.querySelector(targetId);
                    if (section) {
                        e.preventDefault();
                        section.scrollIntoView({ behavior: 'smooth' });
                    }
                }
            });
        });

        //
        // Contact Form Validation
        //
        document.getElementById('contactForm').addEventListener('submit', function(event) {
            // Prevent form from submitting
            event.preventDefault();

            // Get form values
            const name = document.getElementById('name').value.trim();
            const email = document.getElementById('email').value.trim();
            const message = document.getElementById('message').value.trim();

            // Error fields
            let hasError = false;

            // Clear previous errors
            document.getElementById('nameError').textContent = '';
            document.getElementById('emailError').textContent = '';
            document.getElementById('messageError').textContent = '';

            // Name validation
            if (name === '') {
                document.getElementById('nameError').textContent = 'Please enter your name.';
                hasError = true;
            }

            // Email validation (simple regex)
            const emailPattern = /^[^@ \t\r\n]+@[^@ \t\r\n]+\.[a-z]{2,}$/i;
            if (email === '') {
                document.getElementById('emailError').textContent = 'Please enter your email.';
                hasError = true;
            } else if (!emailPattern.test(email)) {
                document.getElementById('emailError').textContent = 'Please enter a valid email address.';
                hasError = true;
            }

            // Message validation
            if (message === '') {
                document.getElementById('messageError').textContent = 'Please enter your message.';
                hasError = true;
            }

            // If valid, show success alert
            if (!hasError) {
                alert('Thank you! Your message has been sent.');
                // Optionally, reset the form
                document.getElementById('contactForm').reset();
            }
        });

        //
        // Interactive Feature
        //
        // When "Click Me!" button is pressed, show a welcome message
        document.getElementById('welcomeBtn').addEventListener('click', function() {
            alert('Welcome to our school!');
        });

        // END OF SCRIPT
    </script>
</body>
</html>
