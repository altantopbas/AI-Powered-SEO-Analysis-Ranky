# Ranky - AI-Enhanced Professional SEO Analysis Platform (2026 Edition)

Ranky is an AI-powered, comprehensive SEO audit and content optimization platform built for modern web standards (2026+). It goes beyond traditional SEO tools by analyzing advanced metrics such as E-E-A-T signals, semantic search compliance, and AI content detection.

![Ranky Logo](static/logo.png) <!-- Add your logo file here if available -->

## 🚀 Key Features

### 1. AI-Powered Deep Analysis
- **Multi-Model Support:** Integrates with leading models like Google Gemini 2.0, DeepSeek R1, NVIDIA Nemotron, and Qwen via OpenRouter.
- **Content Quality Scoring:** Analyzes content based on expertise, depth, and originality.
- **AI Content Detection:** Predicts whether content is AI-generated using advanced algorithms.

### 2. Modern SEO Metrics (2026 Standards)
- **E-E-A-T Analysis:** Scoring of Experience, Expertise, Authoritativeness, and Trustworthiness signals.
- **Semantic Search Optimization:** Analysis of topic depth, lexical richness, and contextual variety.
- **User Intent Detection:** Identifies whether content is informational, navigational, commercial, or transactional.

### 3. Technical SEO Audit
- **Quick Audit:** Checks for Title, Meta Description, Heading Hierarchy (H1-H3), and Image Alt tags.
- **Performance:** Measures page load time and modern web features (Lighthouse compatible).
- **Schema & Structured Data:** Detects JSON-LD, Microdata, and FAQ schemas.

### 4. Professional Reporting & Management
- **PDF Report Generation:** Download customized, detailed analysis reports in PDF format using the ReportLab library.
- **User Dashboard:** Track analysis history and manage subscriptions.
- **Stripe Integration:** Secure payment and subscription management system.

## 🛠 Tech Stack

- **Backend:** [FastAPI](https://fastapi.tiangolo.com/) (Python)
- **Database:** SQLite (Development), PostgreSQL (Production) / SQLAlchemy ORM
- **Frontend:** Jinja2 Templates, Modern CSS (Liquid Glass Aesthetic), Vanilla JS
- **AI Integration:** OpenAI SDK (Various LLMs via OpenRouter)
- **Payment System:** Stripe API
- **Reporting:** ReportLab PDF Library
- **Deployment:** Vercel & Kubernetes compatible architecture

## 📦 Installation

Follow these steps to run the project in your local environment:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd ranky_app_2025
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   # For Windows:
   .\venv\Scripts\activate
   # For Linux/Mac:
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment variables:**
   Copy the `.env.example` file to `.env` and add your API keys:
   ```env
   # AI Service (OpenRouter)
   OPENROUTER_API_KEY=your_openrouter_key

   # Security
   SECRET_KEY=your_secret_key_here

   # Database
   DATABASE_URL=sqlite:///./ranky.db

   # Stripe Payment System
   STRIPE_SECRET_KEY=your_stripe_secret_key
   STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
   STRIPE_PRICE_ID=your_stripe_price_id
   STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
   ```

5. **Run the application:**
   ```bash
   uvicorn main:app --reload
   ```

## 📂 Project Structure

- `main.py`: Main entry point and API endpoints.
- `auth.py`: JWT-based user authentication.
- `database.py`: Database models and connection management.
- `payment.py`: Stripe payment integration logic.
- `templates/`: HTML interface files (Jinja2).
- `static/`: CSS, JavaScript, and image assets.
- `scripts/`: Maintenance and data management scripts.

## 📄 License

This project is proprietary. Unauthorized copying or distribution is prohibited.

---
*Ranky - The Future of SEO Analysis Experience*
