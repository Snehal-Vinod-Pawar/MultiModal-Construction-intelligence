# MultiModal-Construction-intelligence

An AI-powered construction intelligence platform that combines multimodal image analysis, project planning, real estate valuation, construction guidance, and weather-aware recommendations in a single web application.

## Live Demo

**Live Application:** https://multimodal-construction-intelligence.onrender.com/

## Overview

The **Multimodal Construction Intelligence Platform** is an AI-powered web application designed to assist construction professionals, site engineers, and property stakeholders with preliminary construction assessments and decision support.

The platform enables users to upload construction site images, explore AI-generated construction insights, obtain project planning suggestions, estimate property values, and access weather-aware recommendations through an interactive web interface.

## Screenshots
<img width="1917" height="892" alt="Screenshot 2026-10-26 000403" src="https://github.com/user-attachments/assets/8a0b5370-2a61-42bb-82b7-a1685dce80ac" />

<img width="1871" height="898" alt="Screenshot 2026-10-26 000438" src="https://github.com/user-attachments/assets/b46f2838-f289-40c0-a5c6-c6471e6e299f" />

## Key Features

- **Site Safety Review:** Analyze construction site images for potential safety concerns.
- **Crack and Surface Review:** Examine visible cracks and surface conditions for preliminary assessment.
- **Real Estate Valuation:** Generate indicative property valuation estimates based on user-provided information.
- **Project Planning:** Obtain AI-generated construction planning suggestions.
- **Construction Assistant:** Ask construction-related questions and receive AI-generated guidance.
- **Weather-Aware Advisory:** Access weather information and recommendations using external weather data.
- **Interactive Web Interface:** Submit requests and view AI-generated results through a web-based application.

## Technology Stack

- **Backend:** Python, FastAPI, Uvicorn
- **AI Integration:** Google Gemini API
- **Frontend:** HTML, JavaScript, React, Babel
- **Image Processing:** Pillow (PIL)
- **Weather Data:** Open-Meteo API
- **Deployment:** Docker, Render
- **Version Control:** Git, GitHub

## Architecture

The application uses a FastAPI backend to handle user requests, process uploaded images, and communicate with the Gemini API. The frontend provides an interactive interface for users to select workflows, submit information, and view generated results.

Weather-related recommendations use external weather data where applicable. The application is containerized with Docker and deployed on Render.

## Getting Started

### Prerequisites

- Python 3.11 or a compatible version
- Git
- A Google Gemini API key

### 1. Clone the Repository

```bash
git clone https://github.com/Snehal-Vinod-Pawar/MultiModal-Construction-intelligence.git
cd MultiModal-Construction-intelligence
```

### 2. Create a Virtual Environment

**Windows PowerShell:**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**Linux/macOS:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the project root and add your Gemini API key:

```env
GEMINI_API_KEY=your_gemini_api_key
GEMINI_MODEL=gemini-2.5-flash
```

Obtain an API key from [Google AI Studio](https://aistudio.google.com/).

**Important:** Never commit `.env` files, API keys, or other sensitive credentials to GitHub.

### 5. Run the Application

```bash
uvicorn app.main:app --reload
```

Open the application in your browser:

http://127.0.0.1:8000/

Interactive API documentation:

http://127.0.0.1:8000/docs

### 6. Health Check

The application provides a health endpoint at:

`/api/health`

For the deployed application, visit:

https://multimodal-construction-intelligence.onrender.com/api/health

## Deployment

The project is deployed on Render and uses environment variables to configure external AI services.

To deploy your own instance:

1. Import the GitHub repository into Render.
2. Configure the service using the repository's Dockerfile.
3. Add `GEMINI_API_KEY` to the service's environment variables.
4. Deploy the application.
5. Verify the deployment using the health endpoint.

## Limitations and Responsible Use

- AI-generated assessments may be incomplete or inaccurate.
- Image-based observations are preliminary and cannot replace professional site inspections.
- Property valuations are indicative estimates, not certified appraisals.
- Safety-related outputs should be verified by qualified construction and safety professionals.
- Application functionality depends on external API availability, network connectivity, and deployment resources.

This platform is intended for informational and decision-support purposes. It is not a substitute for professional engineering judgment, certified property appraisals, or regulatory compliance checks.

## Future Enhancements

- Advanced multimodal analysis of construction images and documents.
- Integration with construction project management systems.
- Improved cost estimation and material planning.
- Historical project data and construction progress tracking.
- Enhanced reporting and data visualization.

## Author

**Snehal Vinod Pawar**

B.Tech Computer Science and Engineering  
Medi-Caps University, Indore

**GitHub:** https://github.com/Snehal-Vinod-Pawar

## Acknowledgements

- [Google AI Studio](https://aistudio.google.com/) for Gemini API access.
- [Open-Meteo](https://open-meteo.com/) for weather data.
- [FastAPI](https://fastapi.tiangolo.com/) for backend API development.
- [Render](https://render.com/) for cloud deployment.

Built to explore AI-assisted construction intelligence through multimodal image analysis, backend API development, and cloud deployment.
