## Student Enrollment

Attribute | Description
--- | ---
studentEnrollmentId | 
studentEnrollmentStatusId | 
studentEnrollmentDecisionStatusId | 
schoolId | The campus this enrollment is for
studentId | 
languageId | 
obscuredId | 
specialInstructions | 
agencyOwnerId | 
schoolOwnerId | 
sent | Date the enrollment was sent
comments[] | An array of comments / chat associated with the enrollment
comments[].userId | 
comments[].comment | 
fields[] | An array of fields associated with the enrollment
fields[].fieldTypeId | ie. Text, Dropdown, Date, etc..
fields[].codeName | 
fields[].isRequired | 
fields[].description | 
fields[].position | 
fields[].placeholder | 
fields[].value | The value of the field. This is NULL if the field type is dropdown (See options[])
fields[].options[] | An array of options available for the field (if it is a dropdown)
fields[].options[].codeName | 
fields[].options[].selected | 

### Queries

* `studentEnrollment(id: <id>)`
* `studentEnrollments(ids: [<ids>])`

### Mutations

* `createStudentEnrollment(input: <body>)`
* `updateStudentEnrollment(id: <id>, input: <body>)`
* `deleteStudentEnrollment(id: <id>)`
