# Streamlit-LP2-App
This project creates a streamlit application for LP_2 Regression Project

# Title: Store Sales Prediction with GUI using ML Models

# Project Introduction:
  This project aims to develop a sales prediction model for Corporation Favorita, a prominent Ecuadorian-based grocery retailer. The goal is to create a more accurate model to predict the unit sales of thousands of items sold across various Favorita stores. To enhance the user experience, we will build a graphical user interface (GUI) using Streamlit. This GUI collects client input and utilizes machine-learning models to provide accurate sales predictions.

## Key Objectives:
 1. Develop a robust machine learning model for sales prediction: We will leverage historical sales data from Favorita to train and fine-tune our machine learning models. The objective is to build a reliable model that can effectively predict the unit sales of different items.
 2. Create a user-friendly GUI using Streamlit: To streamline the sales prediction process, we will design and implement a GUI using Streamlit. The GUI will serve as an interactive platform where clients can input relevant information, such as item details, store location, and other factors that impact sales. The interface will provide an intuitive and user-friendly experience.

3. Incorporate ML models for accurate predictions: Utilizing various machine learning algorithms such as regression, ensemble methods, or deep learning, we will train models that capture the complex relationships between sales and different factors. These models will be integrated into the GUI to generate accurate sales predictions based on user inputs.

4. Evaluate and optimize model performance: We will thoroughly evaluate the performance of our models using appropriate metrics and validation techniques. By fine-tuning the models and optimizing their parameters, we aim to achieve the highest possible prediction accuracy.
   
5. Provide actionable insights and visualizations: Alongside sales predictions, we will offer actionable insights and visualizations to help clients understand the key factors influencing sales. This will enable stakeholders to make informed decisions and implement effective strategies to improve store performance.

## Project Deliverables:
1. Machine learning model for sales prediction.
2. Streamlit-based GUI for input collection and sales predictions.
3. Comprehensive project documentation, including methodology, model architecture, and evaluation results.
4. Visualizations and insights on key factors impacting sales.

# Project Structure 

Project/
├── app.py
├── predict_page.py
├── data/
│   ├── test.csv
│   └── train.csv
├── models/
│   └── store_sales-regressors.pkl
├── README.md
└── requirements.txt

This project structure provides a clear organization of files and directories, separating the main application files (app.py and predict_page.py), the data files (train.csv and test.csv), the trained model (store_sales-regressors.pkl), and other essential project documentation files (README.md and requirements.txt).
1.	App.py: This is the main file for running the Streamlit application. It serves as the entry point and orchestrates the different components of the application, including loading the trained model, handling user inputs, and displaying the results.
2.	Predict_page.py: This file contains the code for the specific page or module of the Streamlit application responsible for accepting user inputs and generating sales predictions based on those inputs. It defines the user interface elements, input fields, buttons, and any necessary data transformations or calculations.
3.	Data/: This directory stores the input data required for training and testing the sales prediction model. It includes two CSV files: train.csv (containing the training dataset) and test.csv (containing the testing dataset). These files contain relevant information about items, stores, and sales figures.
4.	Models/: This directory holds the serialized trained model or models. In this case, it contains the store_sales-regressors.pkl file is a pickled version of the trained regressor model used for sales prediction. This file can be loaded by the application to make predictions based on user inputs.
5.	README.md: This file provides documentation and instructions for the project. It typically includes an overview of the project, installation instructions, usage guidelines, and any other relevant information for developers or users.
6.	Requirements.txt: This file lists the Python libraries and dependencies required to run the project. It ensures that anyone setting up the project can easily install the necessary packages by running pip install -r requirements.txt.

# Technical Content
## App.py:
	This file serves as the entry point for the Streamlit application.
	It is responsible for loading the trained model, handling user inputs, and displaying the results.
	In the technical implementation, you would import the necessary libraries and modules, such as pandas, scikit-learn, and Streamlit.
	Within app.py, you would define the necessary functions to load the trained model from the models/ directory.
	You would also define the user interface elements using Streamlit, such as text inputs, dropdowns, and buttons, to collect user inputs.
	When the user submits the inputs, the application would pass them to the relevant functions for preprocessing and prediction using the trained model.
	Finally, the application would display the predicted sales results back to the user.
## Predict_page.py:
	This file represents a specific page or module of the Streamlit application.
	It is responsible for handling user inputs and generating sales predictions based on those inputs.
	In the technical implementation, you would define a class or functions within predict_page.py to encapsulate the logic for user input processing and prediction.
	The class or functions would take the user inputs as arguments, perform any necessary data transformations or calculations, and then utilize the trained model to make predictions.
	The predicted sales results would be returned back to app.py for displaying to the user.
## Data/:
	This directory stores the input data required for training and testing the sales prediction model.
	In the technical implementation, you would place the train.csv and test.csv files within the data/ directory.
	These files would typically be read using libraries such as pandas, and the data would be loaded into data structures like dataframes for further processing and model training.
## Models/:
	This directory contains the serialized trained model or models.
	In the technical implementation, you would save the trained regressor model as a serialized file, such as store_sales-regressors.pkl, using libraries like Python's pickle.
	When app.py loads the model, it would use the corresponding library to deserialize the model from the store_sales-regressors.pkl file.
	This deserialized model would be used for making predictions based on user inputs.
## README.md:
	This file provides documentation and instructions for the project.
	In the technical implementation, you would write the necessary project information, including an overview of the project, installation instructions, usage guidelines, and any other relevant information.
	The README.md file would typically be written in Markdown format, allowing you to include headings, lists, code snippets, and other formatting elements to make the documentation more readable and organized.
## Requirements.txt:
	This file lists the Python libraries and dependencies required to run the project.
	In the technical implementation, you would specify the required libraries and their versions within the requirements.txt file.
	Each library and version would be listed on a separate line, allowing others to easily install the necessary packages by running pip install -r requirements.txt.
	This ensures that anyone setting up the project has the same environment with the required dependencies.
## Conclusion
In conclusion, the project aimed to develop a more accurate sales prediction model for Corporation Favorita, a prominent Ecuadorian-based grocery retailer. The goal was to predict the unit sales of thousands of items sold across various Favorita stores. To enhance the user experience, a graphical user interface (GUI) was built using Streamlit, allowing clients to input their preferences and obtain accurate sales predictions.
The project structure provided a clear organization of files and directories, ensuring an efficient development process. The main application files, `app.py` and `predict_page.py`, served as the core components of the Streamlit application. These files were responsible for loading the trained model, handling user inputs, and displaying the predicted sales results.
The data files, `train.csv` and `test.csv`, contained historical sales data, including item details, store information, and corresponding sales figures. These datasets were utilized for training and evaluating the sales prediction model.
The trained model, stored as `store_sales-regressors.pkl`, was serialized and saved within the `models/` directory. This model was crucial for making accurate sales predictions based on user inputs.
Furthermore, the project documentation files, `README.md` and `requirements.txt`, provided essential information and instructions for developers and users. The README.md file included an overview of the project, installation guidelines, usage instructions, and any other relevant details. The requirements.txt file listed the necessary Python libraries and dependencies to run the project.
Through the development process, several machine learning models were explored and evaluated to create a robust and accurate sales prediction model. The model was trained using the historical sales data and relevant features such as item attributes, store characteristics, time-related factors, promotions, and holidays.
By leveraging the graphical user interface built with Streamlit, clients could easily provide their preferences and obtain accurate sales predictions. The GUI streamlined the user experience and made it more intuitive and accessible.
While the project successfully achieved the goal of developing a sales prediction model and a user-friendly GUI, it's important to note that certain challenges and limitations were encountered. These may have included data quality issues, feature engineering complexities, model selection, and the need for continuous updates to adapt to evolving sales patterns.
In conclusion, this project has made significant strides in enhancing sales prediction accuracy for Corporation Favorita. The developed model and the Streamlit-based GUI provide a valuable tool for stakeholders to make informed decisions, optimize inventory management, and improve overall business operations.
# Appreciation
I highly recommend Azubi Africa for their comprehensive and effective programs.



