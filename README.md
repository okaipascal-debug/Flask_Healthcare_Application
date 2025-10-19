## Flask_Healthcare_Application


## 📋 Project Overview

This project collects and analyzes income spending data for healthcare product research. As an R and Python developer working for a data analysis company in Washington, DC, I was assigned the task of developing a survey tool for collecting participants' data. The objective was to analyze their income spending in preparation for a new product launch in the healthcare industry.

## 🚀 Quick Start Guide

### 1. First-Time Setup

```bash
# Install Python packages
pip install -r requirements.txt

# Run the web application
python app.py

# Visit http://localhost:5000 to access the survey
2. Test Data Collection
Open http://localhost:5000

Fill out the survey form

Submit several test entries

3. Process Data

# Generate sample data and CSV
python data_processing/process_data.py
4. Analyze Data

# Start Jupyter notebook
jupyter notebook

# Open analysis/data_analysis.ipynb and run all cells
📁 Project Structure
text
healthcare_survey/
├── app.py                          # Main web application
├── requirements.txt               # Python dependencies
├── templates/index.html           # Survey form
├── data_processing/
│   ├── user_class.py             # User data class
│   └── process_data.py           # Data processing
├── data/survey_data.csv          # Generated data
├── analysis/data_analysis.ipynb  # Data analysis
└── charts/                       # Generated visualizations
🎯 Features Built
✅ Web Application: Flask survey form
✅ Data Storage: MongoDB database
✅ Data Processing: Python class system
✅ Data Analysis: Jupyter notebook with charts
✅ Visualizations: Ready for PowerPoint presentations
✅ AWS Deployment: Production-ready hosting

📊 Generated Charts
Income distribution by age

Gender spending patterns

Healthcare spending analysis

Expense category breakdown

Demographic insights

Savings analysis

🛠️ Technical Implementation
Web Development with Flask
Simple webpage for data collection

Form handling with validation

Flash messages for user feedback

MongoDB integration for data persistence

Data Storage with MongoDB
User details storage (Age, Gender, Income, Expenses)

Expense categories with amounts

Timestamp tracking

Data Processing with Python
Custom "User" class for data modeling

CSV export functionality

Data transformation and analysis

Data Visualization
Comprehensive analysis in Jupyter notebooks

Matplotlib and Seaborn charts

Professional visualizations for client presentations

AWS Deployment
Elastic Beanstalk hosting

Production-ready configuration

Scalable cloud infrastructure

🔧 Installation & Setup
Prerequisites
Python 3.8+

MongoDB (local or Atlas)

Jupyter Notebook

Dependencies

Flask==2.3.3
pymongo==4.5.0
pandas==2.1.1
matplotlib==3.7.2
seaborn==0.13.0
jupyter==1.0.0
python-dotenv==1.0.0
📈 Data Collection Fields
Demographic Information
Age: Participant age (18-100)

Gender: Male, Female, Other, Prefer not to say

Financial Information
Total Monthly Income: Numeric input

Expense Categories:

Utilities

Entertainment

School Fees

Shopping

Healthcare

🔄 Workflow Process
Data Collection: Users submit data via web form

Data Storage: Information stored in MongoDB

Data Processing: Python classes process and export to CSV

Data Analysis: Jupyter notebook generates insights

Visualization: Charts created for client presentation

Deployment: Application hosted on AWS for production use

🚀 Deployment
AWS Elastic Beanstalk Deployment

# Initialize EB application
eb init healthcare-survey-app --region us-east-1

# Create environment and deploy
eb create production-env
eb deploy

# Open deployed application
eb open
Environment Variables
MONGO_URI: MongoDB connection string

SECRET_KEY: Flask secret key

PORT: Application port (default: 5000)

📊 Analysis Outputs
The project generates several key visualizations:

Income Analysis: Ages with highest income patterns

Gender Distribution: Spending patterns across genders

Healthcare Insights: Specific healthcare spending analysis

Expense Breakdown: Category-wise spending distribution

Demographic Analysis: Age and gender-based insights

🆘 Troubleshooting
Common Issues
"Port already in use"


# Change port in app.py
app.run(debug=True, host='0.0.0.0', port=5001)
"MongoDB connection failed"

Check if MongoDB is running

Verify connection string

Use sample data mode as fallback

"Template not found"

Ensure templates folder exists

Verify index.html is in templates/ directory

"Import errors"


# Reinstall requirements
pip install -r requirements.txt
Need Help?
Check all files are in correct folders

Verify Python version (3.8+)

Ensure all packages are installed

Check MongoDB connection

🎯 Testing Sequence
Test Web App: python app.py → http://localhost:5000

Submit Test Data: Fill out form 3-4 times

Process Data: python data_processing/process_data.py

Run Analysis: jupyter notebook → run all cells

Check Outputs: Verify charts in charts/ folder

📝 Sample Data Generation
If needed, create sample data using:


python create_sample_data.py
This generates 50 sample user records for testing and demonstration.

🌐 Live Deployment
The application is deployed on AWS Elastic Beanstalk and accessible at:
http://healthcare-survey-env.xyz.us-east-1.elasticbeanstalk.com

📞 Support
For technical support or questions about this project, please refer to:

The troubleshooting section above

Project documentation

AWS Elastic Beanstalk documentation

📄 License
This project was developed as part of a data analysis assignment for healthcare product research.

Developed by: Pascal Eliezer Okai
Role: R and Python Developer
Company: Data Analysis Company, Washington DC
Purpose: Healthcare product launch research and analysis
