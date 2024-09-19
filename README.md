# Dream Cricket League 
## Dream - 11 wants to launch a Dream Cricket League in India.

## **Project O
overview**

This project focuses on creating balanced teams for Dream-11's upcoming Dream Cricket League, featuring players from IPL seasons 1-9. The goal is to form 5 teams, each consisting of 5 batsmen, 5 bowlers, and 1 wicketkeeper, based on a comprehensive data analysis of player performances across different IPL seasons.

## Collaborators
-[Mohammad Asif](https://github.com/mohammadasifa)
-[Gayatri Tumsare](https://github.com/GayatriTumsare)
-[Saswat NAyak](https://github.com/Saswat132002)
-[Anbuselvan A](https://github.com/Anbu-selvan-2001)

## **Data**
The data used in this project consists of 20 tables of records from IPL seasons 1-9 

![Dataset_Diagram](https://github.com/user-attachments/assets/fea52f86-0b84-40f8-8d50-c61f3935d5da)

## Key Objective 
Perform EDA on this dataset and find relevant insights that will support the above business problem.
- The analysis identified top-performing players from IPL seasons 1-9, focusing on metrics like total runs, strike rates for batsmen, wickets, and economy rates for bowlers.
- Top 5 Teams
- Teams were balanced based on performance consistency, ensuring a fair and competitive Dream Cricket League.
- Match details
- Player statistics

## **Installation**
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Dream-Cricket-League.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd Dream-Cricket-League
   ```
3. **Install the required Python packages:**
   ```bash
   pip install -r requirements.txt
   ```

## **Usage**
- Open the Jupyter notebooks in the `notebooks/` directory to explore the data analysis and team formation process.
- Run the notebooks to reproduce the analysis and insights.

## **Future Work**
- Extend the analysis to include predictive models for player performance in upcoming matches.
- Refine team selections based on real-time data and machine learning models.


This properly-formatted README file is ready for use in your GitHub repository. You can replace the placeholder GitHub link with your actual repository URL.
# App_Archers_011
Here's the README in a properly formatted markdown:

---

# **Dream Cricket League Team Formation - IPL Data Analysis**

## **Project Overview**
This project focuses on creating balanced teams for Dream-11's upcoming Dream Cricket League, featuring players from IPL seasons 1-9. The goal is to form 5 teams, each consisting of 5 batsmen, 5 bowlers, and 1 wicketkeeper, based on a comprehensive data analysis of player performances across different IPL seasons.

## **Table of Contents**
- [Project Overview](#project-overview)
- [Data](#data)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Key Insights](#key-insights)
- [Future Work](#future-work)
- [Contributors](#contributors)
- [License](#license)

## **Data**
The data used in this project consists of ball-by-ball records from IPL seasons 1-9. The dataset includes:
- Match details
- Player statistics
- Ball-by-ball information

## **Project Structure**
```plaintext
.
├── data/                   # Raw data files (not included in the repo)
├── notebooks/              # Jupyter notebooks for data analysis
│   ├── Project_IPL_(EDA)   # Initial analysis notebook, Comprehensive analysis and team formation and Exploratory Data Analysis notebook      
├── scripts/                # Scripts for data processing and analysis
├── README.md               # Project README file
```

## **Exploratory Data Analysis**
1. **Getting the Dataset from zip file**
   ```bash# Define the path
   zip_path = "C:/Users/ASUS/Desktop/Project IPL/IPL_2016.zip"
   extraction_dir = "C:/Users/ASUS/Desktop/Project IPL/IPL_files/"
   
   # Creating a dictionary to extract the files
   os.makedirs(extraction_dir, exist_ok = True)
   
   # Extract the zip file
   with zipfile.ZipFile(zip_path, 'r') as zip_ref:
       zip_ref.extractall(extraction_dir)
   
   # List of files in the directory
   extracted_files = os.listdir(extraction_dir)
   print(f"File Name:\n{extracted_files}")
   ```
2. **Data Cleaning and Data Trasformation**
   ```bash
   for name, df in dataframes.items():
    print(f"\nMissing values in {name}:")
    print(df.isnull().sum())
    # Drop rows with missing values (example approach)
    df.dropna(inplace=True)
    dataframes[name] = df

   for name, df in dataframes.items():
    print(f"\nDuplicates in {name}: {df.duplicated().sum()}")
    df.drop_duplicates(inplace=True)
    dataframes[name] = df
   ```
3. **Saved the cleaned File**
   ```bash
   # Directory where the cleaned CSV files will be saved
   cleaned_dir = "C:/Users/ASUS/Desktop/Project IPL/IPL_2016/IPL_clean_files"
   # cleaned_dir = '/Users/saswatranjannayak/Desktop/ASE204 Project/IPL_2016/clean'
   
   # Create the directory if it doesn't exist
   os.makedirs(cleaned_dir, exist_ok=True)
   
   # Save each cleaned DataFrame to a CSV file
   for name, df in dataframes.items():
       cleaned_file_path = os.path.join(cleaned_dir, f'IPL_{name}.csv')
       df.to_csv(cleaned_file_path, index=False)
       print(f'Saved {name} to {cleaned_file_path}')
   ```

## **Key Insights**
- The analysis identified top-performing players from IPL seasons 1-9
- Teams were balanced based on performance consistency, ensuring a fair and competitive Dream Cricket League.

 ![image](https://github.com/user-attachments/assets/a824b77e-7213-400f-b6b1-41e7f0531373)

![image](https://github.com/user-attachments/assets/add97432-1ef1-4432-b698-ec7d7fa04f2c)

![image](https://github.com/user-attachments/assets/a798c522-5127-4f45-8e45-dd3b0c1449f0)

![image](https://github.com/user-attachments/assets/86782dc7-f73d-461d-9c43-54768e6049c7)

## **Future Work**
- Extend the analysis to include predictive models for player performance in upcoming matches.
- Refine team selections based on real-time data and machine learning models.


This properly formatted README file is ready for use in your GitHub repository. You can replace the placeholder GitHub link with your actual repository URL.
