@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: 'Inter', sans-serif;
    background: #f5f8ff;
    color: #172033;
    line-height: 1.6;
}


/* ================= NAVBAR ================= */

.navbar {
    position: sticky;
    top: 0;
    z-index: 1000;

    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 18px 7%;

    background: rgba(10, 22, 40, 0.95);
    backdrop-filter: blur(15px);

    border-bottom: 1px solid rgba(255,255,255,0.1);
}

.logo {
    color: white;
    font-size: 22px;
    font-weight: 800;
}

.logo span {
    color: #67e8a5;
}

nav {
    display: flex;
    gap: 22px;
}

nav a {
    color: #dce7f5;
    text-decoration: none;
    font-size: 13px;
    font-weight: 500;
    transition: 0.3s;
}

nav a:hover {
    color: #67e8a5;
}


/* ================= HERO ================= */

.hero {
    min-height: 88vh;

    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 80px 10%;

    background:
        radial-gradient(circle at 80% 30%, rgba(103,232,165,0.16), transparent 30%),
        radial-gradient(circle at 20% 70%, rgba(72,149,239,0.16), transparent 30%),
        #081525;

    color: white;
}

.hero-content {
    max-width: 680px;
}

.badge {
    display: inline-block;

    padding: 8px 16px;

    border: 1px solid rgba(103,232,165,0.4);
    border-radius: 50px;

    color: #67e8a5;

    font-size: 12px;
    font-weight: 700;
    letter-spacing: 2px;

    margin-bottom: 25px;
}

.hero h1 {
    font-size: clamp(42px, 6vw, 78px);
    line-height: 1.05;

    margin-bottom: 25px;
}

.hero h1 span {
    display: block;
    color: #67e8a5;
}

.hero p {
    color: #b8c7d9;
    font-size: 18px;
    max-width: 600px;
}

.hero-buttons {
    display: flex;
    gap: 15px;
    margin-top: 35px;
}

.btn {
    padding: 14px 25px;
    border-radius: 10px;

    text-decoration: none;

    font-weight: 700;
    font-size: 14px;
}

.primary {
    background: #67e8a5;
    color: #06151b;
}

.secondary {
    border: 1px solid #65758b;
    color: white;
}

.air-card {
    width: 320px;

    padding: 45px 30px;

    text-align: center;

    background: rgba(255,255,255,0.07);

    border: 1px solid rgba(255,255,255,0.12);

    border-radius: 30px;

    backdrop-filter: blur(20px);

    box-shadow: 0 30px 70px rgba(0,0,0,0.3);
}

.cloud {
    font-size: 55px;
}

.air-card h2 {
    margin-top: 15px;
}

.aqi-number {
    font-size: 65px;
    font-weight: 800;

    color: #67e8a5;

    margin: 10px;
}

.air-card p {
    color: #9fb0c3;
}

.status {
    margin-top: 20px;

    padding: 12px;

    background: rgba(103,232,165,0.1);

    border-radius: 10px;

    color: #67e8a5;

    font-size: 12px;
}


/* ================= SECTIONS ================= */

.section {
    padding: 100px 8%;
}

.dark-section {
    background: #081525;
    color: white;
}

.light-section {
    background: #edf3fb;
}

.section-heading {
    max-width: 800px;
    margin: auto;

    text-align: center;

    margin-bottom: 60px;
}

.section-tag {
    color: #20a36a;

    font-size: 12px;
    font-weight: 800;

    letter-spacing: 2px;

    margin-bottom: 12px;
}

.dark-section .section-tag {
    color: #67e8a5;
}

.section-heading h2 {
    font-size: clamp(30px, 4vw, 48px);
    line-height: 1.2;

    margin-bottom: 18px;
}

.section-heading h2 span {
    color: #20a36a;
}

.dark-section .section-heading h2 span {
    color: #67e8a5;
}

.section-heading p:last-child {
    color: #66758a;
}

.dark-section .section-heading p:last-child {
    color: #aab9ca;
}


/* ================= STATS ================= */

.stats {
    display: grid;
    grid-template-columns: repeat(4, 1fr);

    gap: 20px;

    max-width: 1200px;

    margin: auto;
}

.stat-card {
    padding: 30px;

    background: white;

    border: 1px solid #e2e9f2;

    border-radius: 18px;

    text-align: center;

    transition: 0.3s;
}

.stat-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 50px rgba(20,50,80,0.1);
}

.icon {
    font-size: 32px;
}

.stat-card h3 {
    font-size: 30px;
    margin: 10px;
    color: #20a36a;
}

.stat-card p {
    color: #718096;
}


/* ================= PROBLEM ================= */

.problem-grid {
    max-width: 1200px;
    margin: auto;

    display: grid;

    grid-template-columns: repeat(2, 1fr);

    gap: 20px;
}

.info-card {
    padding: 35px;

    background: rgba(255,255,255,0.05);

    border: 1px solid rgba(255,255,255,0.1);

    border-radius: 20px;

    transition: 0.3s;
}

.info-card:hover {
    transform: translateY(-5px);

    border-color: #67e8a5;
}

.big-icon {
    font-size: 40px;

    margin-bottom: 15px;
}

.info-card h3 {
    margin-bottom: 10px;
}

.info-card p {
    color: #aab9ca;
}


/* ================= DATASET ================= */

.dataset-layout {
    max-width: 1100px;
    margin: auto;

    display: grid;
    grid-template-columns: 1fr 1fr;

    gap: 25px;
}

.dataset-card,
.features-card {
    padding: 35px;

    background: white;

    border-radius: 20px;

    box-shadow: 0 15px 40px rgba(30,50,80,0.07);
}

.dataset-card h3,
.features-card h3 {
    margin-bottom: 25px;
}

.data-row {
    display: flex;
    justify-content: space-between;

    padding: 15px 0;

    border-bottom: 1px solid #edf0f5;

    font-size: 14px;
}

.data-row span {
    color: #6d7b8e;
}

.data-row strong {
    color: #172033;
}

.feature-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
}

.feature-tags span {
    padding: 10px 16px;

    background: #e9f9f1;

    color: #14774d;

    border-radius: 50px;

    font-size: 13px;
    font-weight: 700;
}


/* ================= ANALYSIS ================= */

.analysis-cards {
    max-width: 1100px;
    margin: auto;

    display: grid;
    grid-template-columns: repeat(4, 1fr);

    gap: 20px;
}

.analysis-card {
    padding: 30px;

    background: white;

    border-radius: 18px;

    border: 1px solid #e0e7f0;
}

.analysis-card span {
    font-size: 30px;
}

.analysis-card h3 {
    margin: 15px 0 8px;
}

.analysis-card p {
    color: #68778b;
    font-size: 14px;
}


/* ================= PREPROCESSING ================= */

.process {
    max-width: 1100px;

    margin: auto;

    display: flex;

    align-items: center;

    justify-content: center;
}

.process-step {
    text-align: center;

    width: 200px;
}

.step-number {
    width: 55px;
    height: 55px;

    display: flex;
    justify-content: center;
    align-items: center;

    margin: auto auto 15px;

    background: #e6f8ef;

    color: #168052;

    border-radius: 50%;

    font-weight: 800;
}

.process-step h3 {
    font-size: 15px;
}

.process-step p {
    font-size: 12px;

    color: #718096;

    margin-top: 7px;
}

.process-line {
    width: 60px;
    height: 2px;

    background: #bcebd3;
}


/* ================= CHARTS ================= */

.charts-grid {
    max-width: 1200px;

    margin: auto;

    display: grid;

    grid-template-columns: repeat(2, 1fr);

    gap: 25px;
}

.chart-card {
    padding: 25px;

    background: rgba(255,255,255,0.06);

    border: 1px solid rgba(255,255,255,0.1);

    border-radius: 20px;
}

.chart-card h3 {
    margin-bottom: 20px;

    font-size: 16px;
}


/* ================= MODEL ================= */

.model-flow {
    max-width: 1200px;

    margin: auto;

    display: flex;

    align-items: center;

    justify-content: center;

    flex-wrap: wrap;

    gap: 15px;
}

.flow-box {
    width: 160px;

    min-height: 150px;

    padding: 25px 15px;

    text-align: center;

    background: white;

    border-radius: 18px;

    border: 1px solid #e1e8f0;

    box-shadow: 0 10px 30px rgba(20,50,80,0.05);
}

.flow-box span {
    font-size: 32px;
}

.flow-box h3 {
    margin: 10px 0 5px;

    font-size: 14px;
}

.flow-box p {
    font-size: 11px;

    color: #718096;
}

.forest {
    border: 2px solid #20a36a;
}

.arrow {
    font-size: 25px;

    color: #20a36a;
}

.rf-explanation {
    max-width: 900px;

    margin: 70px auto 0;

    padding: 35px;

    background: #effaf4;

    border-radius: 20px;

    border-left: 5px solid #20a36a;
}

.rf-explanation h3 {
    color: #14774d;

    margin-bottom: 12px;
}

.rf-points {
    display: grid;

    grid-template-columns: 1fr 1fr;

    gap: 10px;

    margin-top: 20px;

    color: #245e46;

    font-size: 14px;
}


/* ================= FEATURE IMPORTANCE ================= */

.feature-section {
    background:
        radial-gradient(circle at 10% 20%, #dff9eb, transparent 30%),
        #f5f8ff;
}

.importance-box {
    max-width: 1100px;

    margin: auto;

    display: grid;

    grid-template-columns: 0.8fr 1.2fr;

    gap: 40px;

    align-items: center;
}

.importance-text {
    padding: 35px;

    background: white;

    border-radius: 20px;

    box-shadow: 0 15px 40px rgba(30,50,80,0.08);
}

.star {
    font-size: 40px;
}

.importance-text h3 {
    margin: 15px 0;
}

.importance-text p {
    color: #66758a;

    margin-top: 12px;
}

.ranking {
    display: flex;

    flex-direction: column;

    gap: 18px;
}

.rank {
    display: grid;

    grid-template-columns: 40px 120px 1fr;

    align-items: center;

    gap: 10px;
}

.rank b {
    color: #20a36a;
}

.rank span {
    font-weight: 600;

    font-size: 14px;
}

.bar {
    height: 10px;

    background: #dce5ee;

    border-radius: 50px;

    overflow: hidden;
}

.bar i {
    display: block;

    height: 100%;

    background: linear-gradient(90deg, #20a36a, #67e8a5);

    border-radius: 50px;
}

.warning {
    max-width: 800px;

    margin: 30px auto 0;

    text-align: center;

    color: #bd7517;

    font-size: 13px;
}


/* ================= METRICS ================= */

.metrics {
    max-width: 1000px;

    margin: auto;

    display: grid;

    grid-template-columns: repeat(4, 1fr);

    gap: 20px;
}

.metric {
    padding: 30px;

    text-align: center;

    background: rgba(255,255,255,0.06);

    border: 1px solid rgba(255,255,255,0.1);

    border-radius: 18px;
}

.metric span {
    color: #67e8a5;

    font-weight: 800;

    font-size: 13px;
}

.metric strong {
    display: block;

    font-size: 35px;

    margin: 8px;
}

.metric p {
    color: #9fb0c3;

    font-size: 12px;
}

.metric-note {
    text-align: center;

    margin-top: 30px;

    color: #91a2b6;

    font-size: 13px;
}


/* ================= CONCLUSION ================= */

.conclusion-grid {
    max-width: 1000px;

    margin: auto;

    display: grid;

    grid-template-columns: 1fr 1fr;

    gap: 25px;
}

.conclusion-card {
    padding: 35px;

    background: white;

    border-radius: 20px;

    border: 1px solid #e2e8f0;
}

.conclusion-card h3 {
    color: #14774d;

    margin-bottom: 15px;
}

.conclusion-card p {
    color: #68778b;
}


/* ================= FOOTER ================= */

footer {
    padding: 50px 20px;

    text-align: center;

    background: #06111e;

    color: #8fa1b5;
}

.footer-logo {
    font-size: 24px;

    color: white;

    font-weight: 800;

    margin-bottom: 12px;
}

.team {
    color: #67e8a5;

    margin: 20px;
}

.copyright {
    font-size: 12px;

    color: #596b80;
}


/* ================= RESPONSIVE ================= */

@media (max-width: 1000px) {

    nav {
        display: none;
    }

    .hero {
        flex-direction: column;

        text-align: center;

        gap: 50px;
    }

    .hero p {
        margin: auto;
    }

    .stats,
    .analysis-cards {
        grid-template-columns: repeat(2, 1fr);
    }

    .dataset-layout,
    .importance-box,
    .conclusion-grid {
        grid-template-columns: 1fr;
    }

    .metrics {
        grid-template-columns: repeat(2, 1fr);
    }

    .process {
        flex-wrap: wrap;
    }

    .process-line {
        display: none;
    }
}


@media (max-width: 600px) {

    .section {
        padding: 70px 5%;
    }

    .stats,
    .analysis-cards,
    .problem-grid,
    .charts-grid,
    .metrics {
        grid-template-columns: 1fr;
    }

    .hero {
        padding: 70px 5%;
    }

    .air-card {
        width: 100%;
    }

    .rf-points {
        grid-template-columns: 1fr;
    }

    .rank {
        grid-template-columns: 30px 90px 1fr;
    }

    .model-flow {
        flex-direction: column;
    }

    .arrow {
        transform: rotate(90deg);
    }
}
