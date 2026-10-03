<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Jomar John M. Paquibo | Portfolio</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #07111f;
            color: #ffffff;
            line-height: 1.6;
        }

        /* =========================
           NAVBAR
        ========================= */

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 70px;
            background: #081525;
            border-bottom: 1px solid rgba(0, 212, 255, 0.15);
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0 8%;
            z-index: 1000;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
            color: #00d9ff;
            letter-spacing: 1px;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 30px;
        }

        nav ul li a {
            text-decoration: none;
            color: #ffffff;
            font-size: 15px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: #00d9ff;
        }

        /* =========================
           GENERAL SECTION
        ========================= */

        section {
            min-height: 100vh;
            padding: 110px 8% 70px;
        }

        .section-title {
            text-align: center;
            font-size: 38px;
            margin-bottom: 50px;
        }

        .section-title span {
            color: #00d9ff;
        }

        /* =========================
           HOME
        ========================= */

        #home {
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            min-height: 100vh;
        }

        .home-content {
            max-width: 800px;
            width: 100%;
        }

        .profile-wrapper {
            width: 140px;
            height: 140px;
            margin: 0 auto 25px;
            padding: 0;
            background: transparent;
            overflow: hidden;
            box-shadow: none;
            border-radius: 0;
        }

        .profile-image {
            width: 100%;
            height: 100%;
            display: block;
            object-fit: cover;
            object-position: center;
            border-radius: 0;
        }

        .home-content h1 {
            font-size: 48px;
            margin-bottom: 10px;
        }

        .home-content h1 span {
            color: #00d9ff;
        }

        .home-content h2 {
            font-size: 24px;
            font-weight: normal;
            color: #b9c8d8;
            margin-bottom: 20px;
        }

        .home-content p {
            max-width: 650px;
            margin: auto;
            color: #aebdce;
            font-size: 17px;
        }

        /* =========================
           ABOUT
        ========================= */

        #about {
            background: #081525;
        }

        .about-container {
            max-width: 900px;
            margin: auto;
            text-align: center;
        }

        .about-container p {
            color: #b9c8d8;
            font-size: 17px;
            margin-bottom: 20px;
        }

        /* =========================
           SKILLS
        ========================= */

        .skills-container {
            max-width: 1000px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .skill-card {
            background: #0b1b2d;
            border: 1px solid rgba(0, 217, 255, 0.2);
            border-radius: 12px;
            padding: 30px 20px;
            text-align: center;
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-5px);
            border-color: #00d9ff;
        }

        .skill-card h3 {
            color: #00d9ff;
            margin-bottom: 10px;
            font-size: 20px;
        }

        .skill-card p {
            color: #aebdce;
            font-size: 15px;
        }

        /* =========================
           PROJECTS
        ========================= */

        #projects {
            background: #081525;
        }

        .projects-container {
            max-width: 1100px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .project-card {
            background: #0b1b2d;
            border: 1px solid rgba(0, 217, 255, 0.2);
            border-radius: 14px;
            padding: 30px;
            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-6px);
            border-color: #00d9ff;
        }

        .project-number {
            color: #00d9ff;
            font-size: 13px;
            font-weight: bold;
            margin-bottom: 15px;
            letter-spacing: 1px;
        }

        .project-card h3 {
            font-size: 25px;
            margin-bottom: 15px;
        }

        .project-card p {
            color: #aebdce;
            font-size: 15px;
            line-height: 1.7;
        }

        /* =========================
           CONTACT
        ========================= */

        .contact-container {
            max-width: 850px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 25px;
        }

        .contact-card {
            background: #0b1b2d;
            border: 1px solid rgba(0, 217, 255, 0.2);
            border-radius: 14px;
            padding: 35px 25px;
            text-align: center;
            transition: 0.3s;
        }

        .contact-card:hover {
            transform: translateY(-5px);
            border-color: #00d9ff;
        }

        .contact-icon {
            font-size: 35px;
            margin-bottom: 15px;
        }

        .contact-card h3 {
            color: #00d9ff;
            margin-bottom: 10px;
        }

        .contact-card a {
            color: #ffffff;
            text-decoration: none;
            word-break: break-word;
        }

        .contact-card a:hover {
            color: #00d9ff;
        }

        /* =========================
           FOOTER
        ========================= */

        footer {
            background: #050d18;
            text-align: center;
            padding: 25px 15px;
            color: #8090a3;
            font-size: 14px;
        }

        /* =========================
           RESPONSIVE
        ========================= */

        @media (max-width: 900px) {

            nav {
                padding: 0 5%;
            }

            nav ul {
                gap: 18px;
            }

            .skills-container,
            .projects-container {
                grid-template-columns: repeat(2, 1fr);
            }

            .home-content h1 {
                font-size: 40px;
            }
        }

        @media (max-width: 650px) {

            nav {
                height: auto;
                min-height: 70px;
                padding: 15px 5%;
                flex-direction: column;
                gap: 10px;
            }

            nav ul {
                gap: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }

            section {
                padding: 130px 5% 60px;
            }

            .section-title {
                font-size: 32px;
            }

            .skills-container,
            .projects-container,
            .contact-container {
                grid-template-columns: 1fr;
            }

            .home-content h1 {
                font-size: 34px;
            }

            .home-content h2 {
                font-size: 20px;
            }

            .home-content p {
                font-size: 15px;
            }
        }

        @media (max-width: 450px) {

            .profile-wrapper {
                width: 110px;
                height: 110px;
            }

            .home-content h1 {
                font-size: 30px;
            }

            .home-content h2 {
                font-size: 18px;
            }

            nav ul {
                gap: 10px;
            }

            nav ul li a {
                font-size: 13px;
            }
        }

    </style>
</head>

<body>

    <!-- =========================
         NAVIGATION
    ========================== -->

    <nav>

        <div class="logo">
            JOMAR.DEV
        </div>

        <ul>
            <li>
                <a href="#home">Home</a>
            </li>

            <li>
                <a href="#about">About</a>
            </li>

            <li>
                <a href="#skills">Skills</a>
            </li>

            <li>
                <a href="#projects">Projects</a>
            </li>

            <li>
                <a href="#contact">Contact</a>
            </li>
        </ul>

    </nav>


    <!-- =========================
         HOME
    ========================== -->

    <section id="home">

        <div class="home-content">

            <div class="profile-wrapper">
                <img
                    src="assets/profile.png"
                    alt="Jomar John M. Paquibo"
                    class="profile-image"
                >
            </div>

            <h1>
                Hi, I'm
                <span>Jomar John M. Paquibo</span>
            </h1>

            <h2>
                Web Developer / IT Student
            </h2>

            <p>
                I am passionate about creating modern,
                responsive, and user-friendly web applications
                while continuously improving my programming
                and technology skills.
            </p>

        </div>

    </section>


    <!-- =========================
         ABOUT
    ========================== -->

    <section id="about">

        <h2 class="section-title">
            About <span>Me</span>
        </h2>

        <div class="about-container">

            <p>
                I am Jomar John M. Paquibo, an aspiring web
                developer and IT professional interested in
                building useful and modern digital solutions.
            </p>

            <p>
                I enjoy developing web applications, working
                with databases, creating responsive interfaces,
                and learning new technologies.
            </p>

            <p>
                My goal is to continue improving my technical
                skills and create applications that provide
                practical solutions for users.
            </p>

        </div>

    </section>


    <!-- =========================
         SKILLS
    ========================== -->

    <section id="skills">

        <h2 class="section-title">
            My <span>Skills</span>
        </h2>

        <div class="skills-container">

            <div class="skill-card">

                <h3>
                    HTML
                </h3>

                <p>
                    Building structured and semantic
                    web pages.
                </p>

            </div>


            <div class="skill-card">

                <h3>
                    CSS
                </h3>

                <p>
                    Creating responsive layouts and
                    modern user interfaces.
                </p>

            </div>


            <div class="skill-card">

                <h3>
                    JavaScript
                </h3>

                <p>
                    Adding interactive functionality
                    and dynamic web features.
                </p>

            </div>


            <div class="skill-card">

                <h3>
                    Database
                </h3>

                <p>
                    Working with data storage,
                    authentication, and backend systems.
                </p>

            </div>


            <div class="skill-card">

                <h3>
                    GitHub
                </h3>

                <p>
                    Managing source code and
                    development projects.
                </p>

            </div>


            <div class="skill-card">

                <h3>
                    Responsive Design
                </h3>

                <p>
                    Designing websites that work
                    across different screen sizes.
                </p>

            </div>

        </div>

    </section>


    <!-- =========================
         PROJECTS
    ========================== -->

    <section id="projects">

        <h2 class="section-title">
            My <span>Projects</span>
        </h2>

        <div class="projects-container">

            <!-- PROJECT 1 -->

            <div class="project-card">

                <div class="project-number">
                    PROJECT 01
                </div>

                <h3>
                    ERecPass
                </h3>

                <p>
                    A hospital portal designed for managing
                    patient information, appointments,
                    medical records, laboratory results,
                    medications, announcements, emergency
                    features, QR patient identification,
                    staff functions, and administrative
                    management.
                </p>

            </div>


            <!-- PROJECT 2 -->

            <div class="project-card">

                <div class="project-number">
                    PROJECT 02
                </div>

                <h3>
                    QR Patient Scanner
                </h3>

                <p>
                    A QR-based patient identification system
                    designed to scan patient QR codes and
                    access patient-related laboratory results
                    and information.
                </p>

            </div>


            <!-- PROJECT 3 -->

            <div class="project-card">

                <div class="project-number">
                    PROJECT 03
                </div>

                <h3>
                    Web Application
                </h3>

                <p>
                    A responsive web application focused on
                    clean interface design, usability, and
                    interactive functionality.
                </p>

            </div>

        </div>

    </section>


    <!-- =========================
         CONTACT
    ========================== -->

    <section id="contact">

        <h2 class="section-title">
            Contact <span>Me</span>
        </h2>

        <div class="contact-container">

            <!-- EMAIL -->

            <div class="contact-card">

                <div class="contact-icon">
                    ✉️
                </div>

                <h3>
                    Email
                </h3>

                <a href="mailto:jomarjohnpaquibo7@gmail.com">
                    jomarjohnpaquibo7@gmail.com
                </a>

            </div>


            <!-- PHONE -->

            <div class="contact-card">

                <div class="contact-icon">
                    📱
                </div>

                <h3>
                    Phone
                </h3>

                <a href="tel:09927609792">
                    09927609792
                </a>

            </div>

        </div>

    </section>


    <!-- =========================
         FOOTER
    ========================== -->

    <footer>

        © 2026 Jomar John M. Paquibo.
        All Rights Reserved.

    </footer>

</body>
</html># JOMARJOHNPAQUIBO_PORTFOLIO
