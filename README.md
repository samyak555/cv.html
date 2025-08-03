<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Samyak Jain - Intern</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        /* Custom CSS for enhanced aesthetics */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #000000; /* Changed to black background */
            color: #eef2f6; /* Lighter text for better contrast on black */
            line-height: 1.6;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2.5rem; /* Increased padding */
        }
        .section-title {
            font-size: 2.5rem; /* Slightly larger title */
            font-weight: 800; /* Extra bold */
            color: #4299e1; /* Vibrant blue for titles */
            margin-bottom: 2rem; /* More space below title */
            border-bottom: 4px solid #4299e1; /* Thicker, vibrant blue border */
            padding-bottom: 0.75rem;
            text-align: center; /* Center align section titles */
            letter-spacing: 0.05em; /* Slight letter spacing */
        }
        .card {
            background-color: #1a202c; /* Darker card background for contrast */
            border-radius: 1.25rem; /* More rounded corners */
            box-shadow: 0 15px 25px rgba(0, 0, 0, 0.3); /* Stronger shadow */
            padding: 2.5rem; /* Increased padding */
            margin-bottom: 2rem; /* More space between cards */
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
        }
        .card:hover {
            transform: translateY(-8px); /* Lift effect on hover */
            box-shadow: 0 20px 35px rgba(0, 0, 0, 0.4); /* Enhanced shadow on hover */
        }
        .project-card {
            background-color: #2d3748; /* Darker background for projects */
            border-left: 6px solid #4299e1; /* Thicker, vibrant border */
            padding: 1.75rem; /* Increased padding */
            border-radius: 1rem; /* More rounded corners */
            margin-bottom: 1.25rem;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2); /* Subtle shadow for project cards */
        }
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
        }
        .skill-badge {
            background-color: #2b6cb0; /* Darker blue for badges */
            color: #ffffff; /* White text */
            padding: 0.6rem 1.2rem; /* Larger padding */
            border-radius: 9999px;
            font-weight: 600; /* Semi-bold */
            margin-right: 0.8rem;
            margin-bottom: 0.8rem;
            display: inline-block;
            transition: background-color 0.2s ease;
        }
        .skill-badge:hover {
            background-color: #3182ce; /* Slightly darker on hover */
        }
        .link-button {
            display: inline-block;
            background-color: #4299e1; /* Vibrant blue */
            color: white;
            padding: 0.9rem 1.8rem; /* Larger buttons */
            border-radius: 0.75rem;
            text-decoration: none;
            font-weight: 700; /* Bold text */
            transition: background-color 0.3s ease, transform 0.2s ease;
            box-shadow: 0 5px 15px rgba(66, 153, 225, 0.4); /* Shadow for buttons */
        }
        .link-button:hover {
            background-color: #3182ce; /* Darker blue on hover */
            transform: translateY(-2px); /* Slight lift on hover */
            box-shadow: 0 8px 20px rgba(66, 153, 225, 0.6);
        }

        /* Highlight for DRDO experience */
        .drdo-highlight {
            background-color: #2c7a7b; /* Darker teal background */
            border: 3px solid #38b2ac; /* Stronger teal border */
            border-radius: 1rem;
            padding: 1.5rem;
            margin-bottom: 1rem;
            box-shadow: 0 8px 20px rgba(56, 178, 172, 0.2); /* Teal shadow */
            transition: all 0.3s ease-in-out;
        }
        .drdo-highlight:hover {
            transform: scale(1.02); /* Slightly larger on hover */
            box-shadow: 0 12px 25px rgba(56, 178, 172, 0.3);
        }

        /* Highlight for achievements */
        .achievement-highlight {
            background-color: #b7791f; /* Darker goldenrod yellow */
            border: 2px solid #daa520; /* Goldenrod border */
            border-radius: 0.5rem;
            padding: 0.5rem 1rem;
            margin-bottom: 0.5rem;
            display: list-item; /* Ensure it behaves as a list item */
            list-style: disc; /* Keep the bullet point */
            margin-left: 1.5rem; /* Indent to align with other list items */
            transition: all 0.3s ease-in-out;
        }
        .achievement-highlight:hover {
            transform: translateX(5px); /* Slight shift on hover */
            box-shadow: 0 4px 10px rgba(218, 165, 32, 0.2);
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .container {
                padding: 1.5rem;
            }
            .section-title {
                font-size: 2rem;
            }
            .card {
                padding: 1.5rem;
            }
            .link-button {
                padding: 0.75rem 1.25rem;
                font-size: 0.9rem;
            }
            .grid-cols-1.md\:grid-cols-2 {
                grid-template-columns: 1fr; /* Stack projects on small screens */
            }
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">
    <div class="container">
        <!-- Header Section -->
        <header class="text-center py-10 bg-gray-950 rounded-xl shadow-2xl mb-10">
            <h1 class="text-6xl font-extrabold text-blue-500 mb-4 tracking-wide">SAMYAK JAIN</h1>
            <p class="text-3xl font-semibold text-gray-200 mb-6">Intern | 3rd Year Undergrad</p>
            <div class="flex flex-wrap justify-center gap-6">
                <a href="https://www.linkedin.com/in/samyak-jain-23a14b288?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank" class="link-button">
                    LinkedIn
                </a>
                <a href="#" class="link-button">
                    samyak.jain2023@vitstudent.ac.in
                </a>
                <a href="#" class="link-button">
                    +91 6260495065
                </a>
            </div>
        </header>

        <!-- About Me Section -->
        <section class="card">
            <h2 class="section-title">About Me</h2>
            <p class="text-lg leading-relaxed text-gray-200">
                I am a second-year B.Tech student with a strong foundation in Electronics, Robotics, AI, and Software
                Development. My expertise includes circuit design, microcontroller programming, embedded systems, and
                building functional prototypes. I have worked extensively with Computer Vision for dataset training and
                implemented LiDAR, ROS, and path-planning algorithms. Additionally, I have a solid grasp of Data Structures and
                Algorithms (DSA) and am proficient in multiple programming languages.
            </p>
        </section>

        <!-- Education Section -->
        <section class="card">
            <h2 class="section-title">Education</h2>
            <div class="mb-6">
                <h3 class="text-2xl font-bold text-blue-500">Bachelor's Degree in Electronics And Computer Engineering</h3>
                <p class="text-lg text-gray-200">Vellore Institute Of Technology, Chennai, Tamil Nadu</p>
                <p class="text-md text-gray-300">2023-2027 | CGPA: 8.09</p>
            </div>
            <div>
                <h3 class="text-2xl font-bold text-blue-500">Higher Secondary Education</h3>
                <p class="text-lg text-gray-200">CBSE Board, 2022</p>
                <p class="text-md text-gray-300">10th: 93.4% , 12th: 81.2%</p>
            </div>
        </section>

        <!-- Skills Section -->
        <section class="card">
            <h2 class="section-title">Skills</h2>
            <div class="flex flex-wrap justify-center">
                <span class="skill-badge">C++ & C</span>
                <span class="skill-badge">Python</span>
                <span class="skill-badge">Embedded C</span>
                <span class="skill-badge">Verilog</span>
                <span class="skill-badge">Nvidia Jetson Nano</span>
                <span class="skill-badge">ROS2</span>
                <span class="skill-badge">LIDAR</span>
                <span class="skill-badge">Autodesk-TinkerCAD</span>
                <span class="skill-badge">Java</span>
                <span class="skill-badge">Data Structure and Algorithm</span>
                <span class="skill-badge">Investment Acumen</span>
                <span class="skill-badge">Computer Vision</span>
                <span class="skill-badge">Microcontroller Programming</span>
                <span class="skill-badge">Embedded Systems</span>
                <span class="skill-badge">Circuit Design</span>
            </div>
        </section>

        <!-- Professional Experience Section -->
        <section class="card">
            <h2 class="section-title">Professional Experience</h2>
            <div class="drdo-highlight mb-8">
                <h3 class="text-2xl font-bold text-blue-500">Interned</h3>
                <p class="text-xl text-gray-200 mb-2">Defence Research and Development Organization (DRDO), Delhi</p>
                <ul class="list-disc list-inside text-gray-200 mt-2 space-y-2">
                    <li>Engaged in LiDAR operations, building LiDAR cartography, and using the data for obstacle evasion.</li>
                    <li>Implemented object recognition via OpenCV and the YOLOv8 dataset using a webcam.</li>
                    <li>Utilized ROS2 and trajectory planning for autonomous rover mobility.</li>
                    <li>Worked on FPGA.</li>
                </ul>
            </div>
            <div class="mb-8">
                <h3 class="text-2xl font-bold text-blue-500">Deputy Lead of Outreach and Media</h3>
                <p class="text-xl text-gray-200 mb-2">Namo Nirvana Special Robotic Team</p>
                <ul class="list-disc list-inside text-gray-200 mt-2 space-y-2">
                    <li>Led outreach initiatives to promote team activities and recruit new members.</li>
                    <li>Managed media relations and created content for various platforms.</li>
                </ul>
            </div>
            <div class="mb-8">
                <h3 class="text-2xl font-bold text-blue-500">College Team - ISRO Robotics Challenge 2024</h3>
                <p class="text-xl text-gray-200 mb-2">Vellore Institute Of Technology, Chennai</p>
                <ul class="list-disc list-inside text-gray-200 mt-2 space-y-2">
                    <li>Developed pathfinding and obstacle avoidance algorithms using LiDAR & IMU.</li>
                    <li>Optimized route efficiency and logged data for performance analysis.</li>
                </ul>
            </div>
            <div>
                <h3 class="text-2xl font-bold text-blue-500">VIT Finance Club</h3>
                <p class="text-xl text-gray-200 mb-2">Vellore Institute Of Technology, Chennai</p>
                <ul class="list-disc list-inside text-gray-200 mt-2 space-y-2">
                    <li>Assisted in financial planning and analysis for club activities.</li>
                    <li>Contributed to budgeting and resource allocation strategies.</li>
                </ul>
            </div>
        </section>

        <!-- Projects Section -->
        <section class="card">
            <h2 class="section-title">Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">Terrain Scout: Multi-Operational Defence Rover (2024)</h3>
                    <p class="text-gray-200">Developed an AI-based object detection system to classify soldiers as friendly or enemy, optimized model accuracy, and structured detection data for CNN improvements.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">IoT Smart Parking Management System (2024)</h3>
                    <p class="text-gray-200">Designed a Python-based data pipeline and SQL database for real-time parking management, improving space utilization by 15% through EDA and visualization.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">Heart Rate Signal Processing (2024)</h3>
                    <p class="text-gray-200">Implemented CNN models for heart rate classification, detected cardiac abnormalities using statistical analysis, and enhanced efficiency by 10% with Python & MATLAB.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">Created a Banana Cluster Project</h3>
                    <p class="text-gray-200">Recognised and funded by MP Government.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">Robofest Gujarat</h3>
                    <p class="text-gray-200">Designed a swarm of autonomous micro-drones for Robofest Gujarat's Minefield Navigation Challenge. Operated via voice/gesture, the swarm maps mines, avoids obstacles, marks safe paths, and guides a person across a 100-meter minefield in under 10 minutes using only onboard computation and coordination.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">BeeChat</h3>
                    <p class="text-gray-200">BeeChat is a peer-to-peer Bluetooth-based messaging app enabling offline communication without internet or cellular networks. Inspired by BitChat, it ensures secure, decentralized chat between nearby devices, ideal for short-range, low-latency messaging in remote areas, emergencies, or privacy-focused environments where connectivity is limited or unavailable.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">Gingr</h3>
                    <p class="text-gray-200">Gingr is an innovative anonymous social platform designed to foster real-time, unfiltered conversations and community engagement. Combining elements of Reddit and Omegle, it enables spontaneous interaction, video streaming, and interactive experiences, with a focus on privacy, user freedom, and next-generation digital social networking.</p>
                </div>
                <div class="project-card">
                    <h3 class="text-xl font-semibold text-blue-500 mb-2">PresencePal: AI-Based Attendance System (2024)</h3>
                    <p class="text-gray-200">Built an AI-powered attendance system with face recognition (Fisherfaces LDA) and IP.</p>
                </div>
            </div>
        </section>

        <!-- Achievements Section -->
        <section class="card">
            <h2 class="section-title">Achievements</h2>
            <ul class="list-disc list-inside text-gray-200 space-y-2">
                <li>Spoken Tutorial Certifications: Python, C, and C++ (issued by IIT Bombay).</li>
                <li>Research Paper: Presence Pal AI-powered automated attendance system.</li>
                <li class="achievement-highlight">Won 3rd prize in Techovation Hackathon Competition at Anna University Chennai.</li>
                <li class="achievement-highlight">Techvilla Hackathon Runner Up.</li>
                <li>Leading Member at Namo Nirvana Robotics Special team.</li>
            </ul>
        </section>

        <!-- Footer Section -->
        <footer class="text-center py-8 text-gray-300 text-sm">
            <p>&copy; 2024 Samyak Jain. All rights reserved.</p>
            <p>Designed with <span class="text-red-500">&hearts;</span> and Tailwind CSS</p>
        </footer>
    </div>
</body>
</html>
