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
        .team-section {
            margin-top: 50px;
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            display: inline-block;
            width: 80%;
            max-width: 600px;
        }
        .team-members {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 20px;
        }
        .team-member {
            margin: 10px;
            text-align: center;
        }
        .team-member img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
            object-fit: cover;
        }
        .team-member p {
            font-size: 16px;
            font-weight: bold;
            margin-top: 5px;
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

    <!-- Team Section -->
    <div class="team-section">
        <h2>Meet the Team 💡</h2>
        <div class="team-members" id="team-members">
            <!-- Team members will be added dynamically using JS -->
        </div>
    </div>

    <script>
        // Team Members Data
        const team = [
            { name: "Kashvi Goyal", img: "https://via.placeholder.com/80" },
            { name: "Shivin Azad", img: "https://via.placeholder.com/80" },
            { name: "Sambhav Sehgal", img: "https://via.placeholder.com/80" },
            { name: "Shivansh Chandel", img: "https://via.placeholder.com/80" }
        ];

        // Dynamically Add Team Members to the Page
        const teamContainer = document.getElementById("team-members");

        team.forEach(member => {
            const memberDiv = document.createElement("div");
            memberDiv.classList.add("team-member");

            memberDiv.innerHTML = `
                <img src="${member.img}" alt="${member.name}">
                <p>${member.name}</p>
            `;
            
            teamContainer.appendChild(memberDiv);
        });
    </script>
</body>
</html>


