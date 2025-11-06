# Smart Expense Tracker

A comprehensive expense tracking application built with Streamlit that helps you track, analyze, and gain insights into your spending habits.

## Features

- **Add Expenses**: Record your expenses with details like date, category, amount, payment method, and description.
- **View Expenses**: Browse and filter your expense history in a clean tabular format with sorting and export options.
- **Analytics**: Visualize your spending patterns with interactive charts and graphs.
- **AI Insights**: Get personalized spending insights and recommendations powered by OpenAI's GPT model.

## Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/expense-tracker.git
   cd expense-tracker
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_openai_api_key_here
   ```
   
   > **Note**: You can get an API key from [OpenAI's website](https://platform.openai.com/api-keys).

## Usage

1. Start the Streamlit application:
   ```bash
   streamlit run app.py
   ```

2. Open your web browser and navigate to `http://localhost:8501`

3. Start adding your expenses and exploring the analytics!

## Project Structure

```
expense-tracker/
├── .env                    # Environment variables
├── app.py                 # Main application file
├── requirements.txt       # Python dependencies
├── README.md              # This file
├── data/                  # Database and data files
│   └── expenses.db        # SQLite database
├── pages/                 # Streamlit pages
│   ├── 1_Add_Expenses.py  # Add/Edit expenses
│   ├── 2_View_Expenses.py # View and manage expenses
│   ├── 3_Analytics.py     # Data visualization
│   └── 4_AI_Insights.py   # AI-powered insights
└── utils/                 # Utility modules
    ├── __init__.py
    ├── database.py        # Database operations
    └── config.py          # Configuration settings
```

## Features in Detail

### 1. Add Expenses
- Intuitive form for adding new expenses
- Support for multiple categories and payment methods
- Option to add custom categories
- Input validation and error handling

### 2. View Expenses
- Tabular display of all expenses
- Filter by date range and category
- Sort by any column
- Export data to CSV
- Delete expenses

### 3. Analytics
- Monthly spending trends
- Category-wise spending distribution
- Payment method analysis
- Interactive charts and graphs
- Responsive design for all screen sizes

### 4. AI Insights
- Personalized spending analysis
- Anomaly detection
- Budgeting recommendations
- Chat interface for asking questions about your spending

## Customization

You can customize the application by modifying the following files:

- `utils/config.py`: Update colors, currency, and other settings
- `utils/database.py`: Modify database schema or queries
- `pages/*.py`: Customize the individual pages

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Charts powered by [Plotly](https://plotly.com/)
- AI insights powered by [OpenAI](https://openai.com/)
- Icons from [Font Awesome](https://fontawesome.com/)
