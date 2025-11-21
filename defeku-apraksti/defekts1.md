# Defect 1: Application crashes when submitting empty required fields

**Description:**  
The user opens the form and leaves a required field empty, then tries to save. The application crashes with an error message.

**Steps to Reproduce:**
1. Open the application.
2. Navigate to the "New Entry" form.
3. Leave a required field empty.
4. Click the "Save" button.

**Expected Result:**  
The form should validate input, warn the user about the empty field, and prevent saving the entry.

**Actual Result:**  
The application crashes and shows a non-informative error message.

**Priority:** Medium

**Additional Information:**  
- OS: Windows 10  
- Application Version: 1.0.3  
- Error in log file: `NullReferenceException at Form.Save()`