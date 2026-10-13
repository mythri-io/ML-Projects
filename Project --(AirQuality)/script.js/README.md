// ==========================================
// AIRGUARD AI - CHARTS
// ==========================================


// ---------- FEATURE IMPORTANCE ----------

const importanceCtx =
    document.getElementById("importanceChart");

new Chart(importanceCtx, {

    type: "bar",

    data: {

        labels: [
            "PM2.5",
            "PM10",
            "NO₂",
            "CO",
            "Temperature",
            "Humidity",
            "Wind Speed"
        ],

        datasets: [{
            label: "Illustrative Importance",

            data: [
                0.27,
                0.20,
                0.15,
                0.13,
                0.11,
                0.08,
                0.06
            ],

            borderWidth: 0
        }]
    },

    options: {

        responsive: true,

        plugins: {
            legend: {
                labels: {
                    color: "#dbe7f3"
                }
            }
        },

        scales: {

            x: {
                ticks: {
                    color: "#b9c7d5"
                }
            },

            y: {
                ticks: {
                    color: "#b9c7d5"
                }
            }

        }
    }

});


// ---------- POLLUTION CHART ----------

const pollutionCtx =
    document.getElementById("pollutionChart");

new Chart(pollutionCtx, {

    type: "line",

    data: {

        labels: [
            "Day 1",
            "Day 2",
            "Day 3",
            "Day 4",
            "Day 5",
            "Day 6",
            "Day 7"
        ],

        datasets: [{

            label: "Pollution Trend",

            data: [
                45,
                52,
                48,
                65,
                72,
                60,
                78
            ],

            tension: 0.4,

            fill: false,

            borderWidth: 3
        }]
    },

    options: {

        responsive: true,

        plugins: {

            legend: {
                labels: {
                    color: "#dbe7f3"
                }
            }

        },

        scales: {

            x: {
                ticks: {
                    color: "#b9c7d5"
                }
            },

            y: {
                ticks: {
                    color: "#b9c7d5"
                }
            }

        }

    }

});


// ---------- WEATHER CHART ----------

const weatherCtx =
    document.getElementById("weatherChart");

new Chart(weatherCtx, {

    type: "bar",

    data: {

        labels: [
            "Temperature",
            "Humidity",
            "Wind Speed"
        ],

        datasets: [{

            label: "Sample Values",

            data: [
                32,
                65,
                14
            ],

            borderWidth: 0
        }]

    },

    options: {

        responsive: true,

        plugins: {

            legend: {
                labels: {
                    color: "#dbe7f3"
                }
            }

        },

        scales: {

            x: {
                ticks: {
                    color: "#b9c7d5"
                }
            },

            y: {
                ticks: {
                    color: "#b9c7d5"
                }
            }

        }

    }

});


// ---------- CORRELATION CHART ----------

const correlationCtx =
    document.getElementById("correlationChart");

new Chart(correlationCtx, {

    type: "radar",

    data: {

        labels: [
            "PM2.5",
            "PM10",
            "NO₂",
            "CO",
            "O₃",
            "Temperature",
            "Humidity",
            "Wind Speed"
        ],

        datasets: [{

            label: "Sample Relationship",

            data: [
                90,
                80,
                65,
                60,
                45,
                35,
                30,
                20
            ],

            borderWidth: 2,

            pointRadius: 4
        }]

    },

    options: {

        responsive: true,

        plugins: {

            legend: {
                labels: {
                    color: "#dbe7f3"
                }
            }

        },

        scales: {

            r: {

                ticks: {
                    color: "#b9c7d5"
                },

                grid: {
                    color: "rgba(255,255,255,0.1)"
                },

                angleLines: {
                    color: "rgba(255,255,255,0.1)"
                },

                pointLabels: {
                    color: "#dbe7f3"
                }

            }

        }

    }

});


// ==========================================
// NAVBAR ACTIVE LINK
// ==========================================

const links = document.querySelectorAll("nav a");

links.forEach(link => {

    link.addEventListener("click", () => {

        links.forEach(item => {
            item.style.color = "";
        });

        link.style.color = "#67e8a5";

    });

});


// ==========================================
// PAGE LOAD MESSAGE
// ==========================================

console.log(
    "🌿 AirGuard AI loaded successfully!"
);

console.log(
    "Machine Learning Project - Air Quality Prediction"
);
