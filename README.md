**Small Business Ledger Bot**

A streamlined Telegram bot designed for small business owners to track daily income and business expenses directly inside Telegram without complex software.

**Key Features**
* Fast logging for income and expense transactions.
* Embedded SQLite database storing complete records per user.
* Instant automated financial report calculation.
* Persistent reply keyboard interface.

**Local Setup**

1. Clone or download project files.
2. Create Python virtual environment:
   python -m venv venv
   source venv/bin/activate
3. Install dependencies:
   pip install -r requirements.txt
4. Copy env example and configure token:
   cp .env.example .env
   Set your BOT_TOKEN inside .env file.
5. Run bot:
   python main.py

**Free Deployment Options**

Option A: Render Background Worker
1. Connect your repository to Render.
2. Create a new Background Worker service.
3. Set Build Command: pip install -r requirements.txt
4. Set Start Command: python main.py
5. Add environment variable BOT_TOKEN under Environment settings.

Option B: Koyeb App
1. Deploy code from your GitHub repository.
2. Choose Worker Service mode.
3. Configure build command: pip install -r requirements.txt
4. Configure run command: python main.py
5. Set secret environment variable BOT_TOKEN.
