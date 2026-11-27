      HEALTH CENTER QUEUE LOG
      
Location:  Brgy. Caparan Ipil

PROBLEM STATEMENT

In Brgy. Caparan Ipil health workers and patients struggle to keep track of the patient queue and know who is next because there is no proper list of patients, only verbal calling, so the queue becomes disorganized, crowded and slow. A web page where the health worker can add patients to an organized queue list would help.

REQUIREMENT

FR-01: Health worker can add a patient to the queue.

Health worker types ONLY:
- Patient Name (First Name + Last Name, First letter of each name must be Uppercase. Example: JoAnne Dacula)
- Purpose of Visit

The app AUTOMATICALLY adds:
- Queue Number
- Date
- Time of Arrival

The health worker DOES NOT type the date and time. This is to prevent bias. No one can change the time to make their friends or family first.

FR-02 (2nd feature via Pull Request): Health worker can search a patient by complete name. Typing in the Search box shows only the matching patient. Pressing CLEAR shows all patients again.

ACCEPTANCE CRITERIA
1. Add patient with Name + Purpose, appears at the end of the queue with correct next Queue Number and automatic Date and Time.
2. Saving with a blank patient name is rejected and an error message appears.
3. Saving with only spaces in the patient name is rejected.
4. Saving with only one name (e.g. Jenny) is rejected. Must be First Name + Last Name.
5. Saving with lowercase name (e.g. jenny reyes, Jenny reyes) is rejected. First letter of First Name and Last Name must be Uppercase.
6. Saving with numbers or symbols in name is rejected. Letters only.
7. Entries are still there after a page refresh because the data is saved in localStorage.
8. Searching for a complete name shows only the matching patient(s).
9. Searching for a name that is not in the list, or incomplete name, shows "No patient found".
10. Duplicate(double entry) is rejected.
