# README.md

## p²Health – IoT Healthcare Platform

A flexible, pervasive IoT ecosystem for monitoring physiological and environmental parameters with real-time physician control. Based on the IEEE research paper by Haghi et al. (2020).

---

## Overview

This project is a proof-of-concept implementation of the research paper "A Flexible and Pervasive IoT Based Healthcare Platform for Physiological and Environmental Parameters Monitoring" (Haghi et al., IEEE Internet of Things Journal 2020).

The original work proposed a wrist-worn prototype (Ubiqsense) for ambient monitoring and an IoT gateway for data collection. This implementation enhances the original by adding:

- Physician-controlled sensor activation and deactivation
- Flexible multi-vendor gateway supporting Fitbit, Garmin, and any BLE wearable
- Real-time bidirectional communication between patient and medic
- Simulated alert system for threshold-based warnings
- Complete web-based dashboard for data visualization

---

## Live Demo

**Website:** [https://iot-healthcare-platform.vercel.app/](https://iot-healthcare-platform.vercel.app/)

**Repository:** [https://github.com/kartikpandey06/iot-healthcare-platform](https://github.com/kartikpandey06/iot-healthcare-platform)

---

## Project Structure

```
iot-healthcare-platform/
├── index.html          # Complete 5-page web application
├── README.md           # Documentation
└── assets/             # (optional) images and screenshots
```

---

## Features

### 1. Dashboard (Home)
- Dual monitoring cards showing Physiological and Environmental parameters
- Physician control panel with individual sensor toggle switches
- NO2 alert simulation button for testing emergency responses
- Real-time status indicators for gateway and cloud connectivity
- Gap Analysis section comparing original paper limitations with implemented innovations

### 2. Team and Credits Page
- Student developer profiles with LinkedIn links
- Bayes Lab acknowledgment for the Paper to Prototype initiative
- GitHub repository link for source code access
- Original research paper citation with DOI

### 3. Architecture Page
- Three-tier IoT system diagram: Sensor Layer, Gateway Layer, Cloud Layer
- Complete parameters table with measurement ranges and alert thresholds
- Security badges detailing AES-128 encryption, HTTPS, and OAuth 2.0

### 4. Research Validation Page
- Three interactive charts: NO2 Spike Detection, HR vs Respiration Synchronization, and 7-Hour Sleep Monitoring
- Key metrics display showing detection latency and monitoring duration
- Laboratory validation quote from celisca, University of Rostock

### 5. Live Demo Page
- Auto-refreshing simulated sensor data updated every 3 seconds
- Emergency alert triggers for NO2 spike and high heart rate
- Real-time value updates demonstrating platform responsiveness

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Page structure and semantic markup |
| CSS3 (Flexbox and Grid) | Responsive styling and layout |
| JavaScript | Interactivity and live data simulation |
| Chart.js | Data visualization for research validation graphs |
| Font Awesome | Iconography |
| Google Fonts (DM Sans, Sora) | Typography |

---

## Parameters Monitored

### Physiological Parameters

| Parameter | Typical Range | Alert Threshold |
|-----------|---------------|-----------------|
| Heart Rate | 60-100 bpm | >120 bpm |
| Respiration Rate | 12-20 brpm | >25 brpm |
| RR Interval (HRV) | 600-1000 ms | <400 ms |
| Skin Temperature | 34-38°C | >38.5°C |
| Sleep Stages | Light / Deep / REM | <4 hours total |

### Environmental Parameters

| Parameter | Typical Range | Alert Threshold |
|-----------|---------------|-----------------|
| NO2 | 0-0.5 ppm | >1.0 ppm |
| CO | 0-9 ppm | >35 ppm |
| O3 | 0-0.07 ppm | >0.1 ppm |
| Noise Level | 30-65 dB | >85 dB |
| UV Index | 0-5 | >6 |
| Ambient Temperature | 18-28°C | >35°C |
| Humidity | 30-70% | >85% |
| Air Pressure | 970-1030 hPa | <960 hPa |

---

## Team

| Name | Role | LinkedIn |
|------|------|----------|
| Kartik Pandey | Full-Stack Developer | [linkedin.com/in/pandeykartik](https://www.linkedin.com/in/pandeykartik/) |
| Ritvik Rao | Research and IoT Specialist | [linkedin.com/in/ritvik-rao-a09a37344](https://www.linkedin.com/in/ritvik-rao-a09a37344/) |
| Advait Hadawle | UI/UX and Presentation | [linkedin.com/in/advait-hadawale-15b513380](https://www.linkedin.com/in/advait-hadawale-15b513380/) |

---


## Experimental Validation

The original research was validated at the Center for Life Science Automation (celisca), University of Rostock with the following results:

- NO2 spike detection latency: Less than 5 seconds (0 to 21.8 ppm)
- Continuous sleep monitoring: 7+ hours
- Bidirectional communication: Confirmed real-time between physician dashboard and patient gateway
- Parameters monitored simultaneously: 13

---

## Security

- AES-128 hardware encryption on sensor nodes
- HTTPS and TLS 1.3 for cloud data transmission
- OAuth 2.0 authentication for API access
- Anonymized patient data for privacy protection
- GDPR compliant data handling

---

## How to Run Locally

1. Clone the repository:
   ```
   git clone https://github.com/kartikpandey06/iot-healthcare-platform.git
   ```

2. Navigate to the project folder:
   ```
   cd iot-healthcare-platform
   ```

3. Open the index.html file in a modern web browser (Chrome, Firefox, or Edge recommended)

Alternatively, use a local development server such as Live Server in VS Code.

---

## Responsive Design

The platform is fully responsive and works on:
- Desktop computers (1920x1080 and above)
- Tablets (768x1024 and iPad resolutions)
- Mobile devices (iPhone, Android, 320px and above)

The navigation menu collapses into a hamburger menu on smaller screens, and cards reflow into single columns for optimal readability.

---

## Future Scope

- Implement AI and machine learning anomaly detection for early warning systems
- Add additional gas sensors for CO, SO2, and O3 detection
- Integrate with hospital electronic medical record (EMR) systems
- Develop multi-patient physician dashboard for clinical use
- Implement edge computing for faster local alert processing
- Replace simulated WebSocket with real-time bidirectional communication
- Add historical data export and reporting features

---

## Acknowledgments

- Bayes Lab for organizing the "Reimagine Research With AI: Paper to Prototype" initiative
- IEEE Internet of Things Journal for publishing the original research
- University of Rostock and Center for Life Science Automation (celisca) for providing the validation environment
- The research team led by M. Haghi for their foundational work

---

## License and Disclaimer

This project is for academic demonstration purposes only.

The original research paper is copyright 2020 IEEE. Personal use of this material is permitted. Republication, redistribution, or reselling requires IEEE permission.

---

## Links

| Resource | URL |
|----------|-----|
| Live Website | https://iot-healthcare-platform.vercel.app/ |
| GitHub Repository | https://github.com/kartikpandey06/iot-healthcare-platform |


---

**Project completed for Bayes Lab - Reimagine Research With AI: Paper to Prototype**
