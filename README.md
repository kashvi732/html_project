# 🌟 AI-Powered Image Search Engine 🔍✨

## 📌 Description  
An intelligent **reverse image search** web app where users can upload an image, and the system finds similar images using AI-powered APIs. This project blends **computer vision, API integration, and a stunning UI** by the team **LazyDevs**.

---

## 🎨 **Live Demo Preview (HTML, CSS & JS)**  

Here’s a **customized HTML, CSS & JavaScript snippet** showcasing part of the project:  

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Image Search</title>
    <style>
        body {
            font-family: "Poppins", sans-serif;
            background: linear-gradient(120deg, #74ebd5, #acb6e5);
            text-align: center;
            padding: 40px;
        }
        h1 {
            color: #2C3E50;
            font-size: 36px;
        }
        .upload-box {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            display: inline-block;
            width: 80%;
            max-width: 500px;
        }
        input[type="file"] {
            display: none;
        }
        .upload-label {
            display: block;
            padding: 15px;
            background: #ff6f61;
            color: white;
            cursor: pointer;
            border-radius: 8px;
            font-size: 18px;
        }
        .upload-label:hover {
            background: #d84315;
        }
        .slider-container {
            margin-top: 30px;
            overflow-x: auto;
            white-space: nowrap;
            padding: 10px;
        }
        .slider-container img {
            width: 180px;
            height: 120px;
            margin: 10px;
            border-radius: 8px;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body>
    <h1>AI-Powered Image Search 🔍✨</h1>
    <div class="upload-box">
        <label for="file-upload" class="upload-label">Upload an Image</label>
        <input type="file" id="file-upload">
    </div>

    <div class="slider-container">
        <img src="https://source.unsplash.com/featured/?nature" alt="Sample Image">
        <img src="https://source.unsplash.com/featured/?city" alt="Sample Image">
        <img src="https://source.unsplash.com/featured/?technology" alt="Sample Image">
    </div>
</body>
</html>

