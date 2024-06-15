---
layout: article
titles:
  # @start locale config
  en      : &EN       About me 

  en-GB   : *EN
  en-US   : *EN
  # @end locale config
key: page-about
---

<div style="background-color: black; color: #00FF00; font-family: 'Courier New', Courier, monospace; padding: 20px; border-radius: 5px; overflow: hidden; white-space: pre;">
  <pre id="terminal" style="margin: 0; line-height: 1.2;">
  /$$$$$$             /$$$$$$                                         
 /$$$_  $$           /$$__  $$                                        
| $$$$\ $$ /$$   /$$| $$  \ $$  /$$$$$$  /$$$$$$$   /$$$$$$  /$$$$$$$ 
| $$ $$ $$|  $$ /$$/|  $$$$$$/ |____  $$| $$__  $$ /$$__  $$| $$__  $$
| $$\ $$$$ \  $$$$/  >$$__  $$  /$$$$$$$| $$  \ $$| $$  \ $$| $$  \ $$
| $$ \ $$$  >$$  $$ | $$  \ $$ /$$__  $$| $$  | $$| $$  | $$| $$  | $$
|  $$$$$$/ /$$/\  $$|  $$$$$$/|  $$$$$$$| $$  | $$|  $$$$$$/| $$  | $$
 \______/ |__/  \__/ \______/  \_______/|__/  |__/ \______/ |__/  |__/
                                                                      
                                                                      
  </pre>
</div>

<script>
  document.addEventListener('DOMContentLoaded', (event) => {
    const terminal = document.getElementById('terminal');
    const messages = [
      "pico -s /bin/sh",
      "/bin/sh",
      "executing.. ",
      "root@aaronvdberg:~$ |"
    ];
    let messageIndex = 0;
    let charIndex = 0;
    const typingSpeed = 180; // typing speed in milliseconds

    function typeWriter() {
      if (messageIndex < messages.length) {
        const message = messages[messageIndex];
        if (charIndex < message.length) {
          terminal.innerHTML += message.charAt(charIndex);
          charIndex++;
          setTimeout(typeWriter, typingSpeed);
        } else {
          terminal.innerHTML += '<br>';
          messageIndex++;
          charIndex = 0;
          setTimeout(typeWriter, typingSpeed * 3); // pause after each message
        }
      }
    }

    typeWriter();
  });
</script>

## Aaron Van Den Berg

Hello! I'm Aaron Van Den Berg, a 20-year-old Computer Science undergraduate and Cyber Security club lecturer at Eduvos. I am passionate about teaching programming and contributing to the growth of the Cybersecurity scene in South Africa. Through this platform, I aim to empower individuals with the knowledge and skills needed to excel in the ever-evolving field of technology.

## What I Do

As a Cyber Security club lecturer, I focus on:
- Introducing students to the basics of programming.
- Teaching advanced cybersecurity concepts and practices.
- Organizing workshops and seminars to keep up with the latest trends in cybersecurity.
- Building a community of like-minded individuals who are passionate about technology and security.

## My Mission

My mission is to educate and inspire the next generation of programmers and cybersecurity professionals in South Africa. By sharing my knowledge and experience, I hope to create a safer and more secure digital environment for everyone.

## Join Me

If you're interested in learning more about programming or cybersecurity, feel free to reach out and join our community. Together, we can make a difference!

## Watch My Introduction

Check out this video to learn more about me and my work:

[![Watch the video](https://img.youtube.com/vi/VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=VIDEO_ID)

## Contact

You can connect with me on:
- [Twitter](https://twitter.com/0x8anon)
- [LinkedIn](https://linkedin.com/in/aaron-vanden-berg)
- [GitHub](https://github.com/aaronvandenberg)

Thank you for visiting my page!

