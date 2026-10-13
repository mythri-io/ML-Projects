<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>AirGuard AI | Air Quality Prediction</title>

    <link rel="stylesheet" href="style.css">

    <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
</head>

<body>

<!-- ================= NAVBAR ================= -->

<header class="navbar">

    <div class="logo">
        🌿 AirGuard <span>AI</span>
    </div>

    <nav>
        <a href="#home">Home</a>
        <a href="#problem">Problem</a>
        <a href="#dataset">Dataset</a>
        <a href="#preprocessing">Preprocessing</a>
        <a href="#eda">EDA</a>
        <a href="#model">Model</a>
        <a href="#results">Results</a>
    </nav>

</header>


<!-- ================= HERO ================= -->

<section id="home" class="hero">

    <div class="hero-content">

        <div class="badge">
            MACHINE LEARNING PROJECT
        </div>

        <h1>
            Air Quality Prediction
            <span>Using Random Forest</span>
        </h1>

        <p>
            Feature Importance Analysis for understanding the major
            factors that influence air quality.
        </p>

        <div class="hero-buttons">
            <a href="#problem" class="btn primary">
                Explore Project
            </a>

            <a href="#eda" class="btn secondary">
                View Analysis
            </a>
        </div>

    </div>

    <div class="air-card">

        <div class="cloud">☁️</div>

        <h2>Air Quality</h2>

        <div class="aqi-number">
            AI
        </div>

        <p>Machine Learning Powered</p>

        <div class="status">
            🌱 Predict • Analyze • Understand
        </div>

    </div>

</section>


<!-- ================= PROJECT OVERVIEW ================= -->

<section class="section">

    <div class="section-heading">

        <p class="section-tag">PROJECT OVERVIEW</p>

        <h2>
            Turning Environmental Data Into
            <span>Intelligent Insights</span>
        </h2>

        <p>
            Our project uses environmental and weather measurements
            to predict air quality and identify the features that
            contribute most to the prediction.
        </p>

    </div>


    <div class="stats">

        <div class="stat-card">
            <div class="icon">🌫️</div>
            <h3>6+</h3>
            <p>Pollutant Features</p>
        </div>

        <div class="stat-card">
            <div class="icon">🌡️</div>
            <h3>3+</h3>
            <p>Weather Features</p>
        </div>

        <div class="stat-card">
            <div class="icon">🌲</div>
            <h3>RF</h3>
            <p>Machine Learning Model</p>
        </div>

        <div class="stat-card">
            <div class="icon">⭐</div>
            <h3>MDI</h3>
            <p>Feature Importance</p>
        </div>

    </div>

</section>


<!-- ================= PROBLEM ================= -->

<section id="problem" class="section dark-section">

    <div class="section-heading">

        <p class="section-tag">01 — PROBLEM DEFINITION</p>

        <h2>
            Why Do We Need
            <span>Air Quality Prediction?</span>
        </h2>

    </div>


    <div class="problem-grid">

        <div class="info-card">

            <div class="big-icon">🌍</div>

            <h3>The Problem</h3>

            <p>
                Air pollution levels change because of several
                interacting environmental and weather factors.
                Monitoring pollution only after it becomes severe
                can limit the time available for action.
            </p>

        </div>


        <div class="info-card">

            <div class="big-icon">⚠️</div>

            <h3>Why It Matters</h3>

            <p>
                Poor air quality can affect public health.
                Early prediction can help people and authorities
                understand pollution conditions and respond sooner.
            </p>

        </div>


        <div class="info-card">

            <div class="big-icon">👥</div>

            <h3>Who Can Use It?</h3>

            <p>
                Students, researchers, environmental monitoring
                teams and authorities can use the system to
                understand air-quality patterns.
            </p>

        </div>


        <div class="info-card">

            <div class="big-icon">🎯</div>

            <h3>Expected Output</h3>

            <p>
                The system predicts air quality and provides a
                ranking showing which input features contribute
                most to the Random Forest prediction.
            </p>

        </div>

    </div>

</section>


<!-- ================= DATASET ================= -->

<section id="dataset" class="section">

    <div class="section-heading">

        <p class="section-tag">02 — DATASET COLLECTION</p>

        <h2>
            Understanding the
            <span>Dataset</span>
        </h2>

        <p>
            The model uses pollutant and weather measurements
            as input features.
        </p>

    </div>


    <div class="dataset-layout">

        <div class="dataset-card">

            <h3>📊 Dataset Information</h3>

            <div class="data-row">
                <span>Dataset Source</span>
                <strong>Air Quality Dataset</strong>
            </div>

            <div class="data-row">
                <span>Data Type</span>
                <strong>Environmental Sensor Data</strong>
            </div>

            <div class="data-row">
                <span>Input Type</span>
                <strong>Numerical</strong>
            </div>

            <div class="data-row">
                <span>Target</span>
                <strong>Air Quality / AQI</strong>
            </div>

            <div class="data-row">
                <span>Model</span>
                <strong>Random Forest</strong>
            </div>

        </div>


        <div class="features-card">

            <h3>🔬 Features</h3>

            <div class="feature-tags">

                <span>PM2.5</span>
                <span>PM10</span>
                <span>NO₂</span>
                <span>SO₂</span>
                <span>CO</span>
                <span>O₃</span>
                <span>Temperature</span>
                <span>Humidity</span>
                <span>Wind Speed</span>

            </div>

        </div>

    </div>

</section>


<!-- ================= DATA UNDERSTANDING ================= -->

<section class="section light-section">

    <div class="section-heading">

        <p class="section-tag">03 — DATA UNDERSTANDING</p>

        <h2>
            Explore the
            <span>Data</span>
        </h2>

    </div>


    <div class="analysis-cards">

        <div class="analysis-card">
            <span>📁</span>
            <h3>Records</h3>
            <p>Dataset records will be displayed after loading the actual dataset.</p>
        </div>

        <div class="analysis-card">
            <span>🔢</span>
            <h3>Features</h3>
            <p>Pollutant and weather measurements are used as input variables.</p>
        </div>

        <div class="analysis-card">
            <span>❓</span>
            <h3>Missing Values</h3>
            <p>Missing values should be identified before model training.</p>
        </div>

        <div class="analysis-card">
            <span>♻️</span>
            <h3>Duplicates</h3>
            <p>Duplicate records should be checked and removed where necessary.</p>
        </div>

    </div>

</section>


<!-- ================= PREPROCESSING ================= -->

<section id="preprocessing" class="section">

    <div class="section-heading">

        <p class="section-tag">04 — DATA PREPROCESSING</p>

        <h2>
            Preparing Data for
            <span>Machine Learning</span>
        </h2>

    </div>


    <div class="process">

        <div class="process-step">
            <div class="step-number">01</div>
            <h3>Missing Values</h3>
            <p>Identify and handle missing observations.</p>
        </div>

        <div class="process-line"></div>

        <div class="process-step">
            <div class="step-number">02</div>
            <h3>Duplicates</h3>
            <p>Detect and remove duplicate records.</p>
        </div>

        <div class="process-line"></div>

        <div class="process-step">
            <div class="step-number">03</div>
            <h3>Outliers</h3>
            <p>Check unusual pollutant and weather readings.</p>
        </div>

        <div class="process-line"></div>

        <div class="process-step">
            <div class="step-number">04</div>
            <h3>Feature Preparation</h3>
            <p>Prepare numerical and categorical variables.</p>
        </div>

    </div>

</section>


<!-- ================= EDA ================= -->

<section id="eda" class="section dark-section">

    <div class="section-heading">

        <p class="section-tag">05 — EXPLORATORY DATA ANALYSIS</p>

        <h2>
            Discover Patterns in
            <span>Air Quality Data</span>
        </h2>

        <p>
            Visualizations help us understand distributions,
            relationships and correlations between features.
        </p>

    </div>


    <div class="charts-grid">

        <div class="chart-card">

            <h3>📊 Feature Importance</h3>

            <canvas id="importanceChart"></canvas>

        </div>


        <div class="chart-card">

            <h3>📈 Pollution Levels</h3>

            <canvas id="pollutionChart"></canvas>

        </div>


        <div class="chart-card">

            <h3>🌡️ Weather Features</h3>

            <canvas id="weatherChart"></canvas>

        </div>


        <div class="chart-card">

            <h3>🔗 Correlation Overview</h3>

            <canvas id="correlationChart"></canvas>

        </div>

    </div>

</section>


<!-- ================= MODEL ================= -->

<section id="model" class="section">

    <div class="section-heading">

        <p class="section-tag">06 — MACHINE LEARNING MODEL</p>

        <h2>
            Random Forest
            <span>Prediction</span>
        </h2>

    </div>


    <div class="model-flow">

        <div class="flow-box">
            <span>📊</span>
            <h3>Dataset</h3>
            <p>Pollutant + weather data</p>
        </div>

        <div class="arrow">→</div>

        <div class="flow-box">
            <span>🧹</span>
            <h3>Preprocessing</h3>
            <p>Clean and prepare data</p>
        </div>

        <div class="arrow">→</div>

        <div class="flow-box">
            <span>✂️</span>
            <h3>Train / Test</h3>
            <p>Split the dataset</p>
        </div>

        <div class="arrow">→</div>

        <div class="flow-box forest">
            <span>🌲</span>
            <h3>Random Forest</h3>
            <p>Train the model</p>
        </div>

        <div class="arrow">→</div>

        <div class="flow-box">
            <span>🎯</span>
            <h3>Prediction</h3>
            <p>Predict air quality</p>
        </div>

    </div>


    <div class="rf-explanation">

        <h3>🌲 Why Random Forest?</h3>

        <p>
            Random Forest combines multiple decision trees to produce
            a more robust prediction. It is suitable for this project
            because air quality depends on several interacting and
            potentially non-linear environmental factors.
        </p>

        <div class="rf-points">

            <div>✓ Handles non-linear relationships</div>
            <div>✓ Works with noisy sensor data</div>
            <div>✓ Reduces overfitting compared with a single tree</div>
            <div>✓ Provides feature importance scores</div>

        </div>

    </div>

</section>


<!-- ================= FEATURE IMPORTANCE ================= -->

<section class="section feature-section">

    <div class="section-heading">

        <p class="section-tag">07 — FEATURE IMPORTANCE</p>

        <h2>
            Which Features Matter
            <span>Most?</span>
        </h2>

        <p>
            Random Forest can rank features according to their
            contribution to the model.
        </p>

    </div>


    <div class="importance-box">

        <div class="importance-text">

            <div class="star">⭐</div>

            <h3>Mean Decrease in Impurity</h3>

            <p>
                Feature importance measures how much each feature
                contributes to reducing impurity across the
                decision trees.
            </p>

            <p>
                Higher importance means the model relied more
                heavily on that feature.
            </p>

        </div>


        <div class="ranking">

            <div class="rank">
                <b>01</b>
                <span>PM2.5</span>
                <div class="bar"><i style="width: 90%"></i></div>
            </div>

            <div class="rank">
                <b>02</b>
                <span>PM10</span>
                <div class="bar"><i style="width: 78%"></i></div>
            </div>

            <div class="rank">
                <b>03</b>
                <span>NO₂</span>
                <div class="bar"><i style="width: 63%"></i></div>
            </div>

            <div class="rank">
                <b>04</b>
                <span>CO</span>
                <div class="bar"><i style="width: 53%"></i></div>
            </div>

            <div class="rank">
                <b>05</b>
                <span>Temperature</span>
                <div class="bar"><i style="width: 42%"></i></div>
            </div>

            <div class="rank">
                <b>06</b>
                <span>Humidity</span>
                <div class="bar"><i style="width: 30%"></i></div>
            </div>

            <div class="rank">
                <b>07</b>
                <span>Wind Speed</span>
                <div class="bar"><i style="width: 22%"></i></div>
            </div>

        </div>

    </div>

    <p class="warning">
        ⚠️ Illustrative ranking — replace with actual model results
        after training the Random Forest model.
    </p>

</section>


<!-- ================= RESULTS ================= -->

<section id="results" class="section dark-section">

    <div class="section-heading">

        <p class="section-tag">08 — MODEL EVALUATION</p>

        <h2>
            Model
            <span>Performance</span>
        </h2>

    </div>


    <div class="metrics">

        <div class="metric">
            <span>R²</span>
            <strong>--</strong>
            <p>R-squared Score</p>
        </div>

        <div class="metric">
            <span>RMSE</span>
            <strong>--</strong>
            <p>Root Mean Square Error</p>
        </div>

        <div class="metric">
            <span>MAE</span>
            <strong>--</strong>
            <p>Mean Absolute Error</p>
        </div>

        <div class="metric">
            <span>ACC</span>
            <strong>--</strong>
            <p>Accuracy</p>
        </div>

    </div>


    <p class="metric-note">
        Actual evaluation values will be added after training
        and testing the model with the final dataset.
    </p>

</section>


<!-- ================= CONCLUSION ================= -->

<section class="section conclusion">

    <div class="section-heading">

        <p class="section-tag">09 — CONCLUSION & FUTURE SCOPE</p>

        <h2>
            From Data to
            <span>Intelligent Decisions</span>
        </h2>

    </div>


    <div class="conclusion-grid">

        <div class="conclusion-card">

            <h3>✅ Conclusion</h3>

            <p>
                Random Forest can be used to predict air quality
                using pollutant and weather measurements while also
                providing an interpretable ranking of important
                features.
            </p>

        </div>


        <div class="conclusion-card">

            <h3>🔮 Future Scope</h3>

            <p>
                The system can be extended using larger datasets,
                more cities, longer time periods, advanced models
                such as XGBoost or LightGBM, and eventually a
                real-time air-quality monitoring dashboard.
            </p>

        </div>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <div class="footer-logo">
        🌿 AirGuard AI
    </div>

    <p>
        Machine Learning Project
    </p>

    <p>
        Feature Importance Analysis for Air Quality Prediction
        Using Random Forest
    </p>

    <div class="team">
        👩‍💻 Darahasini D &nbsp; | &nbsp; 👩‍💻 Mythri R
    </div>

    <p class="copyright">
        © 2026 AirGuard AI
    </p>

</footer>


<script src="script.js"></script>

</body>
</html>
