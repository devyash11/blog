<!doctype html5>
<html>
    <head>
        <title>
            My Blog
        </title>
    </head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link href='styles.css' rel='stylesheet'>

    <body id=body>

        <div class=navbar>
            <br>
            <span class=tab></span>
            <li>
                <a  id=homepage class=navbar-tabs href="https://ide-660f697c8b9843aeb9f29a0774523c42-8080.cs50.ws/index.html">
                     Home
                </a>
            </li>

            <span class=tab></span>
            <li>
                <a id=about class=navbar-tabs href="https://ide-660f697c8b9843aeb9f29a0774523c42-8080.cs50.ws/about.html">
                     About
                </a>
            </li>

            <span class=tab></span>
            <li>
                <a id=contact class=navbar-tabs href="https://ide-660f697c8b9843aeb9f29a0774523c42-8080.cs50.ws/contact.html">
                     Contact
                </a>
            </li>
            <span class=tab></span>
            <li>
                <a id=none class=navbar-tabs href="https://my-ambitions.000webhostapp.com">
                     Another WebPage
                </a>
            </li>
            <span class=tab></span>
            <li>
                <a class="fa" href="https://www.linkedin.com/in/patil-yash/">
                    &#xf08c;
                </a>
            </li>
            <br>
            <br>
        </div>

        <section id=sec1>
            <img src="Iron Man.jpg" id='ironman'>
            <h id=text class=text>WELCOME!</h>
        </section>

        <section id = sec2>
            <h id=blog-title>My Blog</h>
        </section>

        <section id = sec3>
            <p id=para>I'm glad you are here on my page to hear my story of life.
                My life had been chaotic lately, but it's not something to regret.
                Although I have had many mindsets of being passionate about something,
                finally, I have found my true passion; Artificial Intelligence. However,
                those different decisions gave me amazing friends and experiences. I
                don't have much to tell you about myself. There's no other way to brief
                my life any better than describing my ambitions and passions.
            </p>
        </section>

        <section>
            <img src="MIT.jpg" id=mit>
            <h3 id=text1 class=text>MIT, My first and last choice.</h3>
        </section>

        <section>
            <p id=sec4>I've never cared enough about college/university before. Now that I've
                found my passion, and the curiousity to learn new things and challenge
                myself of new adventures of AI. I, seriously, didn't know anything about
                MIT, but when I got to know, I made my mind to attend it. The problem is
                I got introduced about these things much later in my life, by the end of
                my 11th grade. Eventually, It has increased my desire to study there. I
                know you must be thinking that I said I was late, but still the desire
                increased. I told you, I love challenges, and studying at MIT seems to be
                an interesting challenge. However I'm gonna try to get there, I'm not gonna
                stop. My ambitions are no less than studying at MIT, and they're not gonna
                be dumped.</p>
        </section>

        <section class=footer>
            <h6>&#169;2021 by Yash Patil</h6>
        </section>

    </body>

    <script type=text/javascript>
        let ironman = document.getElementById("ironman");
        let mit = document.getElementById("mit");
        let sec2 = document.getElementById("sec2");
        let sec3 = document.getElementById("para");
        let text = document.getElementById("text");
        let text1 = document.getElementById("text1");
        window.addEventListener('scroll', function(){
            var value = window.scrollY;

            ironman.style.top = value * 0.35 + 'px';
            ironman.style.opacity = 1 - 0.001*value;
            text.style.top = value * 0.85 + 'px';
            sec2.style.opacity = 1 - (value - 800) * 0.0015 * (ironman.style.opacity < 0.1);
            sec3.style.opacity = 1 - (value - 800) * 0.0015 * (ironman.style.opacity < 0.1);
            mit.style.top = (value - 1420) * 0.3 * (sec3.style.opacity < 0.1) +'px';
            mit.style.opacity = 1 - (value - 1425) * 0.0015  * (sec3.style.opacity < -0.2);
            text1.style.top = (value - 1420) * 0.85 * (sec3.style.opacity < 0.95) + 'px'
        })
    </script>

</html>
