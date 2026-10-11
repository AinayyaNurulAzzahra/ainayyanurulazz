# SmartDesk test cases
# SmartDesk Test Cases

| Test ID | Input | Steps | Expected result | Actual result | Pass/Fail | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| TC-ValidAccess-001 | Valid access request data | Send POST request to API | Expected HTTP 201 Created with ticket details | | | |
| TC-ValidBilling-002 | Valid billing request data | Send POST request to API | Expected HTTP 201 Created with ticket details | | | |
| TC-ValidTechnical-003 | Valid technical request data | Send POST request to API | Expected HTTP 201 Created with ticket details | | | |
| TC-BlankSubject-004 | Subject field left blank | Send POST request to API | Expected HTTP 400 Bad Request with error message | | | |
| TC-BlankDescription-005 | Description field left blank | Send POST request to API | Expected HTTP 400 Bad Request with error message | | | |
| TC-101CharacterSubject-006 | Subject exceeding 100 characters | Send POST request to API | Expected HTTP 400 Bad Request with length error | | | |
| TC-501CharacterDescription-007 | Description exceeding 500 characters | Send POST request to API | Expected HTTP 400 Bad Request with length error | | | |
| TC-DuplicateTicket-008 | Duplicate ticket data | Send POST request to API | Expected handling or appropriate status code | | | |
| TC-HTMLLikeText-009 | Input containing HTML like `<b>test</b>` | Send POST request to API | Expected sanitized input or HTTP 200/201 | | | |
| TC-AmbiguousTicket-010 | Ambiguous ticket text | Send POST request to API | Expected classification response | | | |
