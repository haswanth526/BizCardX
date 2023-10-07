## Project Overview

   A simple tool for obtaining data from business cards is called BizCardX. The application recognises text on business cards using OCR technology and extracts the information into a SQL database after categorising it with regular expressions. Users can use a GUI created with streamlit to access the retrieved data.
   Users are guided through the uploading and information extraction processes by the BizCardX application's straightforward and user-friendly user interface. Users could simply add the extracted data to the database with a click after it was presented to them in a neat and organised manner. Additionally, users can simply read, edit, and remove data stored in databases according on their needs.
      
## Libraries

   - Pandas - (To Create a DataFrame with the scraped data)
   - mysql.connector - (To store and retrieve the data)
   - Streamlit - (To Create Graphical user Interface)
   - EasyOCR - (To extract text from images)
   
   
## Workflow

   The steps listed below will help you get started with BizCardX Data Extraction:

- Use the pip install command to install the necessary libraries. Streamlit, pandas, easyocr, and mysql.connector.
   
      Installing a library with pip

- Use the run command in streamlit to run **"BizCardX_main.py".

      run BizCardX_main.py in streamlit

- A webpage is shown in the browser; I have designed the app with three menu options, including **HOME," "UPLOAD & EXTRACT," and "MODIFY," where the user can upload the relevant business card, the information from which must be **extracted, stored, modified, or deleted," as necessary.

- The **easyocr** library extracts the text from the business card when the user uploads it.

- The collected text is delivered to the user-defined get_data() method, which I wrote, for text classification as the firm name, card holder name.
- Using loops and some regular expression, you may find a designation, mobile number, email address, website URL, area, city, state, and pin code.

- The user can alter the displayed categorised data further according to their needs.

- Data is stored in the MySQL Database upon clicking the **Upload to Database Button**. (Note: For connection establishment, enter the appropriate host, user, password, and database name in create_database, sql_table_creation, and connect_database.)

