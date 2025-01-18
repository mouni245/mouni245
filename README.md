<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Webpage</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #c2c2f3;
        }
        
        header {
            background-color: #6d11ef;
            color: rgb(186, 176, 176);
            padding: 1rem 2rem;
            text-align: center;
        }
        
        main {
            padding: 2rem;
        }
        
        button {
            background-color: #6200ea;
            color: white;
            border: 1;
            padding: 0.5rem 1rem;
            cursor: pointer;
            border-radius: 5px;
        }
        
        button:hover {
            background-color: #3700b3;
        }
        
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #eee;
            margin-top: 2rem;
        }
        
        img {
            width: 3%;
            height: 3%;
        }
    </style>
</head>

<body>
    <header>
        <h1>Welcome to My Basic Webpage</h1>
    </header>
    <main>
        <p>This is a simple webpage created using HTML, CSS, and JavaScript. Click the button below to see some interaction.</p>
        <button id="alertButton">Click Me!</button>
    </main>
    <footer>
        <p>You can follow me</p>
        <image src="insta.png" id="instagram-bt">
            <image src="whatspp.png" id="whatsapp-bt" width=3% height=3%>
    </footer>
    <script>
        document.getElementById('alertButton');
        addEventListener('click', function() {

            alert('I can able to create a basic page with front end tools');
        });
        const instagrambt = document.getElementById("instagram-bt");
        const whatsappbt = document.getElementById("whatsapp-bt");
        //add event listeners now
        instagrambt.addEventListener("click", () => {
            // In order to open links in a new window we have to follow this feature syntax 
            window.open("https://www.instagram.com/", "_blank");
            alert('instagram button is clicked!'); // Opens instargram in a new tab

        });
        whatsappbt.addEventListener("click", () => {
            window.open("https://web.whatsapp.com/", "_blank"); // Opens whatsapp in a new tab
        });
    </script>
</body>

</html>
