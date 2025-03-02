# Disease Prediction Web Application

This project is a Streamlit web application that predicts the likelihood of a patient having various diseases based on user-provided health data. It uses pre-trained machine learning models to make predictions for diabetes, heart disease, Parkinson's disease, lung cancer, and hypothyroidism.

## Table of Contents

-   [Features](#features)
-   [Requirements](#requirements)
-   [Installation](#installation)
-   [Usage](#usage)
-   [Models](#models)
-   [Model Creation](#model-creation)
-   [Contributing](#contributing)
-   [License](#license)

## Features

*   **Interactive User Interface:** Built with Streamlit for easy interaction.
*   **Disease Prediction:** Predicts the likelihood of diabetes, heart disease, Parkinson's disease, lung cancer, and hypothyroidism.
*   **Input Validation:** Uses number input fields to ensure valid data entry.
*   **Clear Output:** Displays the prediction result in a user-friendly manner.
*   **Customizable:** Includes options for changing the page title, icon, and background image.

## Requirements

*   Python 3.6 or higher
*   Streamlit
*   Scikit-learn
*   Pickle
*   streamlit-option-menu

## Installation

1.  **Clone the repository:**

    ```
    git clone <repository_url>
    cd <repository_directory>
    ```

2.  **Create a virtual environment (recommended):**

    ```
    python -m venv venv
    source venv/bin/activate  # On Linux/macOS
    venv\Scripts\activate  # On Windows
    ```

3.  **Install the required packages:**

    ```
    pip install -r requirements.txt
    ```

## Usage

1.  **Run the Streamlit application:**

    ```
    streamlit run app.py
    ```

    Replace `app.py` with the actual name of your main script if it's different.

2.  **Open the application in your web browser:**

    Streamlit will provide a URL (usually `http://localhost:8501`) to access the application.

3.  **Select a disease to predict from the dropdown menu.**

4.  **Enter the required health data in the input fields.** Tooltips are provided to explain each field.

5.  **Click the "Test Result" button to get the prediction.** The result will be displayed on the screen.

## Models

The application uses pre-trained machine learning models stored in `.sav` files. These files should be placed in a directory named `Models` within the main project directory.  Here's a list of the models used:

*   `diabetes_model.sav`: Diabetes prediction model
*   `heart_disease_model.sav`: Heart disease prediction model
*   `parkinsons_model.sav`: Parkinson's disease prediction model
*   `lungs_disease_model.sav`: Lung cancer prediction model
*   `Thyroid_model.sav`: Hypothyroidism prediction model

**Important:**

*   Ensure that the paths to these model files in the code (`app.py`) are correct for your local setup.  The original code uses absolute paths which are machine-specific (e.g., `C:\\Users\\akshi\\Downloads\\Medical diagnosis using AI\\Models\\diabetes_model.sav`).  **It is highly recommended to change these to relative paths** for portability.  For example, if the `Models` directory is in the same directory as `app.py`, you would change the path to `"Models/diabetes_model.sav"`.
*   The models are loaded using `pickle`.

## Model Creation

Notebooks detailing the process of creating and training the machine learning models used in this application are provided in the repository. These notebooks contain the code, data preprocessing steps, model selection, training, and evaluation procedures.  Refer to these notebooks for a comprehensive understanding of how the models were built. The models are saved as `.sav` files using the `pickle` library.

## Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with clear, descriptive messages.
4.  Test your changes thoroughly.
5.  Submit a pull request.

## License

This project is licensed under the [License](LICENSE).

