#  JIRA Bug Report Examples – Manual Testing

This document contains sample bug reports written in a Jira-style format.
These examples demonstrate my understanding of defect identification,
reporting, and lifecycle management as a Manual QA fresher.

---

##  Bug 1: Login Validation Bug

### Summary
Login form allows user to submit without entering password

### Environment
- Browser: Google Chrome (Version 120)
- OS: Windows 10
- Environment: QA

### Steps to Reproduce
1. Open the application
2. Navigate to the Login page
3. Enter a valid registered email address
4. Leave the password field empty
5. Click on the **Login** button

### Expected Result
System should display a validation message:
**"Password is required"**

### Actual Result
Login request is submitted without password validation

### Priority
High

### Severity
Major

---

##  Bug 2: UI Alignment Bug

### Summary
Login button is misaligned on mobile view

### Environment
- Device: Android Mobile
- Browser: Chrome
- Screen Resolution: 360 × 640
- Environment: QA

### Steps to Reproduce
1. Open the application on a mobile device
2. Navigate to the Login page
3. Observe the position of the Login button

### Expected Result
Login button should be properly aligned and fully visible on the screen

### Actual Result
Login button overlaps with the password field and is partially hidden

### Priority
Medium

### Severity
Minor

---

##  Bug 3: API Status Code Bug (Login API)

### Summary
Login API returns 200 OK for invalid credentials

### Environment
- Tool: Postman
- API Environment: QA
- Method: POST

### Steps to Reproduce
1. Open Postman
2. Send a POST request to `/api/login`
3. Enter valid email and invalid password in request body
4. Send the request

### Expected Result
API should return:
- Status Code: **401 Unauthorized**
- Error message: "Invalid credentials"

### Actual Result
API returns:
- Status Code: **200 OK**
- Success response even with invalid password

### Priority
High

### Severity
Critical

---


