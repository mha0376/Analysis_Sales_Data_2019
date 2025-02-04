# Analysis_Sales_Data_2019

This project analyzes sales data from 2019 to identify trends and insights. While the original repository lacked a description, this README provides documentation to facilitate understanding and use.

**Dataset:** Sales Data 2019 Month Wise
**Source:** Kaggle
**Link:** https://www.kaggle.com/datasets/shivamsingh17072001/sales-data-2019-month-wise

## Features and Functionality

This project performs the following analyses on the sales data:

* **Data Cleaning and Preprocessing:**
    * Handles missing values.
    * Converts data types as needed.
    * Removes duplicate entries.
* **Feature Engineering:**
    * **Task 1: Month and Day Columns:** Creates new columns for 'Month' and 'Day' extracted from the 'Order Date' column.
    * **Task 3: City Column:** Adds a 'City' column to the dataset.
    * **Task 7: Order Date Conversion and Day Column:** Converts the 'Order Date' column to datetime format and creates a 'Day' column (e.g., Monday, Tuesday).
* **Sales Trend Analysis:**
    * **Task 2: Highest Sales Month:** Identifies the month with the highest total revenue and reports the corresponding revenue.
* **Product Performance Analysis:**
    * **Task 6: Best-Selling Product:** Identifies the product with the highest sales volume. Analyzes potential factors contributing to its popularity (e.g., price, marketing campaigns).
    * **Task 5: Frequently Purchased Products:** Identifies products that are most often purchased together (product bundling analysis).
* **Sales by Location Analysis:**
    * **Task 4: Highest Sales City:** Identifies the city with the highest sales volume.
* **Customer Analysis:**
    * **Task 8: Highest Value Customer:** Identifies the customer with the highest total purchase value.

## Technology Stack

* **Programming Language:** Python
* **Libraries/Frameworks:** pandas, NumPy, Matplotlib.
* **Data Storage:** CSV files in kaggle link (https://www.kaggle.com/datasets/shivamsingh17072001/sales-data-2019-month-wise)

## Prerequisites

To run this project and reproduce the analysis, you will need the following:

1.  **Python:** Python 3.x is required. It's highly recommended to use a virtual environment to manage project dependencies and avoid conflicts with other Python projects.

2.  **Virtual Environment (Recommended):** Creating a virtual environment is best practice. Here's how:

    *   **Create:**
        ```bash
        python3 -m venv .venv  # Creates a virtual environment named ".venv"
        ```
        (Or, if you're using `conda`: `conda create -n myenv python=3.x`)

    *   **Activate:**
        *   Linux/macOS:
            ```bash
            source .venv/bin/activate
            ```
            (Or, if using `conda`: `conda activate myenv`)
        *   Windows:
            ```bash
            .venv\Scripts\activate
            ```
            (Or, if using `conda`: `conda activate myenv`)

3.  **Required Libraries:** Install the project's dependencies using the provided `requirements.txt` file. Make sure your virtual environment is activated *before* running this command:

    ```bash
    pip install -r requirements.txt
    ```

    This will install all the necessary Python packages, including `pandas`, `matplotlib`, `scikit-learn` (and any others you've listed in `requirements.txt`), along with the correct version numbers.

4.  **Jupyter Notebook:** Ensure you have Jupyter Notebook installed. If not, you can install it using pip within your activated virtual environment:

    ```bash
    pip install notebook
    ```

    (Or, if you prefer conda: `conda install notebook`)

5.  **Data Files:** This project uses data from Kaggle. The notebook itself will download the data using the `kagglehub` library.  No manual download is required.  Just make sure you have the `kagglehub` library installed (covered in step 3). The notebook expects the data to be in the same directory as the notebook itself, or in a `dataset/` sub-directory. The notebook code should handle creating this sub-directory automatically.

    To download the data, the notebook uses the following code:

    ```python
    import kagglehub
    path = kagglehub.dataset_download("shivamsingh17072001/sales-data-2019-month-wise")
    print("Path to dataset files:", path)
    ```

    This code will download the data and print the path to the downloaded files.  The notebook should then use this `path` variable to access the data.





## Installation Instructions

1. Clone the repository: `git clone https://github.com/mha0376/Analysis_Sales_Data_2019.git`
2. Navigate to the project directory: `cd Analysis_Sales_Data_2019`
3. Create a virtual environment (recommended): `python3 -m venv venv`
4. Activate the virtual environment:
    * **Linux/macOS:** `source venv/bin/activate`
    * **Windows:** `venv\Scripts\activate`
5. Install dependencies: `pip install -r requirements.txt` (A `requirements.txt` file should be created listing all project dependencies.  This file should be added to the repository.)


## Contributing Guidelines

Contributions are welcome! Please follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Submit a pull request with a clear description of your changes.


## Contact/Support Information

For any questions or issues, please contact the repository owner directly via GitHub.
