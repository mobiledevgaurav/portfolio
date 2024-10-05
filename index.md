
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume - Gaurav Patil</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            background-image: linear-gradient(to right, #e0eafc, #cfdef3);
            scroll-behavior: smooth; /* Enable smooth scrolling */
        }

        .resume-container {
            max-width: 1000px;
            margin: 30px auto;
            background: rgba(255, 255, 255, 0.9);
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }

        .tabs {
            display: flex;
            justify-content: space-around;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }

        .tabs button {
            background-color: #8e44ad;
            color: white;
            border: none;
            padding: 15px 20px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
            font-size: 18px; /* Increased font size */
            flex: 1;
            margin: 5px;
            border-radius: 8px;
            position: relative;
            overflow: hidden;
        }

        .tabs button:hover {
            background-color: #9b59b6;
            transform: translateY(-2px);
        }

        .tabs button.active {
            background-color: #6f2c91;
        }

        .tab-content {
            display: none;
            opacity: 0; /* Start hidden */
            transition: opacity 0.5s ease-in-out; /* Smooth opacity transition */
        }

        .tab-content.active {
            display: block;
            opacity: 1; /* Fade in */
        }

        h1 {
            text-align: center;
            font-size: 36px;
            color: #2c3e50;
        }

        h2 {
            font-size: 26px; /* Increased font size */
            color: #2980b9;
            margin-bottom: 20px;
        }

        h3 {
            color: #8e44ad;
            margin-top: 0;
            font-size: 20px; /* Increased font size */
        }

        ul {
            list-style-type: none;
            padding-left: 0;
        }

        ul li {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            transition: transform 0.3s;
        }

        ul li:hover {
            transform: translateX(5px);
        }

        ul li i {
            margin-right: 10px;
            color: #3498db;
            font-size: 1.5em;
        }

        .section {
            margin-bottom: 20px;
        }

        .card {
            background-color: #ecf0f1;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .contact a {
            color: #3498db;
            text-decoration: none;
            font-weight: bold;
        }

        .contact a:hover {
            text-decoration: underline;
        }

        /* Responsive Design */
        @media screen and (max-width: 768px) {
            .resume-container {
                padding: 20px;
                margin: 20px;
                max-width: 100%;
            }

            h1 {
                font-size: 28px;
            }

            h2 {
                font-size: 22px; /* Adjusted for better clarity */
            }

            .tabs {
                flex-direction: column;
            }

            .tabs button {
                padding: 10px;
                font-size: 16px; /* Adjusted for better clarity */
            }

            .card {
                padding: 15px;
            }

            ul li {
                font-size: 14px; /* Adjusted for better clarity */
            }
        }

        @media screen and (max-width: 480px) {
            .resume-container {
                padding: 15px;
            }

            h1 {
                font-size: 24px;
            }

            h2 {
                font-size: 20px; /* Adjusted for better clarity */
            }

            .tabs button {
                font-size: 14px; /* Adjusted for better clarity */
                padding: 8px;
            }

            .card {
                padding: 10px;
            }

            ul li {
                font-size: 12px; /* Adjusted for better clarity */
            }
        }
    </style>
</head>
<body>
    <div class="resume-container">
        <h1>Gaurav Patil</h1>

        <!-- Tabs -->
        <div class="tabs">
            <button class="tab-link active" onclick="openTab(event, 'about')">About Me</button>
            <button class="tab-link" onclick="openTab(event, 'skills')">Skills</button>
            <button class="tab-link" onclick="openTab(event, 'experience')">Experience</button>
            <button class="tab-link" onclick="openTab(event, 'education')">Education</button>
        </div>

        <!-- Tab Content -->
        <div id="about" class="tab-content active">
            <h2>About Me</h2>
            <div class="card">
                <p>"I am a passionate mobile app developer dedicated to creating cutting-edge applications that prioritize security and sustainability. By leveraging object-oriented programming principles, I focus on streamlining code, optimizing app size, and maximizing reusability to deliver exceptional user experiences."</p>
            </div>
            <div class="section contact">
                <h3>Contact</h3>
                <ul>
                    <li><i class="fas fa-envelope"></i>Email: <a href="mailto:gaurav.patil97@outlook.com">gaurav.patil97@outlook.com</a></li>
                    <li><i class="fas fa-phone"></i>Phone: 9595402012</li>
                    <li><i class="fas fa-map-marker-alt"></i>Location: Pune, India</li>
                    <li><i class="fab fa-linkedin"></i>LinkedIn: <a href="https://linkedin.com/in/gaurav-patil-b6bb96187">linkedin.com/in/gaurav-patil</a></li>
                </ul>
            </div>
        </div>

        <div id="skills" class="tab-content">
            <h2>Skills</h2>

           <div class="card">
                <ul>
                    <li><i class="fas fa-code"></i>.NET MAUI</li>
                    <li><i class="fas fa-code"></i>Xamarin</li>
                    <li><i class="fas fa-code"></i>C#</li>
                    <li><i class="fas fa-network-wired"></i>REST APIs</li>
                    <li><i class="fas fa-file-code"></i>XML</li>
                    <li>
<i class="fab fa-github"></i>GitHub</li>
                </ul>
            </div>
        </div>

        <div id="experience" class="tab-content">
            <h2>Work Experience</h2>
            <div class="card">
                <h3>Xamarin Developer - Incision</h3>
                <p>WAi Technologies, Pune (05/2022 - 11/2023)</p>
                <ul>
                    <li>Developed responsive mobile applications for both Android and iOS platforms.</li>
                    <li>Implemented REST APIs and managed API calls, ensuring effective data binding with MVVM architecture.</li>
                    <li>Created various UI components, including checkboxes, date pickers, and sliders.</li>
                </ul>
            </div>
            <div class="card">
                <h3>Xamarin Developer - Live Broiler Booking</h3>
                <p>Venky's India Ltd, Pune (12/2023 - Present)</p>
                <ul>
                    <li>Developed role-based permissions for administrators and users.</li>
                    <li>Integrated REST APIs for operations such as POST, GET, and UPDATE.</li>
                </ul>
            </div>
        </div>

                <div id="education" class="tab-content">
            <h2>Education</h2>
            <div class="card">
                <h3>Bachelor of Engineering</h3>
                <p>Pravara Rural Engineering College, Loni (2016 - 2021)</p>
                <p>Degree in Information Technology - 70.80%</p>
            </div>
        </div>
    </div>

    <script>
        function openTab(evt, tabName) {
            var tabContent = document.getElementsByClassName("tab-content");
            for (var i = 0; i < tabContent.length; i++) {
                tabContent[i].classList.remove("active");
                tabContent[i].style.display = "none"; // Hide all tabs
            }

            var tabLinks = document.getElementsByClassName("tab-link");
            for (var i = 0; i < tabLinks.length; i++) {
                tabLinks[i].classList.remove("active");
            }

            // Show the current tab and add active class to the button
            document.getElementById(tabName).style.display = "block";
            document.getElementById(tabName).classList.add("active");
            evt.currentTarget.classList.add("active");
        }
    </script>
</body>
</html>
