<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Credits</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="credits-container">
        <div class="credits">
            <h1>Project Team</h1>
            <ul>
                <li>John Doe - Lead Developer</li>
                <li>Jane Smith - Designer</li>
                <li>Robert Brown - Backend Engineer</li>
                <li>Alice White - Frontend Developer</li>
                <li>Chris Green - DevOps Engineer</li>
                <li>Emma Black - QA Specialist</li>
                <li>Lucas Gray - Data Scientist</li>
                <li>Rachel Blue - Product Manager</li>
                <li>Michael Silver - UX Researcher</li>
                <li>Olivia Gold - Copywriter</li>
            </ul>
        </div>
    </div>
<style>
body {
    background-color: black;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
    overflow: hidden;
}

.credits-container {
    width: 80%;
    height: 100%;
    overflow: hidden;
    display: flex;
    align-items: flex-end;
}

.credits {
    text-align: center;
    color: white;
    font-family: Arial, sans-serif;
    font-size: 1.5rem;
    line-height: 2;
    animation: scroll-up 20s linear infinite;
}

.credits h1 {
    margin-bottom: 2rem;
    font-size: 2.5rem;
}

@keyframes scroll-up {
    0% {
        transform: translateY(100%);
    }
    100% {
        transform: translateY(-100%);
    }
}

        
</style>
</body>
</html>



