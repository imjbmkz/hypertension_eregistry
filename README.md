## Hypertension e-Registry
Excel-based hypertensive patient tracking, monitoring, and reporting system

### About this document
This document contains (1) the workflow that discusses how the Hypertension e-Registry is used on the users' level, and (2) the technical aspects, such as the modules,  functions and sub-procedures used, and the worksheet dependencies.

### Description of this project
The **Hypertension e-Registry** (simply *e-Registry*) is an Excel-based system that is used to track hypertensive patients, monitor their monthly visits, and extract reports containing statistics and indicators relevant to hypertension. This is intended to be used at the municipality level (eg. RHU). The e-Registry has two primary sections: (1) **Patient Registry** and (2) **Reports**. The following are the tasks that each section can do.

**Patient Registry**
- Search existing patient records
- Update patient details
- Add visit details (blood pressure, medications)
- Drop patients
- Enroll new patients

**Reports**
- Generate annual and quarterly statistics (counts and percentages)
- Generate defined indicators
- Generate quarterly list of defaulters
- Generate quarterly count of current medications
- Download patient masterlist

The e-Registry can only be used by one person at a time to ensure that the data is up to date, and are not scattered to different Excel files. Merging different e-Registry versions with different enrollments isn't part of the e-Registry's functions. In the **Portable Hypertension Reporting Tool** (**PoHRT**) section, the alternative way of adding visit details of existing patients will be discussed.

### System Requirements
The Hypertension e-Registry was developed using Microsoft Excel 2010. It can be used with Microsoft Excel 2010, Excel 2013, Excel 2016, Excel 2019, and Excel 365. Note that this is not going to work with Google Sheets, LibreOffice, WPS, and the like. The file contains macros, hence, macro must be enabled after opening the e-Registry. 
![Enable content in Excel](/images/enable_content.png)

### User Instructions 
#### User Interface
The Hypertension e-Registry has only one sheet named **User Interface**. It has some brief description about the major components of the e-Registry, and the buttons that open the user forms and run the defined procedures and functions. Every time the e-Registry opens, each patient is checked and status is changed to **lost to follow-up** (**L2FU**) if they didn't have visit records for the last 12 months (more of this on **Drop Patient** section).
![User Interface](/images/user_interface.png)

**Update Municipality**
Before using the e-Registry, **Region**, **Province**, and **Municipality** fields must be filled-out. Encoders can update existing records, **but not enroll new patients** if these fields are blank. To update this, click on the **UPDATE MUNICIPALITY** button, fill-out the **Region**, **Province**, and **Municipality** fields, and click **UPDATE**. The fields will be completed afterwards.
![Update Municipality](/images/update_municipality.png)

**Patient Registry and Reports**
The User Interface has the buttons that open the **Patient Registry** and **Reports** forms of the e-Registry. The **Open the e-Registry** button opens the patient registry that is used for managing patient records, adding visits, updating medications, and enrolling new patients. The **Generate Reports** button opens the generator of hypertension-related statistics (count of patients with controlled/uncontrolled monitoring, defaulters, active and inactive patients), and key indicators (service effectiveness and service coverage).

#### Patient Registry
##### Search Patient
Patients can be searched using their **last name**, **first name**, **PhilHealth #**, and/or **date of birth**. Approximate search can be done (see sample on the image). Results will be shown in the list box. **Double-click** on an entry to select that patient.

![Search Patient](/images/search_patient.png)

After selecting a patient, their details will be added on the right-side panel of the patient registry. Patient’s **name**, **PhilHealth #**, **date of birth**, **enrollment date**, **date of last visit**, **last blood pressure reading**, **current status**, **inactivation date (for dropped patients)**, and **diagnosis** will be available. A patient must be selected before using the next three tabs.

![Select Patient](/images/select_patient.png)

If there are no results that matched with the search entries, two prompt messages will show up. The first one is a warning saying, “**There are no results found**” and to “**check spelling**”. The second message is a confirmation to the user if s/he **wants to open the enroll form**. Selecting “yes” would allow the user to enroll a new patient. 

![Select Patient](/images/no_results_found.png)

##### Enroll New Patient

##### User Interface

##### Edit Patient Details

##### Add Visit

##### Drop Patient

#### Reports
##### Statistics

##### Indicators

##### Defaulters

##### Medications
