<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Educational Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            font-weight: bold;
            margin: 0;
            padding: 0;
            background-color: #718e97;
        }
        nav {
            background-color: #6a828a;
            padding: 10px;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }
        .menu-content {
            background-color: #6D1865;
            color: white;
            padding: 10px;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
        }
        main {
            padding: 20px;
        }
        .video-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-top: 20px;
        }
        .video-container h2 {
            color: #2c3e50;
        }
        .wistia_embed {
            width: 80%;
            max-width: 800px;
            margin-bottom: 20px;
        }
        .login-container {
            background-color: #ffffff;
            padding: 2.5rem;
            border-radius: 12px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
            width: 100%;
            max-width: 500px;
            text-align: center;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            display: block;
        }
        .login-container.active {
            display: block;
        }
        h1 {
            margin-bottom: 1.5rem;
            font-size: 2rem;
            color: #333;
        }
        label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: #555;
        }
        input {
            width: 100%;
            padding: 0.75rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
            border-radius: 6px;
            box-sizing: border-box;
            font-size: 1rem;
            color: #333;
        }
        button {
            width: 100%;
            padding: 0.75rem;
            background-color: #007bff; /* Change this to your preferred color */
            color: #fff;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            font-size: 1.1rem;
            font-weight: bold;
        }
        button:hover {
            background-color: #0056b3; /* Change this for the hover effect */
        }
        .error {
            color: red;
            margin-top: 1rem;
        }
        .hidden {
            display: none;
        }
        .welcome-message {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: #2c3e50;
        }
        .videos-button {
            color: #6D1865;
            background-color: #2c3e50; /* Dark color for the button */
            padding: 5px 15px;
            border-radius: 5px;
            text-decoration: none;
            transition: background-color 0.3s ease;
        }
        .videos-button:hover {
            background-color: #1a252f; /* Slightly darker on hover */
        }
    </style>
</head>
<body>
    <nav id="nav">
        <ul>
        </ul>
    </nav>
    
    <main id="main" style="display:none;">
        <section id="home">
            <div style="text-align: center; padding: 20px; border-radius: 8px;">
                <img src="https://i.ibb.co/59zvgNq/image-removebg-preview-6-removebg-preview-1.png" alt="The Process Platform Image" style="width: 100%; max-width: 400px; margin-bottom: 20px;">
                <h2 style="color: white;">The Process Platform</h2>
            </div>
        </section>

        <section id="videos" class="video-container">
<select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
                <option value="video0">.....option.....</option>
                <option value="video1">شرح الفصل الثالث (Part 1) </option>
                <option value="video2">شرح الفصل الثالث (Part 2)</option>
                <option value="video3">تدريبات الدرس الاول </option>
                <option value="video4">تدريبات الدرس الثاني </option>
                <option value="video5">تدريبات الدرس الثالث </option>
                <option value="video6">تدريبات الدرس الرابع </option>
            </select>
            
            
            
            <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">شرح الفصل الثالث (Part 1)</h1>
  <iframe 
    src="https://drive.google.com/file/d/13hf2rREv3bIV-aiuAj94sZcLDxj8qKu0/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
  </iframe>
</div>
</div>
            <div class="video" id="video2" style="display: none;">
                <h1 class="video-title">شرح الفصل الثالث (Part 2)</h1>
  <iframe 
    src="https://drive.google.com/file/d/1FnyiymnXUG2yIy1f_6NVodCAfcpQ0059/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
  </iframe>
</div>
            <div class="video" id="video3" style="display: none;">
                <h1 class="video-title">تدريبات الدرس الاول  </h1>
                 <h1 class="video-title"> (part1) </h1>

<iframe 
    src="https://drive.google.com/file/d/1CqnOF1m6Ce_pfI13c8vJc5ViLy6bWHeW/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title"> (part2) </h1>

<iframe 
    src="https://drive.google.com/file/d/1OJ2uBI8RfdQeWVQBK1QXjvfvDli18_Yo/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title"> (part3) </h1>

<iframe 
    src="https://drive.google.com/file/d/15RTu4Y3nbUEA18OgfKlMZC6F4VPS3USI/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
</div>
<div class="video" id="video4" style="display: none;">
                <h1 class="video-title">تدريبات الدرس الثاني  </h1>
                 <h1 class="video-title"> (part1) </h1>

<iframe 
    src="https://drive.google.com/file/d/1W_7GGE6DBv-IKeoYckUhSDyHz93zO41Y/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title"> (part2) </h1>

<iframe 
    src="https://drive.google.com/file/d/1q5NttcIKMYaK-YTClB6Jv8jcVHWJNLB_/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
</div>
<div class="video" id="video5" style="display: none;">
                <h1 class="video-title">تدريبات الدرس الثاث  </h1>
                 <h1 class="video-title"> (part1) </h1>
<iframe 
    src="https://drive.google.com/file/d/1otMVRc-NX9dZAiod0wag4-FsYMIM_IkV/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title"> (part2) </h1>

<iframe 
    src="https://drive.google.com/file/d/1DiGwZVOBSwrcKmLdpIO8pOkKstMTmQpV/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
</div>
<div class="video" id="video6" style="display: none;">
                <h1 class="video-title">تدريبات الدرس الرابع  </h1>
<iframe 
    src="https://drive.google.com/file/d/19D6HIpfepV8N2lfD5_we8NjCjYy-Q6Wd/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
</div>

        </section>
        
        <section id="contact">
            <h2>Contact Us</h2>
            <p>If you have any questions or need further information, feel free to contact us at <a href="mailto:info@educationwebsite.com">mamrro8529@gmail.com</a>.</p>
            <div class="social-icons">
                <a href="https://wa.me/message/5LRM2DVHPZQFM1" target="_blank">
                    <img src="https://img.icons8.com/fluent/48/000000/whatsapp.png" alt="WhatsApp" />
                </a>
                <a href="https://www.facebook.com/mamro8529?mibextid=ZbWKwL" target="_blank">
                    <img src="https://img.icons8.com/fluent/48/000000/facebook-new.png" alt="Facebook" />
                </a>
                <a href="http://t.me/Mora_mo1" target="_blank">
                    <img src="https://img.icons8.com/fluent/48/000000/telegram-app.png" alt="Telegram" />
                </a>
                <p>Developed by Eng: Amr Mohamed</p>
            </div>
        </section>
    </main>

    <div class="login-container" id="loginContainer">
        <img src="https://i.ibb.co/nmgZDmT/Whats-App-Image-2024-09-04-at-15-05-46-removebg-preview.png" alt="Login Image" style="width: 60%; max-width: 300px; margin-bottom: 20px;">
        <h1>Login to The Process platform</h1>
        <form id="loginForm">
            <label for="username">Username</label>
            <input type="text" id="username" name="username" required>
            <button type="submit">Login</button>
            <div id="errorMessage" class="error"></div>
        </form>
        <p>Developed by Eng: Amr Mohamed</p>
    </div>

<script>
document.addEventListener('DOMContentLoaded', function () {
    const loginContainer = document.getElementById('loginContainer');
    const mainContent = document.getElementById('main');
    const videoSelector = document.getElementById('videoSelector');
    const video1 = document.getElementById('video1');
    const video2 = document.getElementById('video2');

    function showLogin() {
        loginContainer.style.display = 'block';
        mainContent.style.display = 'none';
    }

    function showMainContent() {
        loginContainer.style.display = 'none';
        mainContent.style.display = 'block';
    }

    document.getElementById('loginForm').addEventListener('submit', function (event) {
        event.preventDefault();

        const username = document.getElementById('username').value.trim();
        const errorMessage = document.getElementById('errorMessage');

        // List of valid usernames
        const validUsernames = [
            '45454', '0', '13227', '66100', '51089', '42877',
'92584', '81807', '29699', '96915',
'83933', '15134', '85643', '99949',
'20995', '39094', '41661', '49757',
'52293', '65639', '16495', '17290',
'15417', '84597', '16833', '34244',
'16228', '57031', '59657', '31693'

        ];

        // Validate username
        if (validUsernames.includes(username)) {
            errorMessage.textContent = '';
            showMainContent();
        } else {
            errorMessage.textContent = 'Invalid username';
        }
    });

    // Video selection handler
    videoSelector.addEventListener('change', function() {
    // Hide all videos initially
    for (let i = 1; i <= 12; i++) {
        let video = document.getElementById('video' + i);
        if (video) {
            video.style.display = 'none';
        }
    }

    // Show the selected video
    let selectedVideo = videoSelector.value;
    let videoToShow = document.getElementById(selectedVideo);
    if (videoToShow) {
        videoToShow.style.display = 'block';
    }
});


    showLogin();
});
</script>
