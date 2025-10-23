<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Statistics</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica Neue', sans-serif;
            background: #f8f9fa;
            padding: 60px 20px;
            min-height: 100vh;
        }

        .wrapper {
            max-width: 900px;
            margin: 0 auto;
        }

        .header {
            margin-bottom: 50px;
            text-align: center;
        }

        .header h2 {
            font-size: 28px;
            font-weight: 600;
            color: #1a1a1a;
            letter-spacing: -0.3px;
        }

        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 16px;
            margin-bottom: 48px;
        }

        .stat-box {
            background: white;
            padding: 24px 16px;
            border-radius: 8px;
            border: 1px solid #e5e7eb;
            text-align: center;
            transition: all 0.2s ease;
        }

        .stat-box:hover {
            border-color: #d1d5db;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
        }

        .stat-value {
            font-size: 32px;
            font-weight: 700;
            color: #1a1a1a;
            margin-bottom: 6px;
        }

        .stat-label {
            font-size: 12px;
            color: #6b7280;
            font-weight: 500;
            letter-spacing: 0.3px;
        }

        .section {
            background: white;
            border: 1px solid #e5e7eb;
            border-radius: 8px;
            padding: 32px;
            margin-bottom: 24px;
        }

        .section-title {
            font-size: 14px;
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 24px;
            letter-spacing: 0.3px;
            text-transform: uppercase;
        }

        .languages {
            display: flex;
            flex-direction: column;
            gap: 16px;
        }

        .language-item {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .language-label {
            font-size: 13px;
            font-weight: 500;
            color: #374151;
            min-width: 90px;
        }

        .language-bar-container {
            flex: 1;
            height: 4px;
            background: #e5e7eb;
            border-radius: 2px;
            overflow: hidden;
        }

        .language-bar {
            height: 100%;
            border-radius: 2px;
            transition: width 0.3s ease;
        }

        .bar-js { background: #f59e0b; }
        .bar-html { background: #ef4444; }
        .bar-ts { background: #3b82f6; }
        .bar-css { background: #8b5cf6; }
        .bar-scss { background: #ec4899; }

        .language-percent {
            font-size: 12px;
            color: #9ca3af;
            font-weight: 500;
            min-width: 40px;
            text-align: right;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 24px;
        }

        .info-item {
            display: flex;
            flex-direction: column;
            gap: 8px;
        }

        .info-label {
            font-size: 12px;
            color: #6b7280;
            font-weight: 500;
            letter-spacing: 0.3px;
        }

        .info-value {
            font-size: 24px;
            font-weight: 700;
            color: #1a1a1a;
        }

        @media (max-width: 640px) {
            .stats-container {
                grid-template-columns: repeat(2, 1fr);
            }

            .section {
                padding: 24px;
            }

            .stat-value {
                font-size: 24px;
            }

            .header h2 {
                font-size: 22px;
            }
        }
    </style>
</head>
<body>
    <div class="wrapper">
        <div class="header">
            <h2>GitHub Statistics</h2>
        </div>

        <div class="stats-container">
            <div class="stat-box">
                <div class="stat-value">57</div>
                <div class="stat-label">Total Stars</div>
            </div>
            <div class="stat-box">
                <div class="stat-value">140</div>
                <div class="stat-label">Commits</div>
            </div>
            <div class="stat-box">
                <div class="stat-value">4</div>
                <div class="stat-label">Pull Requests</div>
            </div>
            <div class="stat-box">
                <div class="stat-value">0</div>
                <div class="stat-label">Issues</div>
            </div>
            <div class="stat-box">
                <div class="stat-value">239</div>
                <div class="stat-label">Contributions</div>
            </div>
            <div class="stat-box">
                <div class="stat-value">2</div>
                <div class="stat-label">Current Streak</div>
            </div>
        </div>

        <div class="section">
            <div class="section-title">Most Used Languages</div>
            <div class="languages">
                <div class="language-item">
                    <div class="language-label">JavaScript</div>
                    <div class="language-bar-container">
                        <div class="language-bar bar-js" style="width: 45.06%"></div>
                    </div>
                    <div class="language-percent">45.06%</div>
                </div>
                <div class="language-item">
                    <div class="language-label">HTML</div>
                    <div class="language-bar-container">
                        <div class="language-bar bar-html" style="width: 29.90%"></div>
                    </div>
                    <div class="language-percent">29.90%</div>
                </div>
                <div class="language-item">
                    <div class="language-label">TypeScript</div>
                    <div class="language-bar-container">
                        <div class="language-bar bar-ts" style="width: 19.78%"></div>
                    </div>
                    <div class="language-percent">19.78%</div>
                </div>
                <div class="language-item">
                    <div class="language-label">CSS</div>
                    <div class="language-bar-container">
                        <div class="language-bar bar-css" style="width: 4.92%"></div>
                    </div>
                    <div class="language-percent">4.92%</div>
                </div>
                <div class="language-item">
                    <div class="language-label">SCSS</div>
                    <div class="language-bar-container">
                        <div class="language-bar bar-scss" style="width: 0.34%"></div>
                    </div>
                    <div class="language-percent">0.34%</div>
                </div>
            </div>
        </div>

        <div class="section">
            <div class="section-title">Overview</div>
            <div class="info-grid">
                <div class="info-item">
                    <div class="info-label">Followers</div>
                    <div class="info-value">16</div>
                </div>
                <div class="info-item">
                    <div class="info-label">Following</div>
                    <div class="info-value">6</div>
                </div>
                <div class="info-item">
                    <div class="info-label">Longest Streak</div>
                    <div class="info-value">7 days</div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
