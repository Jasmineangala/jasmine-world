<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jasmine's World 💚</title>
    <link rel="preconnect" 
    href="https://fonts.googleapis.com">
<link rel="preconnect" 
href="https://fonts.gstatic.com" 
crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap" 
rel="stylesheet">
<link rel="stylesheet" 
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.1/css/all.min.css" 
integrity="sha512-5Hs3dF2AEPkpNAR7UiOHba+lRSJNeM2ECkwxUIxC1Q/FLycGTbNapWXB4tP889k5T5Ju8fs4b1P5z/iB4nMfSQ==" 
crossorigin="anonymous" 
referrerpolicy="no-referrer" />
  <link rel="stylesheet" href="styles.css"/> 
</head>
<body>
    <div id="header">
        <div class="container">
            <nav>
                <img src="images/logo.png" class="logo">
                <ul id="sidemenu">
                    <li><a href="#header">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#portfolio">Portfolio</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <i class="fa-solid fa-xmark" onclick="closemenu()"></i>
                </ul>
                <i class="fa-solid fa-bars" onclick="openmenu()"></i>
            </nav>
            <div class="header-text">
                <p>Basic programmer</p>
                <h1>Hi, I'm <span>Jassiya</span>.<br> A newbie Web Programmer.</h1>
            </div>
        </div>
    </div>
<!-----------about--------------->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="images/2.JPG">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>As a programmer, ability to understand and manage own thoughts, 
                        emotions, and behaviors is crucial for success. Self-awareness is not just
                        about introspection; it's about actively observing and analyzing
                        internal world to gain insights that can enhance coding skills, 
                        improve communication, and foster a more fulfilling career.
                        </p>

                    <div class="tab-titles">
                        <p class="tab-links" onclick="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>Basic Programing</span><br>Animation</li>
                            <li><span>Microsoft word etc.</span><br>documents</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>2019 - 2020</span><br>NC III 3D Animation Holder </li>
                            <li><span>2017 - 2018</span><br>NC II 2D Animation Holder  </li>
                            <li><span>2015 - 2016</span><br>Training of Crash IT Course</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>Current</span><br>Zamboanga Peninsula Polytechnic State Unuversity.</li>
                            <li><span>2020</span><br>Comtech Institute.</li>
                            <li><span>2015</span><br>Zamboanga National High School WEST.</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
                <a href="#learn more">Learn more.</a>
            </div>
            <div>
                <i class="fa-solid fa-crop"></i>
                <h2>Web Development</h2>
                <a href="#">Learn more.</a>
            </div>
        </div>
    </div>
</div>

<!------------portfolio-------------------->
<div id="portfolio">
    <div class="container">
        <h1 class="sub-title">My Works</h1>
        <div class="work-list">
            <div class="work">
                <ul>
                    <li><span>2023 - 2024</span><br>ZPPSU BSESS FACULTY OFFICE </li>
                    <li><span>2022 - 2023</span><br>ZPPSU PE FACULTY OFFICE </li>
                    <li><span>2017 - 2018</span><br>BFP ON JOB TRAINING  </li>
                    <li><span>2015 - 2016</span><br>Training of Crash IT Course</li>
                </ul>
                </div>
            </div>
        </div>
        <a href="#" class="btn">See more</a>
    </div>
</div>
<!----------contact----------->
<div id="contact">
    <div class="container">
        <div class="row">
            <div class="contact-left">
                <h1 class="sub-title">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i>angalajasmine0@gmail.com</p>
                <p><i class="fa-solid fa-phone"></i>09750555996</p>
                <div class="social-icons">
                    <a href="https://www.facebook.com/Jasmine Angala" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-facebook"></i></a>
                    <a href="https://www.instagram.com/Jasyy/" target="_blank" rel="noopener noreferrer"><i class="fa-brands fa-instagram"></i></a>
                <a href="images/Updated CV.pdf" download class="btn btn2">Download CV</a>
            </div>
            <div class="contact-right">
                <form name="submit-to-google-sheet">
                    <input type="text" name="Name" placeholder="Your Name" required>
                    <input type="email" name="email" placeholder="Your Email" required>
                    <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                    <button type="submit" class="btn btn2">Submit</button>
                </form>
                <span id="msg"></span>
            </div>
        </div>
    </div>
    <div class="copyright">
        <p>Copyright © Jassiya<i class="fa-solid fa-heart"></i></p>
    </div>
</div>

<script>

    var tablinks = document.getElementsByClassName("tab-links");
    var tabcontents = document.getElementsByClassName("tab-contents");

    function opentab(tabname){
        for(tablink of tablinks){
            tablink.classList.remove("active-link");
        }
        for(tabcontent of tabcontents){
            tabcontent.classList.remove("active-tab");
        }
        event.currentTarget.classList.add("active-link");
        document.getElementById(tabname).classList.add("active-tab");
    }
</script>

<script>
    var sidemenu = document.getElementById("sidemenu");

    function openmenu(){
        sidemenu.style.right = "0";
    }
    function closemenu(){
        sidemenu.style.right = "-200px";
    }
</script>
<script>
    const scriptURL = 'https://script.google.com/macros/s/AKfycbwXzwWIMiwvGHE3NOQJI8PBKguEoo39ij_PjbSLPc9Nwya_syubFtucVD0vUA_qMXoVXg/exec'
    const form = document.forms['submit-to-google-sheet']
    const msg = document.getElementById("msg")
  
    form.addEventListener('submit', e => {
      e.preventDefault()
      fetch(scriptURL, { method: 'POST', body: new FormData(form)})
        .then(response => {
            msg.innerHTML = "Message sent successfully"
            setTimeout(function(){
                msg.innerHTML = ""
            },5000)
            form.reset()
        })
        .catch(error => console.error('Error!', error.message))
    })
  </script>
</body>
</html>
