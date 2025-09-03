<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Trophy Section</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0d1117, #161b22, #0d1117);
            color: #c9d1d9;
            min-height: 100vh;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
        }
        
        header {
            text-align: center;
            margin-bottom: 30px;
            border-bottom: 1px solid #30363d;
            padding-bottom: 20px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #58a6ff;
        }
        
        .subtitle {
            color: #8b949e;
            font-size: 1.1rem;
            margin-bottom: 20px;
        }
        
        .stats-bar {
            display: flex;
            justify-content: space-around;
            background: #161b22;
            border-radius: 8px;
            padding: 15px;
            margin-bottom: 30px;
            border: 1px solid #30363d;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #3fb950;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: #8b949e;
        }
        
        .trophies-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .trophy-card {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            transition: transform 0.3s ease;
        }
        
        .trophy-card:hover {
            transform: translateY(-5px);
            border-color: #58a6ff;
        }
        
        .trophy-icon {
            width: 70px;
            height: 70px;
            background: linear-gradient(45deg, #ffd700, #ffaa00);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 15px;
            font-size: 2rem;
            color: #fff;
        }
        
        .trophy-title {
            font-size: 1.2rem;
            font-weight: bold;
            margin-bottom: 10px;
            text-align: center;
            color: #c9d1d9;
        }
        
        .trophy-description {
            font-size: 0.9rem;
            color: #8b949e;
            text-align: center;
            margin-bottom: 15px;
        }
        
        .trophy-date {
            font-size: 0.8rem;
            color: #3fb950;
            margin-top: auto;
        }
        
        .trophy-rarity {
            display: flex;
            margin-top: 10px;
        }
        
        .rarity-dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            margin: 0 2px;
            background-color: #30363d;
        }
        
        .rarity-dot.active {
            background-color: #ffd700;
        }
        
        .github-integration {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 8px;
            padding: 20px;
            margin-top: 30px;
        }
        
        .github-integration h2 {
            color: #58a6ff;
            margin-bottom: 15px;
            text-align: center;
        }
        
        .code-block {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 15px;
            overflow-x: auto;
            margin: 15px 0;
            font-family: 'Courier New', monospace;
            font-size: 0.9rem;
            color: #c9d1d9;
        }
        
        .note {
            background: #1c6b48;
            border-left: 4px solid #3fb950;
            padding: 15px;
            margin: 15px 0;
            border-radius: 4px;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .trophies-container {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            }
            
            .stats-bar {
                flex-wrap: wrap;
            }
            
            .stat {
                flex: 1 0 50%;
                margin-bottom: 15px;
            }
        }
        
        @media (max-width: 480px) {
            .trophies-container {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🏆 Achievement Gallery</h1>
            <p class="subtitle">Showcasing my developer milestones and accomplishments</p>
        </header>
        
        <div class="stats-bar">
            <div class="stat">
                <div class="stat-number">12</div>
                <div class="stat-label">Trophies</div>
            </div>
            <div class="stat">
                <div class="stat-number">5</div>
                <div class="stat-label">Gold</div>
            </div>
            <div class="stat">
                <div class="stat-number">4</div>
                <div class="stat-label">Silver</div>
            </div>
            <div class="stat">
                <div class="stat-number">3</div>
                <div class="stat-label">Bronze</div>
            </div>
        </div>
        
        <div class="trophies-container">
            <div class="trophy-card">
                <div class="trophy-icon">🥇</div>
                <h3 class="trophy-title">Flutter Expert</h3>
                <p class="trophy-description">Mastered Flutter framework and published multiple apps</p>
                <div class="trophy-date">Earned: Jan 2024</div>
                <div class="trophy-rarity">
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot"></div>
                </div>
            </div>
            
            <div class="trophy-card">
                <div class="trophy-icon">🚀</div>
                <h3 class="trophy-title">App Innovator</h3>
                <p class="trophy-description">Created an innovative mobile application with unique features</p>
                <div class="trophy-date">Earned: Mar 2024</div>
                <div class="trophy-rarity">
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot active"></div>
                </div>
            </div>
            
            <div class="trophy-card">
                <div class="trophy-icon">🎨</div>
                <h3 class="trophy-title">UI/UX Designer</h3>
                <p class="trophy-description">Designed beautiful and functional user interfaces</p>
                <div class="trophy-date">Earned: Feb 2024</div>
                <div class="trophy-rarity">
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot"></div>
                    <div class="rarity-dot"></div>
                </div>
            </div>
            
            <div class="trophy-card">
                <div class="trophy-icon">🔥</div>
                <h3 class="trophy-title">Firebase Master</h3>
                <p class="trophy-description">Integrated Firebase services in multiple projects</p>
                <div class="trophy-date">Earned: Apr 2024</div>
                <div class="trophy-rarity">
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot active"></div>
                    <div class="rarity-dot"></div>
                </div>
            </div>
        </div>
        
        <div class="github-integration">
            <h2>How to Add This to Your GitHub Profile</h2>
            
            <p class="note">Note: GitHub READMEs support limited HTML, but for best compatibility, use the Markdown version below.</p>
            
            <p>Add the following code to your README.md file:</p>
            
            <div class="code-block">
## 🏆 Trophies<br>
<br>
| Trophy | Description | Earned |<br>
| :--- | :--- | :--- |<br>
| 🥇 **Flutter Expert** | Mastered Flutter framework and published multiple apps | Jan 2024 |<br>
| 🚀 **App Innovator** | Created innovative mobile application with unique features | Mar 2024 |<br>
| 🎨 **UI/UX Designer** | Designed beautiful and functional user interfaces | Feb 2024 |<br>
| 🔥 **Firebase Master** | Integrated Firebase services in multiple projects | Apr 2024 |<br>
<br>
**Total Trophies:** 12 &nbsp;&nbsp; • &nbsp;&nbsp; **Gold:** 5 &nbsp;&nbsp; • &nbsp;&nbsp; **Silver:** 4 &nbsp;&nbsp; • &nbsp;&nbsp; **Bronze:** 3
            </div>
            
            <p>Alternatively, you can use GitHub's profile trophy feature by adding this to your README:</p>
            
            <div class="code-block">
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=nour-eldein10&theme=onedark&column=4&margin-w=15&margin-h=15" alt="Trophies" />
</p>
            </div>
        </div>
    </div>
</body>
</html>
