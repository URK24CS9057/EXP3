<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web Technology Lab - Experiment 2</title>
    <link rel="stylesheet" href="exp3.css">
</head>
<body>
    <!-- Main Container -->
    <div class="profile-container">
        <!-- Header with Background & Custom Font Styling -->
        <header class="profile-header">
            <div class="avatar-wrap">
                <img src="son.jpg" alt="Mr.mokshith" class="avatar-img">
            </div>
            <h1 class="profile-name">Mr. mokshith</h1>
        </header>
        <!-- Navigation using styled Link states and Display property -->
        <nav class="tab-navigation">
            <a href="#personal" class="tab-link">Personal</a>
            <a href="#academic" class="tab-link">Academic</a>
            <a href="#activity" class="tab-link">Activity</a>
            <a href="#others" class="tab-link">Others</a>
        </nav>
        <!-- Middle Section tracking Padding and Margins -->
        <section class="bio-section">
            <div class="bio-card">
                <p class="bio-text">
                 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent a volutpat ex, ut blandit augue. 
                    Cras malesuada consectetur leo, porta malesuada purus volutpat in.
                </p>
            </div>
        </section>
        <!-- Stack Grid testing Width & Height constraints -->
        <section class="tech-grid">
            <div class="tech-box html5-box">
                <span class="tech-title">HTML5</span>
            </div>
            <div class="tech-box css3-box">
                <span class="tech-title">CSS3</span>
            </div>
            <div class="tech-box js-box">
                <span class="tech-title">Javascript</span>
            </div>
            <div class="tech-box php-box">
                <span class="tech-title">PHP</span>
            </div>
        </section>
        <!-- Dynamic Family Information Cards -->
        <section class="family-section">
            
            <div class="family-card">
                <div class="circle-frame">
                    <img src="father.jpg" alt="Father">
                </div>
                <h3>Mr. Father's Name</h3>
                <p>It was my father who taught me to value myself. He told me that I was uncommonly beautiful and that I was the most precious thing in his life.</p>
            </div>
            <div class="family-card">
                <div class="circle-frame">
                    <img src="mother.jpg" alt="Mother">
                </div>
                <h3>Mrs. Mother's Name</h3>
                <p>My mother taught me that we all have the power to achieve our dreams.</p>
            </div>
            <div class="family-card">
                <div class="circle-frame">
                    <img src="brother.jpg" alt="Sibling">
                </div>
                <h3>Sis / Bro Name</h3>
                <p>A sister is both your mirror - and your opposite.</p>
            </div>
        </section>
    </div>
    <!-- Mandatory Uniform Academic Footer -->
    <footer class="lab-footer">
        <p><strong>Your address</strong></p>
        <p>© 2026-2032. (URK24CS9057) - Web Technology Lab Batch 1. All Rights Reserved.</p>
    </footer>
</body>
</html>

style.css

/* --- 1. Global Reset & Base Layout --- */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    /* Background Properties */
    background-color: #f5f5f5;
    background-image: url("https://transparenttextures.com");
    background-repeat: no-repeat;
    color: #333;
}

.profile-container {
    max-width: 900px;
    margin-top: 30px;
    margin-bottom: 30px;
    margin-left: auto;
    margin-right: auto;
    background-color: #ffffff;
    box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}

/* --- 2. Header & Advanced Typography Formatting --- */
.profile-header {
    background-color: #8a2be2; /* Deep purple matching sample */
    padding-top: 40px;
    padding-bottom: 20px;
    text-align: center;
}

.avatar-wrap {
    margin-bottom: 15px;
}

.avatar-img {
    width: 110px;
    height: 110px;
    border-radius: 50%;
    border: 3px solid #fff;
    object-fit: cover;
}

.profile-name {
    color: #ffffff;
    /* Font properties assignment */
    font-family: Georgia, Garamond, serif;
    font-style: normal;
    font-weight: bolder;
    font-size: 28px;
    letter-spacing: 2px;
    /* Text shadow integration */
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}

/* --- 3. Link Pseudo-classes & Display Property --- */
.tab-navigation {
    display: flex;
    background-color: #b0e0e6; /* Powder blue background tint */
}
.tab-link {
    display: block; /* Changes from inline to block layout item */
    flex: 1;
    text-align: center;
    padding-top: 12px;
    padding-bottom: 12px;
    font-family: Arial, sans-serif;
    font-weight: bold;
    font-size: 15px;
    text-decoration: none;
    transition: all 0.2s ease;
}

/* Pseudo-Class States Requirements */
.tab-link:link {
    color: #2f4f4f;
    background-color: #b0e0e6;
}
.tab-link:visited {
    color: #4b0082;
}
.tab-link:hover {
    color: #ffffff;
    background-color: #008080;
    text-decoration: underline;
}
.tab-link:active {
    background-color: #ff69b4;
    color: #fff;
}

/* --- 4. Padding & Margin Box Model Area --- */
.bio-section {
    background-color: #008080; /* Teal backdrop panel */
    /* Padding configurations */
    padding-top: 40px;
    padding-bottom: 40px;
    padding-left: 20px;
    padding-right: 20px;
    display: flex;
    justify-content: center;
}

.bio-card {
    background-color: rgba(255, 255, 255, 0.15);
    border: 2px dashed #ffffff;
    max-width: 500px;
    /* Margin usage on elements */
    margin-top: 10px;
    margin-bottom: 10px;
    padding: 25px;
}

.bio-text {
    color: #ffffff;
    font-family: 'Courier New', Courier, monospace;
    font-size: 15px;
    line-height: 1.6;
    text-align: justify;
}

/* --- 5. Height & Width Layout Configurations --- */
.tech-grid {
    display: flex;
    background-color: #e6e6e6;
    padding: 20px;
    justify-content: space-around;
    gap: 15px;
}

.tech-box {
    /* Height & Width constraints testing assignment */
    height: 120px;
    width: 22%; 
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 4px 6px rgba(0,0,0,0.15);
    transition: transform 0.2s;
}

.tech-box:hover {
    transform: translateY(-5px);
}

.html5-box { background-color: #e34c26; }
.css3-box  { background-color: #264de4; }
.js-box    { background-color: #f7df1e; }
.php-box   { background-color: #777bb4; }

.tech-title {
    color: #fff;
    font-weight: bold;
    font-size: 16px;
    font-family: Arial, sans-serif;
    letter-spacing: 1px;
}
.js-box .tech-title { color: #333; } /* dark text contrast for yellow box */

/* --- 6. Lower Grid Presentation Components --- */
.family-section {
    background: linear-gradient(135deg, #004d61 0%, #002d3a 100%);
    padding: 50px 20px;
    display: flex;
    justify-content: space-around;
    gap: 20px;
    flex-wrap: wrap;
}

.family-card {
    width: 280px;
    text-align: center;
    color: #ffffff;
}

.circle-frame {
    width: 130px;
    height: 130px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 20px;
    border-radius: 50%;
    overflow: hidden;
    border: 4px solid #70d63c;
    background-color: #fff;
}

.circle-frame img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.family-card h3 {
    font-family: Georgia, serif;
    color: #70d63c;
    font-size: 16px;
    margin-bottom: 12px;
}

.family-card p {
    font-size: 13px;
    line-height: 1.5;
    color: #cbd5e1;
    text-align: center;
}

/* --- 7. Academic Lab Footer --- */
.lab-footer {
    background-color: #fce4c8;
    padding-top: 15px;
    padding-bottom: 15px;
    padding-left: 30px;
    padding-right: 30px;
    font-family: Arial, sans-serif;
    font-size: 13px;
    color: #333;
    border-top: 1px solid #dcd3c1;
    line-height: 1.6;
}
