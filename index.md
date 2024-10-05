
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resume - Gaurav Patil</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        .resume-container {
            max-width: 1000px;
            margin: 30px auto;
            background: #fff;
            padding: 20px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }

        .tabs {
            display: flex;
            justify-content: space-around;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }

        .tabs button {
            background-color: #2c3e50;
            color: white;
            border: none;
            padding: 15px 20px;
            cursor: pointer;
            transition: background-color 0.3s;
            font-size: 16px;
            flex: 1;
            margin: 5px;
            position: relative;
            overflow: hidden;
        }

        .tabs button:hover {
            background-color: #3498db;
        }

        .tabs button.active {
            background-color: #2980b9;
        }

        .tabs button::before {
            content: '';
            position: absolute;
            left: 50%;
            top: 100%;
            width: 300%;
            height: 300%;
            background: rgba(255, 255, 255, 0.2);
            transition: all 0.5s ease;
            transform: translateX(-50%) rotate(45deg);
        }

        .tabs button:hover::before {
            top: -100%;
        }

        .tab-content {
            display: none;
            animation: fadeIn 0.5s;
        }

        .tab-content.active {
            display: block;
            animation: slideIn 0.5s ease-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideIn {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        h1 {
            text-align: center;
            font-size: 36px;
            color: #2c3e50;
        }

        h2 {
            font-size: 24px;
            color: #2980b9;
            margin-bottom: 20px;
        }

        h3 {
            color: #8e44ad; /* Changed from green to dark purple */
        }

        ul {
            list-style-type: none;
            padding-left: 0;
        }

        ul li {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        ul li i {
            margin-right: 10px;
            color: #3498db;
        }

        .section {
            margin-bottom: 20px;
        }

        .card {
            background-color: #ecf0f1;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.05);
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
                padding: 15px;
                margin: 20px;
                max-width: 100%;
            }

            h1 {
                font-size: 28px;
            }

            h2 {
                font-size: 20px;
            }

            .tabs {
                flex-direction: column;
            }

            .tabs button {
                padding: 10px;
                font-size: 14px;
            }

            .card {
                padding: 10px;
            }

            ul li {
                font-size: 14px;
            }
        }

        @media screen and (max-width: 480px) {
            .resume-container {
                padding: 10px;
            }

            h1 {
                font-size: 24px;
            }

            h2 {
                font-size: 18px;
            }

            .tabs button {
                font-size: 12px;
                padding: 8px;
            }

            .card {
                padding: 8px;
            }

            ul li {
                font-size: 12px;
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
                <p>"Experienced software developer with 2.3 years of proven expertise seeking a higher-level position to leverage strong coding and problem-solving skills. Eager to contribute to a dynamic team and drive impactful solutions."</p>
            </div>
            <div class="section contact">
                <h3>Contact</h3>
                <ul>
                    <li><i class="fas fa-envelope"></i>Email: <a href="mailto:gaurav.patil97@outlook.com">gaurav.patil97@outlook.com</a></li>
                    <li><i class="fas fa-phone"></i>Phone: 9595402012</li>
                    <li><i class="fas fa-map-marker-alt"></i>Location: Jalgaon, India</li>
                    <li><i class="fab fa-linkedin"></i>LinkedIn: <a href="https://linkedin.com/in/gaurav-patil-b6bb96187">linkedin.com/in/gaurav-patil</a></li>
                    <li><i class="fas fa-globe"></i>Website: <a href="https://yourwebsite.com">yourwebsite.com</a></li>
                </ul>
            </div>
        </div>

        <div id="skills" class="tab-content">
            <h2>Skills</h2>
            <div class="card">
                <ul>
                    <li><i class="fas fa-code"></i>Xamarin, MAUI, Dart</li>
                    <li><i class="fas fa-code"></i>XML, C#</li>
                    <li><i class="fas fa-code"></i>MVVM Architecture</li>
                    <li><i class="fas fa-mobile-alt"></i>Xamarin Android, iOS</li>
                    <li><i class="fas fa-network-wired"></i>RESTful API, Swagger, Postman, Git</li>
                </ul>
            </div>
        </div>

        <div id="experience" class="tab-content">
            <h2>Work Experience</h2>
            <div class="card">
                <h3>Incision (Xamarin Developer)</h3>
                <p>WAi Technologies, Pune (05/2022 - 11/2023)</p>
                <ul>
                    <li>Worked on different device responsiveness for mobile applications on Android and iOS.</li>
                    <li>Implemented REST APIs, API calling, data binding with MVVM architecture.</li>
                    <li>Developed various views like checkboxes, date pickers, sliders, etc.</li>
                </ul>
            </div>
            <div class="card">
                <h3>Live Broiler Booking (Xamarin Developer)</h3>
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
                <p>Information Technologies - 70.80%</p>
            </div>
        </div>
    </div>

    <script>
        function openTab(evt, tabName) {
            // Hide all tab contents
            var tabContent = document.getElementsByClassName("tab-content");
            for (var i = 0; i < tabContent.length; i++) {
                tabContent[i].style.display = "none";
                tabContent[i].classList.remove("active");
            }

            // Remove active class from all tab buttons
            var tabLinks = document.getElementsByClassName("tab-link");
            for (var i = 0; i < tabLinks.length; i++) {
                tabLinks[i].classList.remove("active");
            }

            // Show the current tab, and add an "active" class to the clicked tab button
            document.getElementById(tabName).style.display = "block";
            evt.currentTarget.classList.add("active");
        }
    </script>
</body>
</html>
