# Ex.08 Design of Interactive Image Gallery
## Date:

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title>
</head>
<body style="background-color: black;">
    <header style="text-align: center; background-color: #333; color: white; padding: 1rem 0;">
        <h1>Anime - NARUTO</h1>
    </header>

    <div style="white-space: nowrap; overflow-x: auto; padding: 1rem; text-align: center;">
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="./img/gallery 1.png" style="height: 200px; alt: center;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="./img/gal 2.png" style="height: 200px;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="./img/gal3.png" style="height: 200px;">
        </div>
        <div style="display: inline-block;" onclick="openModal(this)">
            <img src="./img/gal 4.png" style="height: 200px;">
        </div>
    </div>

    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%;">
    </div>

<!-- JAVASCRIPT CODE --> 
 
    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>
```

## OUTPUT:
<img width="1138" height="610" alt="Screenshot 2025-12-25 203002" src="https://github.com/user-attachments/assets/bf5a2cba-6dd7-4537-aad8-37d82649aaf9" />
<img width="1140" height="612" alt="Screenshot 2025-12-25 203018" src="https://github.com/user-attachments/assets/7923ced2-0935-47ce-b044-1c5598a53868" />



## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
