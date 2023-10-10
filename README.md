# BizcardX
BizcardX: Extracting Business Card Data with OCR

**Overview**

BizcardX is a versatile tool that enables users to extract and manage data from business cards efficiently. It utilizes Optical Character Recognition (OCR) to extract text from business cards, provides a user-friendly Streamlit GUI for interaction, stores the extracted data in an SQL database, and offers data extraction capabilities. This README file serves as a guide for setting up and using BizcardX.

**Features**

OCR Data Extraction: Automatically extracts text from business cards, including names, phone numbers, emails, addresses, and more.

Streamlit GUI: Provides an intuitive and interactive interface for users to upload and process business card images.

SQL Database: Stores extracted business card data in an SQL database for easy retrieval and management.

Data Extraction: Offers data extraction capabilities, allowing users to search and export specific business card data.

**Libraries and Modules used**

Streamlit-To create a graphical user interface
EasyOCR  -Too extract text from images
mysql.connector- To store and retrive the data

**Workflow**

• Install the rquired libraries using the pip install command. Streamlit, mysql.connector, pandas, easyocr

```pip install [Name of the library]```

• Execute the “BizCardX_main.py” using the streamlit run command.

```streamlit run BizCardX_main.py```

• A webpage is created in the browser with threee menu options namely HOME,UPLOAD AND EXTRACT MODIFY whee user can upload the respective business card whose infromation has to be extracted stored and modified or deleted

• Once user uploads a business card, the text present in the card is extracted by easyocr library

• The extracted text is sent to get_data() function(user defined- I have coded this function) for respective text classification as company name, card holder name, designation, mobile number, email address, website URL, area, city, state, and pin code using loops and some regular expression.

• On Clicking Upload to Database Button the data gets stored in the MySQL Database

• MODIFY menu -uploaded data’s in SQL Database can be accessed for Read, Update and Delete Operations












