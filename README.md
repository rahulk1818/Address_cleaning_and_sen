
# Project Report: Address Cleaning and Sanitization Program

## Introduction
The purpose of this project is to develop an address cleaning and sanitization program that converts a given raw address dataset into a usable dataframe. The company is facing challenges with addresses that contain special symbols, repeated words, extra useless information, and improper data formatting. These issues can impact the efficiency and accuracy of data analysis, as well as the retrieval of relevant information. The address cleaning and sanitization program aims to overcome these challenges by implementing a series of preprocessing steps to refine the address dataset. In this report, we provide an overview of the project process, along with detailed explanations for each step, and provide additional insights and information.

## Project Process
Reading Dataset and Creating Dataframe:-
In this initial step, we read the address data from the system and create a dataframe to store the data in a structured format. This allows for efficient manipulation and analysis of the address dataset. By using a dataframe, the company can leverage the functionalities and benefits offered by dataframes, such as easy data access, filtering, and transformation.

## Manually removing visible garbage values:-
Visible garbage values, such as random characters or nonsensical entries, can introduce noise and disrupt subsequent operations. The manual removal of these garbage values ensures the integrity and quality of the address data. By taking the time to inspect and remove these values, the program can produce a cleaner dataset, resulting in more accurate and reliable analysis outcomes.

## Checking and handling null in the Dataframe:-
Null values are a common challenge in datasets and can create problems during data processing. By checking for null values in the dataframe, the program identifies missing or empty entries in the address data. Handling these null values appropriately ensures that subsequent operations are not affected by missing or incomplete information. Techniques such as data imputation or data exclusion can be applied based on the specific requirements of the project.


## Inserting space between numerals and characters:-
Numerals and characters are often written together in raw address data, which can make it challenging to parse and extract relevant information. By inserting spaces between numerals and characters, the program enhances the readability and comprehensibility of the address data. This step facilitates the accurate identification and separation of different address components, such as street numbers, building names, and apartment numbers, leading to more precise analysis and information retrieval.

## Replacing all special characters with space:-
Special characters, such as punctuation marks or symbols, do not provide valuable information for address analysis and can create issues during data processing. By replacing all special characters with spaces, the program eliminates potential conflicts or errors that may arise from the presence of these characters. This step also helps standardize the address data, making it more consistent and easier to work with.

## Creating address part markers:-
Address data is typically composed of multiple components, including street names, city names, state names, postal codes, and more. By creating separate columns as markers for each address part, the program enables efficient data organization and retrieval. This segmentation provides clear boundaries between different address components, simplifying subsequent operations such as filtering or aggregating specific parts of the address data.

## Moving Pincodes to another column:-
Postal codes, or Pincodes, are essential for location-based analysis and are often included in addresses. By extracting and moving Pincodes to a separate column, the program enhances the accessibility and usability of this information. Isolating Pincodes allows the company to perform targeted analyses, such as identifying clusters of customers in specific geographic areas or optimizing logistics routes based on postal code zones.

## Removing unnecessary info from the address:-
Raw address data may contain extraneous information that is not relevant to the analysis or objective of the project. By removing unnecessary information, the program improves the accuracy and focus of the address dataset. This step ensures that subsequent analyses are based on the most pertinent and meaningful address details, reducing noise and increasing the precision of results.

## Replacing known words and abbreviation in address:-
Known words and abbreviations can introduce inconsistencies or variations in the address dataset. By replacing them with standardized terms, the program promotes consistency and enhances the usability of the address data. This standardization improves data quality and reduces the potential for errors or misinterpretations during analysis.

## Segregating address markers:-
The segregation of address markers into different columns builds upon the earlier creation of address part markers. By storing data in separate columns based on these markers, the program further enhances data organization and accessibility. This enables more focused analyses of specific address components and facilitates quick data retrieval for various use cases, such as customer segmentation by city or state.

## Creating corpus that are NonNumeric and bigger/equal to 3:-
The creation of a corpus specifically containing non-numeric words with a length of three or more characters is a valuable step in address analysis. This corpus serves as a reference for identifying significant words within the address dataset. By focusing on non-numeric words of a certain length, the program excludes common short words and numeric values that might not provide meaningful insights or contribute to the analysis objectives.

## Removing NULL from the end of words:-
In the preprocessing stage, some words may end up with the string "NULL" appended to them. This string is likely an artefact of the data processing and does not carry any useful information. By removing "NULL" from the end of words, the program ensures data accuracy and prevents potential discrepancies or misinterpretations caused by this artefact.

## Finding similar words in the corpus through fuzzy and adding to the word-only dataframe:-
Fuzzy matching techniques are employed to identify similar words within the created corpus. This process expands the coverage and accuracy of the word data by capturing variations or misspellings that may exist within the dataset. By adding these similar words to a dedicated dataframe, the program enables more comprehensive analysis and enhances the completeness of the word data for further exploration or information retrieval tasks.

## Exporting to CSVs:-
The program exports the processed word data to CSV files to ensure data persistence and easy sharing with other stakeholders. By storing the processed data in a structured and standardized format, the program enables seamless integration with other systems or analysis tools. This step facilitates collaboration and the utilization of the cleaned address data across various applications and projects.

## Keeping necessary/useful word only:-
In the final step, the program filters the word-only dataframe to retain only the necessary and useful words for the specific objectives of the project. By focusing on essential information, the program improves the efficiency of subsequent analyses and reduces the complexity associated with working with a large number of words. This streamlined dataset provides valuable insights and facilitates accurate and targeted information retrieval.

## Conclusion:-
In conclusion, the address cleaning and sanitization program successfully addresses the challenges faced by the company with its raw address dataset. By implementing a comprehensive series of preprocessing steps, the program cleans and transforms the address data into a usable dataframe. This allows for efficient data analysis, accurate information retrieval, and improved decision-making. The program's methodologies, such as removing garbage values, handling null values, and replacing known words, enhance the data quality and consistency, reducing errors and increasing the reliability of analysis outcomes. The program provides valuable insights and information from the address dataset, enabling the company to optimize various processes, enhance customer analytics, and make informed business decisions based on clean and accurate address data.
