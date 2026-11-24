## 1 · Purpose validation
- Prompt: Reject blank Purpose. Require at least 3 letters, only letters and spaces. Example: Check Up, Dental.
- Result: Added validatePurpose function. Blank Purpose rejected, Check Up accepted.
- Verified: Tested blank Purpose -> rejected, Check Up -> accepted.
- Commit: Add Purpose validation

## 2 · Delete with confirmation
- Prompt: Add a Delete button per patient. Before deleting, show a confirmation: Are you sure you want to delete JoAnne Dacula? Use confirm(). After delete, update the list and Queue No.
- Result: Added deletePatient function with confirm dialog.
- Verified: Tested delete JoAnne Dacula -> clicked OK, patient removed. Clicked Cancel, patient stayed.
- Commit: Add delete with confirmation

## 3 · Search by Name
- Prompt: Add a search box on top of the list. When health worker types a name, filter the list in real time. Search should ignore uppercase/lowercase. Show "No patient found" if no match.
- Result: Added search input with filter function.
- Verified: Tested search "joanne" -> showed JoAnne Dacula. Search "zzz" -> showed No patient found.
- Commit: Add search by Name

## 4 · Auto Queue No. after delete
- Prompt: Queue No. should always be 1, 2, 3 in order. After deleting a patient, renumber the remaining patients automatically. Do not reuse deleted Queue No. incorrectly.
- Result: Added renumber function after delete.
- Verified: Tested delete Queue No. 2 -> remaining patients became 1, 2.
- Commit: Fix Queue No. renumber

## 5 · Clear All button
- Prompt: Add a Clear All button. Before clearing, show confirmation: Are you sure you want to clear all patients? After clearing, localStorage should also be empty.
- Result: Added clearAll function that clears list and localStorage.
- Verified: Tested Clear All -> clicked OK, list empty, refresh page, still empty.
- Commit: Add Clear All button

## 6 · Date and Time format
- Prompt: Date should be MM/DD/YYYY and Time should be 12-hour format with AM/PM. Example: 11/24/2026, 02:30 PM. Date and Time are automatic when adding a patient, health worker cannot edit them.
- Result: Updated date and time formatting using toLocaleDateString and toLocaleTimeString.
- Verified: Tested add patient -> showed 11/24/2026, 02:30 PM.
- Commit: Fix Date and Time format

## 7 · Prevent duplicate patient
- Prompt: Do not allow same Name + Purpose twice on the same day. If JoAnne Dacula with Check Up already exists today, show alert: Patient already in queue today.
- Result: Added duplicate check before adding.
- Verified: Tested add JoAnne Dacula Check Up twice -> second one rejected with alert.
- Commit: Prevent duplicate patient
