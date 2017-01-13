## Student

Attribute | Description
--- | ---
studentId  | 
ownerId | The ID of the staff member assigned to this student
agencyId | The ID of the agency office that this student belongs to
nationalityId | The ID of the country representing the student’s nationality
firstname | 
lastname | 
email | 
phone | 
address | 
postalCode | 
gender | M / F
birthdate | 
passportNumber | 
notes | 
accommodation | 
budget | 
startMonth | 
startYear | 
startDay | 
durationWeekAmount | The number of weeks the student would prefer to study for
hoursPerWeek | 
amOrPm | 
isHighPriority | 
isArchived | 
archiveNotes | 
archiveDate | 
studentSecondaryContacts | An array of Student Secondary Contact objects
studentCoursePreferences | An array of Student Course Preference objects
studentLocationPreferences | An array of Student Location Preference objects
studentSchoolPreferences | An array of Student School Preferences objects
studentStudyRecords | An array of Student Study Record objects
studentTags | An array of Student Tag objects
customProperties | An array of custom properties that can be stored with the student. The custom properties can be configured at the agency office level.
customProperties[].customPropertyId | 
customProperties[].label | 
customProperties[].value | 


### Queries

* `student(id: <id>)`
* `students(ids: [<ids>])`

### Mutations

* `createStudent(input: <body>)`
* `updateStudent(id: <id>, input: <body>)`
* `upsertStudent(input: <body>)`
* `deleteStudent(id: <id>)`