<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Educational Website</title>
    <style>
        /* CSS من الأكواد الثلاثة */
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
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            font-size: 1.1rem;
            font-weight: bold;
        }
        button:hover {
            background-color: #0056b3;
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
            background-color: #2c3e50;
            padding: 5px 15px;
            border-radius: 5px;
            text-decoration: none;
            transition: background-color 0.3s ease;
        }
        .videos-button:hover {
            background-color: #1a252f;
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
            <!-- سيتم تعبئة هذا القسم بناءً على الكود المدخل -->
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
            const videoContainer = document.getElementById('videos');

            function showLogin() {
                loginContainer.style.display = 'block';
                mainContent.style.display = 'none';
            }

            function showMainContent() {
                loginContainer.style.display = 'none';
                mainContent.style.display = 'block';
            }

            function loadVideoContent(code) {
                let videoHTML = '';

                if (code === 'CODE1') {
                    videoHTML = `
                        <select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
                            <option value="video0">.....option.....</option>
                            <option value="video1">شرح الفصل الثاني (Part 1)</option>
                            <option value="video2">شرح الفصل الثاني (Part 2)</option>
                            <option value="video3">شرح الفصل الثاني (Part 3)</option>
                            <option value="video4">تدريبات الدرس الأول</option>
                            <option value="video5">تدريبات الدرس الثاني</option>
                            <option value="video6">تدريبات الدرس الثالث</option>
                            <option value="video7">تدريبات الدرس الرابع</option>
                        </select>
                        <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">شرح الفصل الثاني (Part 1)</h1>
<iframe src="https://drive.google.com/file/d/1JsbhZ8UWhqh9p2RlecTBrCa5L_8vgJCR/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                 </div>

            <div class="video" id="video2" style="display: none;">
            <h1 class="video-title">شرح الفصل الثاني (Part 2)</h1>
<iframe src="https://drive.google.com/file/d/1fOeP-_8VgSYQkiR5BeMhL0Xt422Wv7Vc/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video3" style="display: none;">
            <h1 class="video-title"> شرح الفصل الثاني (Part 3)</h1>

<iframe src="https://drive.google.com/file/d/17dQEtszqYpmPmpU3GKYfsiyjGmwCHKhq/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
         
              <div class="video" id="video4" style="display: none;">
            <h1 class="video-title">تدريبات الدرس الاول </h1>
            <h1 class="video-title"> part 1</h1>
<iframe src="https://drive.google.com/file/d/1Xafno2FXrklMu3N5udbsb_FAPQwQI0Na/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
             <h1 class="video-title"> part 2</h1>
<iframe src="https://drive.google.com/file/d/1Uqmcfk2Ujoq2X_u8-6K3MTIA7B9NQ-RY/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
             <h1 class="video-title"> part 3</h1>
<iframe src="https://drive.google.com/file/d/1b4NmhBy8VpzKk4wl0ktq9CvVDU5RVhgJ/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
             <h1 class="video-title"> part 4</h1>
<iframe src="https://drive.google.com/file/d/1oYsLZZQhUABeYI9aH2Ac1_eewUfYOC1D/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>

            </div>
              <div class="video" id="video5" style="display: none;">
            <h1 class="video-title"> تدريبات الدرس الثاني</h1>
            <h1 class="video-title"> part 1</h1>
<iframe src="https://drive.google.com/file/d/1n8VJZWh6MZLM5EJZoydah6GQzsvpx_pN/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
           <h1 class="video-title"> part 2</h1>
<iframe src="https://drive.google.com/file/d/1XcTlpD_pOpFchYzye_OzLf54RoxlfVWl/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>

            </div>
            
              <div class="video" id="video6" style="display: none;">
            <h1 class="video-title">تدريبات الدرس الثالث </h1>
                <h1 class="video-title"> part 1</h1>
<iframe src="https://drive.google.com/file/d/1FSiqPd1aI2N6ObTw1IqskrkkT5A3wDeV/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                <h1 class="video-title"> part 2</h1>
<iframe src="https://drive.google.com/file/d/18uhR-4gz7w9Npu9Ronztyu-IMukHurld/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                <h1 class="video-title"> part 3</h1>
<iframe src="https://drive.google.com/file/d/1B0R8m9BavCxYEtXOz1qMHiQMEHqCebAA/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>

            </div>
            
              <div class="video" id="video7" style="display: none;">
            <h1 class="video-title"> تدريبات الدرس الرابع</h1>
            <h1 class="video-title"> part 1</h1>
<iframe src="https://drive.google.com/file/d/11MiD_5E587CPRDIRi4j6nMth61_8YbiW/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            <h1 class="video-title"> part 2</h1>
<iframe src="https://drive.google.com/file/d/1hSEX0DJvQTrggrkmtIm0NxyoEFvd_RN4/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            <h1 class="video-title"> part 3</h1>
<iframe src="https://drive.google.com/file/d/17czArTr3Mms54nFtW00TIeA8PHAS-vpc/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>

            </div>
            
                    `;
                } else if (code === 'CODE2') {
                    videoHTML = `
                        <select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">                
                            <option value="video0">.....option.....</option>
                            <option value="video1">شرح الفصل الثالث (Part 1)</option>
                            <option value="video2">شرح الفصل الثالث (Part 2)</option>
                            <option value="video3">تدريبات الدرس الأول</option>
                            <option value="video4">تدريبات الدرس الثاني</option>
                            <option value="video5">تدريبات الدرس الثالث</option>
                            <option value="video6">تدريبات الدرس الرابع</option>
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

                    `;
                } else if (code === 'CODE3') {
                    videoHTML = `
                        <select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
                            <option value="video0">.....option.....</option>
                            <option value="video1">شرح الفصل الأول</option>
                            <option value="video2">شرح الفصل الرابع</option>
                            <option value="video3">تدريبات الفصل الأول</option>
                            <option value="video4">تدريبات الفصل الثاني</option>
                            <option value="video5">تدريبات الفصل الثالث</option>
                            <option value="video6">تدريبات الفصل الرابع</option>
                        </select>
                                    
            
            
            <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">شرح الفصل الاول</h1>
                 <h1 class="video-title">part (1)</h1>

  <iframe 
    src="https://drive.google.com/file/d/16UzX2Nfb4HGPDUWFTiG_p__RTfMTuXQR/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title">part (2)</h1>

<iframe 
    src="https://drive.google.com/file/d/1rYDFBKZPf4la00IzGtWR4f9Nu7sdqVRD/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title">part (3)</h1>

<iframe 
    src="https://drive.google.com/file/d/1xyBmw7CqQ1XuvjzvjT-srDO0E0xGQG6E/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>

<div class="video" id="video2" style="display: none;">
                <h1 class="video-title">شرح الفصل الرابع </h1>
                 <h1 class="video-title">part (1)</h1>

<iframe 
    src="https://drive.google.com/file/d/1TTlJWmBOe5KrDzch5-azinqcpt92TeM8/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title">part (2)</h1>

<iframe 
    src="https://drive.google.com/file/d/1zOFLEM1CNFqyllYeg7fm312Oi0vDca4o/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title">part (3)</h1>

<iframe 
    src="https://drive.google.com/file/d/1Q5TCeS5Cdt04svAEtJ52OrVQFgE21X0e/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>
<div class="video" id="video3" style="display: none;">
                <h1 class="video-title">تدريبات الفصل الاول</h1>
                                 <h1 class="video-title">part (1)</h1>

                <iframe 
    src="https://drive.google.com/file/d/1un-8-NjBdwYGhJF4t1vxvFc07na-KiJL/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title">part (2)</h1>

<iframe 
    src="https://drive.google.com/file/d/1P1vUgpk7NWmvMkHDT3CoMPzLKynP5bZf/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                 <h1 class="video-title">part (3)</h1>

<iframe 
    src="https://drive.google.com/file/d/1lPxniWhIklJwzkg1s4zghxblZAgVizrb/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>

<div class="video" id="video4" style="display: none;">
                <h1 class="video-title">تدريبات الفصل الثاني</h1>
                                 <h1 class="video-title">part (1)</h1>
<iframe 
    src="https://drive.google.com/file/d/1HwWrfRx0YTNBkBBRRzCmwdmYCryhkvJF/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                                 <h1 class="video-title">part (2)</h1>

<iframe 
    src="https://drive.google.com/file/d/1B28GGn5O-YVse6VtQzk0aHVsES-4zbKa/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>

<div class="video" id="video5" style="display: none;">
                <h1 class="video-title">تدريبات الفصل الثالث</h1>
                                 <h1 class="video-title">part (1)</h1>
<iframe 
    src="https://drive.google.com/file/d/1_pSdMvY0UKJ23Vv-aye9-aAyr3aYV0BX/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                                 <h1 class="video-title">part (2)</h1>

<iframe 
    src="https://drive.google.com/file/d/19vgZBaNM1gkjHCRwKVHiRX3us9IphDy-/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>

<div class="video" id="video6" style="display: none;">
                <h1 class="video-title">تدريبات الفصل الرابع</h1>
                                 <h1 class="video-title">part (1)</h1>
<iframe 
    src="https://drive.google.com/file/d/14o9Y0DRinHZe0AJ-QOr0ACtQcTuDDM1_/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
                                 <h1 class="video-title">part (2)</h1>

<iframe 
    src="https://drive.google.com/file/d/1lXffint_g9wgofI4gc5nO7ID0u4dEvNp/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
      </div>
                    `;
                } else if (code === 'CODE4') {
                    videoHTML = `
                        <select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
                            <option value="video0">.....option.....</option>
                            <option value="video1">شرح الفصل الخامس part.1</option>
                            <option value="video2">شرح الفصل الخامس part.2</option>
                            <option value="video3">شرح الفصل الخامس part.3</option>
                            <option value="video4">تدريبات الفصل الخامس</option>
                            <option value="video5">شرح الفصل السادس part.1</option>
                            <option value="video6">شرح الفصل السادس part.2</option>
                            <option value="video6">تدريبات الفصل السادس</option>
                        </select>
                                   
<div class="video" id="video1" style="display: none;">
<h1 class="video-title">شرح الفصل الخامس part.1</h1>
<iframe 
    src="https://drive.google.com/file/d/1IZfE3pnggeVN-yFaRmtHHWPSyFaJWSFA/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>
                                   
<div class="video" id="video2" style="display: none;">
<h1 class="video-title">شرح الفصل الخامس part.2</h1>
<iframe 
    src="https://drive.google.com/file/d/12ozPmVjysD4ySqiPPe25sY70g98wR3AV/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>
                                   
<div class="video" id="video3" style="display: none;">
<h1 class="video-title">شرح الفصل الخامس part.3</h1>
<iframe 
    src="https://drive.google.com/file/d/1fL34DsdA_lbeMMBLshtDyM0s0eSEoKO7/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>

    </div>
  
                                   
<div class="video" id="video4" style="display: none;">
<h1 class="video-title">تدريبات الفصل الخامس</h1>
<iframe 
    src="https://drive.google.com/file/d/19PrLNK2C4kYOG-hHt04vylfxAlsz4FgA/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>

    </div>
                                   
<div class="video" id="video5" style="display: none;">
<h1 class="video-title">شرح الفصل السادس part.1</h1>
<iframe 
    src="https://drive.google.com/file/d/16Gkts-ij62FF_JV5aWiWSaNruoc5PBG7/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>
    
                                   
<div class="video" id="video6" style="display: none;">
<h1 class="video-title">شرح الفصل السادس part.2</h1>
<iframe 
    src="https://drive.google.com/file/d/19ku0XT2tw2FvnWG5UYKrdbZ98jFU8K93/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>
    
    
                                   
<div class="video" id="video7" style="display: none;">
<h1 class="video-title">تدريبات الفصل السادس</h1>
<iframe 
    src="https://drive.google.com/file/d/1AMktiCnt4ny3SdtpK4AnFlxToTxVd0hH/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div> `;
}
                videoContainer.innerHTML = videoHTML;

                const videoSelector = document.getElementById('videoSelector');
                if (videoSelector) {
                    videoSelector.addEventListener('change', function () {
                        const selectedVideo = videoSelector.value;
                        const videos = document.querySelectorAll('.video');
                        videos.forEach(video => video.style.display = 'none');
                        const videoToShow = document.getElementById(selectedVideo);
                        if (videoToShow) {
                            videoToShow.style.display = 'block';
                        }
                    });
                }
            }

            document.getElementById('loginForm').addEventListener('submit', function (event) {
                event.preventDefault();

                const username = document.getElementById('username').value.trim();
                const errorMessage = document.getElementById('errorMessage');

                const validUsernames = {
                    'CODE1': ['45454', '18234', '19543', '52614', '51367', '74659', '76431', '63824', '72904', '52918', '84957', '71945', '83629', '38241', '47285', '29067', '94185', '90576', '35926', '83415', '47623', '63172', '81023', '67892', '85297', '24785', '74381', '90283', '19473'],
                    
                    'CODE2': ['45454', , '13227', '66100', '51089', '42877', '92584', '81807', '29699', '96915', '83933', '15134', '85643', '99949', '20995', '39094', '41661', '49757', '52293', '65639', '16495', '17290', '15417', '84597', '16833', '34244', '16228', '57031', '59657', '31693'],
                    
                    'CODE3': [ '85800', '64622', '48007', '45427', '93111', '99452', '60560', '56689', '13885', '30329', '12103', '18638', '35358', '79862', '40574', '22080', '93577', '75673', '66981', '20482', '62787', '96462', '31451', '89339', '12833', '81447', '96579', '31230'],

                   'CODE4': ['23218', '74138', '59055', '40555', '50599','42923', '62461', '53810', '20534', '42979', '34383', '98406', '14639', '92421', '20267', '26378', '12506','39637', '37625', '11908','51746', '70910', '10852', '56540', '99246',  '85281', '37906', '38005', '94620', '99935']
                };

                let code = '';
                for (const [key, values] of Object.entries(validUsernames)) {
                    if (values.includes(username)) {
                        code = key;
                        break;
                    }
                }

                if (code) {
                    errorMessage.textContent = '';
                    loadVideoContent(code);
                    showMainContent();
                } else {
                    errorMessage.textContent = 'Invalid username';
                }
            });

            showLogin();
        });
    </script>
