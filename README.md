 HEALTH CENTER QUEUE LOG

 Location: Brgy. Caparan Ipil, Zamboanga Sibugay

PROBLEM STATEMENT 

In Brgy. Caparan Ipil, Zamboanga Sibugay, health workers and patients struggle to keep track of the patient queue and know who is next because there is no proper list of patients, only verbal calling, so the queue becomes disorganized, crowded and slow. A web page where the health worker can add patients to an organized queue list with a queue number, name, purpose and time of arrival would help.

 REQUIREMENT

**FR-01:** Health worker can add a patient to the queue: patient name, purpose of visit, date and time of arrival.

**FR-02 (2nd feature via Pull Request):** Health worker can search a patient by name. Typing in the Search box filters the list. Pressing CLEAR shows all patients again.

 ACCEPTANCE CRITERIA 

1. Saving with a blank patient name is rejected and an error message appears.
2. Saving with only spaces in the patient name is rejected.
3. Entries are still there after a page refresh because the data is saved in localStorage.
4. The new patient appears at the end of the queue with the correct next queue number and time.
5. Searching for a name shows only the matching patient(s). Searching for a name that is not in the list shows "No patient found".
