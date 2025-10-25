🛡️ Advanced Drag-and-Drop CAPTCHA

An interactive, secure, and modern CAPTCHA system implemented in ASP.NET, JSP, and PHP, featuring drag-and-drop puzzle elements. Designed to prevent bots while maintaining a smooth user experience.

✨ Features

Drag-and-Drop Interaction: Users drag puzzle pieces or icons to a target area

Cross-Platform: Implemented in ASP.NET (C#), JSP (Java), and PHP

Dynamic CAPTCHA Generation: Randomized images, positions, and puzzle pieces

Server-Side Validation: Ensures security against bots

Responsive Design: Works on desktop and mobile devices

Customizable: Puzzle size, images, complexity, and token expiration

Easy Integration: Can be added to login forms, registration forms, or any sensitive action

🧩 How It Works

Server-Side Puzzle Generation:

ASP.NET → System.Drawing generates random images and splits into pieces

JSP → BufferedImage / Servlet generates CAPTCHA puzzle

PHP → GD Library generates puzzle image with unique session token

Client-Side Drag-and-Drop:

HTML5 Drag-and-Drop API (draggable, droppable)

jQuery UI optional for easier handling

Validation:

User drags the puzzle piece to the correct target

On submit, coordinates or order are sent to server

Server validates against generated solution stored in session

🖥️ Installation
ASP.NET

Clone the repo

Open solution in Visual Studio

Run project (Ctrl+F5)

Add <div> puzzle CAPTCHA to your login or registration pages

JSP / Java

Clone the repo

Deploy to Tomcat or any Servlet container

Access via browser

Use captcha.jsp and CaptchaServlet.java for integration

PHP

Clone the repo to your web server

Ensure GD extension is enabled in php.ini

Include captcha.php in your form

Validate using validate_captcha.php

⚙️ Usage

User opens form with CAPTCHA

Drag puzzle piece to correct position

Click Submit

Server verifies solution

If correct → proceed; if incorrect → reload CAPTCHA

🔒 Security Tips

Randomize puzzle pieces and positions every load

Validate only on server-side

Use session tokens to prevent replay attacks

Optional: Set expiry time for CAPTCHA validity

🛠️ Technologies
Language / Platform	Libraries / APIs
ASP.NET (C#)	System.Drawing, HTML5 Drag-and-Drop, jQuery UI
JSP / Java	Servlet, BufferedImage, HTML5 Drag-and-Drop, jQuery UI
PHP	GD Library, HTML5 Drag-and-Drop, AJAX
🎨 Future Enhancements

Multi-layer puzzle CAPTCHA (more pieces)

AI-assisted dynamic image CAPTCHA generation

Custom animations and responsive scaling

Multi-language support for instructions

Analytics: Track failed CAPTCHA attempts

🏷️ Tags

#captcha #draganddrop #aspnet #jsp #php #security #websecurity #html5 #javascript #gdlib #jquery #visualcaptcha #botprotection
