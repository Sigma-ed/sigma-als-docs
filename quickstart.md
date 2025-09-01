# Sigma-ALS Quick Start Guide

## 🚀 5-Minute Demo Setup

### For UNICEF Evaluators & Stakeholders

#### Immediate Demo Access (No Installation Required)
1. **Visit Interactive Demos**: [sigma-als-demos repository](../sigma-als-demos)
2. **Download demo files** (agriculture-mvp.html, tvet-mvp.html, math-mvp.html)
3. **Open in any modern web browser** (Chrome, Firefox, Safari, Edge)
4. **Interact with AI features** - Click buttons, type questions, test offline mode
5. **Experience multi-sector capabilities** - Switch between agricultural, TVET, and math contexts

#### Demo Features to Test
- **AI Chat Interaction**: Ask questions and receive contextual responses
- **Offline Mode Toggle**: Simulate rural connectivity challenges  
- **Teacher Oversight System**: See quality control and approval workflows
- **Mobile Responsiveness**: Resize browser window to test mobile experience
- **Cross-Sector Navigation**: Experience different educational contexts

### For Technical Implementers

#### Prerequisites Checklist
- **Python 3.8+** for backend development
- **Node.js 16+** for frontend development  
- **PostgreSQL 12+** for production database
- **Redis 6+** for caching and session management
- **Modern web browser** for testing and development

#### Backend Quick Setup (Django)
```bash
# Clone core repository
git clone https://github.com/SigmaALS-Africa/sigma-als-core.git
cd sigma-als-core

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Environment setup
cp .env.example .env
# Edit .env with your configuration

# Database setup
python manage.py migrate
python manage.py createsuperuser

# Start development server
python manage.py runserver
