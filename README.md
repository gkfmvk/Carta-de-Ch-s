# Carta-de-Ch-s
Carta de Chás
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    
  
<meta name="viewport" content="width=device-width, initial-scale=1.0">
    
 
<title>Galeria de Imagens</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 20px;
        }
        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
        }
        .gallery img {
            width: 200px;
            height: auto;
            border-radius: 5px;
        }
        input {
            margin-top: 20px;
        }
    </style>

</h
</head>
<body>

    <h1>Minha Galeria</h1>
    
   
<input type="file" id="imageUpload" accept="image/*">
    
 
<div class="gallery" id="gallery"></div>

    

<script>
 

        document.getElementById("imageU

        document.getElementById("imageUpload").addEventListener("chan

        document.getElementById("imageUpload").addEventListener("change", function(event) {
            const file = event.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const img = document.createElement("i

        document.getElementById("imageUpload").addEventListener("change", function(event) {
            const file = event.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const img = document.createElement("img");
                    img.src = e.target.result;
                    document.getElementById("gallery

        document.getElementById("imageUpload").addEventListener("change", function(event) {
            const file = event.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const img = document.createElement("img");
                    img.src = e.target.result;
                    document.getElementById("gallery").appendChild(img);
                };
                reader.readAsDataURL(file);
            }
        });
    </script>



<
</body>
</html>
