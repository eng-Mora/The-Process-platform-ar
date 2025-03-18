<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Process</title>
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
<section id="videos" class="video-container">
<select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
            <option value="video1">.....option.....</option>
                <option value="video1">Magnetic flux </option>
                <option value="video2">Flux density due to current passing in straight wire</option>
                <option value="video3">Total flux density</option>
                <option value="video4">Cicular coil </option>
                <option value="video5">Solenoid </option>
                <option value="video6">Magnetic force </option>
                <option value="video7">Torque </option>
                <option value="video8">Galvanometer </option>
                <option value="video9">Ammeter </option>
                <option value="video10">Voltmeter </option>
                <option value="video11">Ohmmeter </option>
                <option value="video12">Important on devices</option>
                <option value="video13">Lecture 1 exercises</option>
                <option value="video14">Lecture 2 exercises</option>
                <option value="video15">Lecture 3 exercises</option>
                <option value="video16">Lecture 4 exercises</option>
                
                
            </select>
            
            
            
            <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">Magnetic flux</h1>
<iframe src="https://drive.google.com/file/d/15KaT0AVNz1WNIaT2sSkWzxNlFdnrKiNi/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                 </div>

            <div class="video" id="video2" style="display: none;">
            <h1 class="video-title">Flux density due to current passing in straight wire</h1>
<iframe src="https://drive.google.com/file/d/1A8putuPbjHw5CeNHCl_SYby-HdvRN5xH/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video3" style="display: none;">
            <h1 class="video-title"> Total flux density</h1>
<iframe src="https://drive.google.com/file/d/1wLttY10Q-iQ8yXjLIhb8WJPBqwiq6uKo/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
          
              <div class="video" id="video4" style="display: none;">
            <h1 class="video-title">Cicular coil </h1>
<iframe src="https://drive.google.com/file/d/1dDMF-1y_g20K5iec815xjTQesF7ORQdk/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video5" style="display: none;">
            <h1 class="video-title"> Solenoid</h1>
<iframe src="https://drive.google.com/file/d/1KN8YLcwh5csP5MSqC-y5cNOh8saC1kz7/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video6" style="display: none;">
            <h1 class="video-title">Magnetic force </h1>
<iframe src="https://drive.google.com/file/d/10dHYNaaRFkvAuoW7lKZLIWWi9so-5HKR/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video7" style="display: none;">
            <h1 class="video-title"> Torque</h1>
<iframe src="https://drive.google.com/file/d/1WcTWRaxKrMaE6-sA1hDeOVModv_zos7R/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video8" style="display: none;">
            <h1 class="video-title"> Galvanometer</h1>
<iframe src="https://drive.google.com/file/d/1GBm6oLaP1vQSSijqk7_tiK-a_UOK2N2x/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video9" style="display: none;">
            <h1 class="video-title">Ammeter </h1>
<iframe src="https://drive.google.com/file/d/1CGdm_XWQNu_T9LuuVqtoaJwWOvQa1B9K/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
              <div class="video" id="video10" style="display: none;">
            <h1 class="video-title"> Voltmeter</h1>
<iframe src="https://drive.google.com/file/d/1M-5z44sdEw1oP2u3p4WSYEe6gaCarnmB/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
</div>            
             
              <div class="video" id="video11" style="display: none;">
            <h1 class="video-title"> Ohmmeter</h1>
<iframe src="https://drive.google.com/file/d/1B2bPG2Jd3mxGfYwPxvjxVGD4TRKkTH3d/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
              <div class="video" id="video12" style="display: none;">
            <h1 class="video-title"> Important on devices</h1>
<iframe src="https://drive.google.com/file/d/19uTpb0KheuAWuR3vyDylR0ge0EWY-8aW/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
            </div>
            
                          <div class="video" id="video13" style="display: none;">
            <h1 class="video-title"> Lecture 1 exercises</h1>
             <h1 class="video-title"> part 1</h1>
<iframe src="https://drive.google.com/file/d/1CSKT46MhUNa5Hd1J3dFyTfFKKncZ9cw-/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                        <h1 class="video-title"> part 2</h1>
<iframe src="https://drive.google.com/file/d/1D1fuPu2GXxOf7FiYKc9CsyPtzlLIr-X6/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                         <h1 class="video-title"> part 3</h1>
<iframe src="https://drive.google.com/file/d/11SJIHFp3YvNoOKvOcd_Y4ZVil5NkZj2y/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                        <h1 class="video-title"> part 4</h1>
<iframe src="https://drive.google.com/file/d/1kH-Fy4ZQIVwUb-9aymh9JZOHyF9P8wTO/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
           </div>

                          <div class="video" id="video14" style="display: none;">
            <h1 class="video-title"> Lecture 2 exercises</h1>
<iframe src="https://drive.google.com/file/d/1oBoK9l4K7tbDUWb-xhq7qv5-_QgeweZG/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen>
</iframe>
           </div>
                          <div class="video" id="video15" style="display: none;">
            <h1 class="video-title"> Lecture 3 exercises</h1>
<iframe src="https://drive.google.com/file/d/1E4v_fKT0zmliw0KM1is4Attl3Pr4sZOo/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen>
</iframe>
                      </div>
                      
                      <div class="video" id="video16" style="display: none;">
            <h1 class="video-title"> Lecture 4 exercises</h1>
                        <h1 class="video-title"> part 1</h1>
<iframe src="https://drive.google.com/file/d/1ezGOIbNqI314sf209HQgS1zifixZWPlP/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen>
</iframe>


                                   <h1 class="video-title"> part 2</h1>
<iframe src="https://drive.google.com/file/d/1R0ZQXkYbajlfrynBhmcxcVt7HcP_21bs/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>
                                              <h1 class="video-title"> part 3</h1>
<iframe src="https://drive.google.com/file/d/1kBFmbFj0zV4BBXqvHbVo3Xe4S2X7TzMs/preview" 
        width="640" 
        height="480" 
        allow="autoplay" 
        allowfullscreen></iframe>

                      </div>
            
                    `;
                } else if (code === 'CODE2') {
                    videoHTML = `
        <section id="videos" class="video-container">
<select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
            <option value="video0">.....option.....</option>
                <option value="video1">Faraday rule and lenz </option>
                <option value="video2">Induced emf in straight wire</option>
                <option value="video3">Mutual Induction</option>
                <option value="video4">Self induction</option>
                <option value="video5">Dynamo </option>
                <option value="video6">Transformer </option>
                <option value="video7">Motor </option>
                <option value="video8">Lecture 1 exercises</option>
                <option value="video9">Lecture 2 exercises</option>
                <option value="video10">Lecture 3 exercises</option>
                <option value="video11">Lecture 4 exercises</option>
                            </select>
            
            
            
            <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">Faraday rule and lenz</h1>
<iframe src="https://drive.google.com/file/d/1CO-KACGNBJN_B5XQjG4hymadfe2qQCuK/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video2" style="display: none;">
                <h1 class="video-title">Induced emf in straight wire</h1>
<iframe src="https://drive.google.com/file/d/1IgK0AzHmdPveba0dS6G-w3oB9KzIwtAz/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video3" style="display: none;">
                <h1 class="video-title">Mutual Induction</h1>
<iframe src="https://drive.google.com/file/d/1ZOkxgRwNktqEU01ArtPCdGPtI0_DTfhf/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video4" style="display: none;">
                <h1 class="video-title">Self induction</h1>
<iframe src="https://drive.google.com/file/d/1JBvRufHVy54Fdti4Qebfxk8FxeUEJuXd/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video5" style="display: none;">
                <h1 class="video-title">Dynamo</h1>
<iframe src="https://drive.google.com/file/d/1bNTVPDdRFlbivMj4w5Bme--D-1hmDDZB/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video6" style="display: none;">
                <h1 class="video-title">Transformer</h1>
<iframe src="https://drive.google.com/file/d/10TxqnXvRF9liW7nXWVZ9E6Jt8hlC1A1h/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video7" style="display: none;">
                <h1 class="video-title">Motor</h1>
<iframe src="https://drive.google.com/file/d/1bcCGuVSG-FFeqRpxtdbAruL3e7kUUBPY/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>
<div class="video" id="video8" style="display: none;">
                <h1 class="video-title">Lecture 1 exercises</h1>
                <h1 class="video-title">part 1</h1>
<iframe src="https://drive.google.com/file/d/1BLVKeHRyPq8fDLbcKJi0bakUYSjlJWY9/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                <h1 class="video-title">part 2</h1>
<iframe src="https://drive.google.com/file/d/1Xn6LxprOv8HdTgjeSPmvndy7KFOgK_pB/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>
<div class="video" id="video9" style="display: none;">
                <h1 class="video-title">Lecture 2 exercises</h1>
<iframe src="https://drive.google.com/file/d/1lPQUGCqKjVid1Cphn_TVEy9cBvehHCEm/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video10" style="display: none;">
                <h1 class="video-title">Lecture 3 exercises</h1>
                                <h1 class="video-title">part 1</h1>
<iframe src="https://drive.google.com/file/d/1oE4TZc0kejYkzQV_MLB7qentyafUeQ7-/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                <h1 class="video-title">part 2</h1>
<iframe src="https://drive.google.com/file/d/1-Vu8Pq-tr_u86f5VzVJkcQfAXSAP6SZw/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video11" style="display: none;">
                <h1 class="video-title">Lecture 4 exercises</h1>
<iframe src="https://drive.google.com/file/d/1HG7iTWDu2r6681Q1akj0qNzCm12k8g1X/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

                    `;
                } else if (code === 'CODE3') {
                    videoHTML = `
        <section id="videos" class="video-container">
<select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
            <option value="video0">.....option.....</option>
                <option value="video1">ch.1 part 1 </option>
                <option value="video2">ch.1 part 2</option>
                <option value="video3">ch.1 part 3</option>
                
                <option value="video4"> Ac circuits and hot wire ammeter</option>
                <option value="video5"> R-Circuit - L-Circuit </option>
                <option value="video6">Capacitor with DC and C-Circuit </option>
                <option value="video7">RL-Circuit -- RC-Circuit -- RLC-Circuit </option>
                <option value="video8">Resonance </option>
                
                <option value="video9">chapter 1 exercises</option>
                <option value="video10">chapter 2 exercises</option>
                <option value="video11">chapter 3 exercises</option>
                <option value="video12">chapter 4 exercises</option>
                            </select>
            
            
            
            <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">ch.1 part 1</h1>
<iframe src="https://drive.google.com/file/d/1QQJBGgQNp-glB5wdLCOGVkFzgk2WFQbX/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video2" style="display: none;">
                <h1 class="video-title">ch.1 part 2</h1>
<iframe src="https://drive.google.com/file/d/1QSOLviOMwU31qGRWo3MaEDddElsr6CMz/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video3" style="display: none;">
                <h1 class="video-title">ch.1 part 3</h1>
<iframe src="https://drive.google.com/file/d/1QU1WOgR8EknGyZjKeyOA9rAl3tqGVs2L/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video4" style="display: none;">
                <h1 class="video-title">Ac circuits and hot wire ammeter</h1>
<iframe src="https://drive.google.com/file/d/1kZWVO3VpIxGA8o3DLboFfOp4G5bhk8hV/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video5" style="display: none;">
                <h1 class="video-title">R-Circuit - L-Circuit</h1>
<iframe src="https://drive.google.com/file/d/1I36i38fDMn7RGNEGc6MeZUNmaAno1DJb/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video6" style="display: none;">
                <h1 class="video-title">Capacitor with DC and C-Circuit</h1>
<iframe src="https://drive.google.com/file/d/1fDzXl307Vnl8K9Oy9oVDlg8JJj0id-az/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video7" style="display: none;">
                <h1 class="video-title">RL-Circuit -- RC-Circuit -- RLC-Circuit </h1>
<iframe src="https://drive.google.com/file/d/1IX7bL_MCQziOEmEnOPJAsD3J-H6ZhHCK/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>

<div class="video" id="video8" style="display: none;">
                <h1 class="video-title">Resonance</h1>
<iframe src="https://drive.google.com/file/d/1WETnTpCniFzIjR-RVTwqY2OcjJYUOyXF/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>
            
            
<div class="video" id="video9" style="display: none;">
                <h1 class="video-title">chapter 1 exercises</h1>
                                <h1 class="video-title">part 1</h1>
<iframe src="https://drive.google.com/file/d/1wbOMR2BlUdBxKhfiJVhSjh6dNoIy0EHn/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                                <h1 class="video-title">part 2</h1>

<iframe src="https://drive.google.com/file/d/1t48dWfEsA5M3y3g-5Z1Xck6-NqzK3Uzu/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                                <h1 class="video-title">part 3</h1>

<iframe src="https://drive.google.com/file/d/1h_P1VZmz7xT7kBmIUbJLlF-xYndAMT6c/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>


<div class="video" id="video10" style="display: none;">
                <h1 class="video-title">chapter 2 exercises</h1>
                                                <h1 class="video-title">part 1</h1>

<iframe src="https://drive.google.com/file/d/1xGk3-sYF_Mt3FkIoRd8ZDaIOTAFAmzlc/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                                <h1 class="video-title">part 2</h1>

<iframe src="https://drive.google.com/file/d/14pEEKr84OvYUlJHCkVPzFCab3kcrRcno/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>

            </div>

<div class="video" id="video11" style="display: none;">
                <h1 class="video-title">chapter 3 exercises</h1>
                                                <h1 class="video-title">part 1</h1>

<iframe src="https://drive.google.com/file/d/1vqVOpiShRU6yyRWB10iQ79yUzIww-Hta/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                                <h1 class="video-title">part 2</h1>

<iframe src="https://drive.google.com/file/d/1o0lVv9qIupDqFt90zgTFZRH-ijki5CMO/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                                <h1 class="video-title">part 3</h1>

<iframe src="https://drive.google.com/file/d/1nsj2vEIktEJUWO1uqwu4aLnXPyAwx_uV/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>

            </div>

<div class="video" id="video12" style="display: none;">
                <h1 class="video-title">chapter 4 exercises</h1>
                                                <h1 class="video-title">part 1</h1>

<iframe src="https://drive.google.com/file/d/1jhY5V9jRHGLiv0o3-gFR0AW2lkTK7YTr/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
                                <h1 class="video-title">part 2</h1>

<iframe src="https://drive.google.com/file/d/1pa2lk25sEXv-alDMXsoZl7iQ9KnI_1Qp/preview" width="640" height="480" allow="autoplay" allowfullscreen></iframe>
            </div>
                    `;
                } else if (code === 'CODE4') {
                    videoHTML = `
                        <select id="videoSelector" style="padding: 10px; font-size: 16px; background-color: #3A5795; color: white; border: none;">
                            <option value="video0">.....option.....</option>
                            <option value="video1"> الفصل 5 part 1</option>
                            <option value="video2"> الفصل 5 part 2</option>
                            <option value="video3"> الفصل 5 part 3</option>
                            <option value="video4">الفصل 5 part 4 (تدريبات)</option>
                            <option value="video5">الفصل 6 part 1</option>
                            <option value="video6">الفصل 6 part 2</option>
                            <option value="video7">الفصل 6 part 3 (تدريبات)</option>
                        </select>
                                    
            <div class="video" id="video1" style="display: none;">
                <h1 class="video-title">الفصل 5 part 1</h1>
  <iframe 
    src="https://drive.google.com/file/d/1IZfE3pnggeVN-yFaRmtHHWPSyFaJWSFA/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
    </div>
 <div class="video" id="video2" style="display: none;">
                <h1 class="video-title">الفصل 5 part 2</h1>
<iframe 
    src="https://drive.google.com/file/d/12ozPmVjysD4ySqiPPe25sY70g98wR3AV/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>               
</div>
<div class="video" id="video3" style="display: none;">
        <h1 class="video-title">الفصل 5 part 3</h1>
<iframe 
    src="https://drive.google.com/file/d/1fL34DsdA_lbeMMBLshtDyM0s0eSEoKO7/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe> 
</div>
<div class="video" id="video4" style="display: none;">
                <h1 class="video-title">الفصل 5 part 4 (تدريبات)</h1>
<iframe 
    src="https://drive.google.com/file/d/19PrLNK2C4kYOG-hHt04vylfxAlsz4FgA/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>         
</div>
<div class="video" id="video5" style="display: none;">
                <h1 class="video-title">الفصل 6 part 1</h1>
<iframe 
    src="https://drive.google.com/file/d/16Gkts-ij62FF_JV5aWiWSaNruoc5PBG7/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>         
</div>
<div class="video" id="video6" style="display: none;">
                <h1 class="video-title">الفصل 6 part 2</h1>
<iframe 
    src="https://drive.google.com/file/d/19ku0XT2tw2FvnWG5UYKrdbZ98jFU8K93/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>          
</div>
<div class="video" id="video7" style="display: none;">
                <h1 class="video-title">الفصل 6 part 3 (تدريبات)</h1>
<iframe 
    src="https://drive.google.com/file/d/1AMktiCnt4ny3SdtpK4AnFlxToTxVd0hH/preview" 
    width="640" 
    height="480" 
    allow="autoplay" 
    allowfullscreen>
</iframe>
</div>
`; }
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
    'CODE1': [
         '60752', '29316', '10592', '84267', '37518', '86247', 
        '82654', '31605', '82436', '59123', '93821', '79824', '10547', '43096', 
        '27509', '94251', '94238', '71825', '60194', '63472', '68025', '94257', 
        '43712', '85213', '71489', '37486', '59184', '40958', '27936', '68047', 
        '31562', '85947', '23947', '58372', '91763', '48205', '75314', '10658', 
        '58260', '39471', '93487', '52863', '31705', '78102', '46852', '63458', 
        '19273', '91426', '60128'
    ],

    'CODE2': [
         '92777', '37501', '97485', '90990', '68199', '76459', 
        '12530', '67168', '11105', '91748', '45645', '42781', '84862', '73863', 
        '52481', '27718', '23996', '22713', '85718', '28951', '36109', '14409', 
        '11723', '84785', '96488', '10559', '58453', '62311', '53593', '32607', 
        '95387', '33866', '12346', '70725', '90673', '65499', '48656', '14890', 
        '56922', '90165', '59160', '51359', '17306', '19957', '40231', '49313', 
        '27344', '25664', '82880', '26583', '75100', '89249', '34216', '13139', 
        '41456', '99585'
    ],

    'CODE3': [
        '34584', '73742', '18701', '91648', '66935', '19744', '97598', '67813', 
        '54189', '46597', '27775', '94777', '85778', '99408', '75470', '55547', 
        '35097', '94698', '39484', '30188', '16873', '17101', '45496', '95929', 
        '66446', '71968', '90722', '23468', '43499', '13836', '76972', '28222', 
        '72148', '40881', '49777', '16113', '80035', '62141', '86937', '75875', 
        '85937', '79891', '60231', '11869', '55042', '90120', '82880', '75575', 
        '48736', '51388', '25449', '57886', '82800', '94366', '73544', '76153', 
        '49467', '50703', '73280', '76634', '54069', '58455', '47470', '24187', 
        '13327', '61063', '65643', '66278', '16506', '77537', '24942', '40267', 
        '25494', '66710', '95621', '25560', '20932', '21246', '26142', '27603', 
        '41031', '15336', '31003', '48775'
    ],
    
    'CODE4': ['52903', '79650', '67861', '72333', '25520', '32973',  '39264', '53797', '64717', '36339', '82937', '25739',   '80616', '66645', '76578', '15973', '87692', '20374',  '67678', '73631', '94004', '46798', '96293', '20751',   '62290', '48708', '59522', '11281', '78664', '40295',  '35897', '81859', '85188', '98710', '98291', '18616',   '68910', '81546', '27865', '15946', '59305', '50859']

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
