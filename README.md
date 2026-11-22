Health Center Queue Log 

**Location:** Brgy. Caparan, Ipil, Zamboanga Sibugay

## Problem Statement 
In Brgy. Caparan Ipil, Zamboanga Sibugay, health workers and patients struggle to keep track of the patient queue and know who is next because there is no proper list of patients, only verbal calling, so the queue becomes disorganized, crowded and slow. A web page where the health worker can add patients to an organized queue list with a queue number, name, purpose and time of arrival would help.

## Requirement
User = The health worker
can [action] = add a patient to the queue
[the fields or data] = patient name, purpose of visit, time of arrival, queue number

### Acceptance Criteria
1. Saving with a blank patient name is rejected and an error message appears.
2. Saving with only spaces in the patient name is rejected.
3. Entries are still there after a page refresh because the data is saved in localStorage.
4. The new patient appears at the end of the queue with the correct next queue number and time.
