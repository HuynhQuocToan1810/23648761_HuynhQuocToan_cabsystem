| TC ID | Business Context | Scenario | API | Method | Test Data | Expected Result | Status |
|---|---|---|---|---|---|---|---|
| TC02-01 | Customer | View own profile | Customer API | GET | Valid JWT | Own profile returned | NOT RUN |
| TC02-02 | Customer | Update profile with valid data | Customer API | PUT/PATCH | Valid name/phone | Profile updated | NOT RUN |
| TC02-03 | Customer | Update profile with invalid email | Customer API | PUT/PATCH | Invalid email | Validation error | NOT RUN |
| TC02-04 | Customer | Update profile with invalid phone | Customer API | PUT/PATCH | Invalid phone | Validation error | NOT RUN |
| TC02-05 | Customer | View trip history | Trip API | GET | Valid customer JWT | Own trip history returned | NOT RUN |
| TC02-06 | Customer | View another customer's trip | Trip API | GET | Other customer's trip ID | 403/404 returned | NOT RUN |
| TC02-07 | Customer | Access profile without authentication | Customer API | GET | No JWT | 401 Unauthorized | NOT RUN |
