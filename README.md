# CSV Analysis using Django 

## Project Overview

This Django-based web application allows users to upload CSV files, performs data analysis using pandas and numpy, and displays the results and visualizations on a web interface. The project is designed to provide a simple, user-friendly way to gain insights from CSV data through basic analysis and visualizations.

## Features

- **File Upload**: Users can upload CSV files through a web interface.
- **Data Analysis**: The application reads the uploaded CSV file and performs basic data analysis, including:
  - Displaying the first few rows of the data.
  - Calculating summary statistics (mean, median, standard deviation) for numerical columns.
  - Identifying and handling missing values.
- **Data Visualization**: Generates basic plots (e.g., histograms) using matplotlib or seaborn and displays them on the web page.


## Setup Instructions

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/prajwalk-1/CSV-Analysis-using-Django.git
   cd csv_analysis
   ```

2. **Create a Virtual Environment:**

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment:**

   - On Windows:

     ```bash
     venv\Scripts\activate
     ```

   - On macOS/Linux:

     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

### Database Setup

1. **Apply Migrations:**

   ```bash
   python manage.py migrate
   ```

### Running the Server

1. **Start the Django Development Server:**

   ```bash
   python manage.py runserver
   ```

2. **Open your Browser:**

   Go to `http://127.0.0.1:8000/` to access the application.

### Usage

1. **Upload a CSV File:**

   - Navigate to the home page.
   - Use the provided form to upload a CSV file.

2. **View Data Analysis Results:**

   - After uploading, the application will display:
     - The first few rows of the data.
     - Summary statistics for numerical columns.
     - Information about missing values.
     - A histogram of numerical columns.

### Project Structure

- `csv_analysis/`: Django project directory.
  - `csv_analysis/settings.py`: Project settings.
  - `csv_analysis/urls.py`: Project URL configurations.
- `analysis/`: Django app directory.
  - `templates/analysis/`: HTML templates for the app.
    - `upload.html`: Template for file upload page.
    - `result.html`: Template for displaying analysis results.
  - `forms.py`: Form definitions for file upload.
  - `urls.py`: URL configurations for the app.
  - `views.py`: View functions for handling requests and processing data.
- `requirements.txt`: Python dependencies.
- `National_Olympic_Committee_2022_medals.csv`: A sample CSV file for testing purposes.


### Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to create an issue or submit a pull request.


### Acknowledgements

This project uses the following libraries:

- [Django](https://www.djangoproject.com/)
- [pandas](https://pandas.pydata.org/)
- [numpy](https://numpy.org/)
- [matplotlib](https://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
```
