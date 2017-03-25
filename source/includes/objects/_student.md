## Student

Attribute | Description
--- | ---
studentId | 
ownerId | The ID of the staff member assigned to this student
agencyId | The ID of the agency office that this student belongs to
nationalityId | The ID of the country representing the student’s nationality
photoId | 
firstname | 
lastname | 
email | 
phone | 
address | 
postalCode | 
gender | 
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
created | 
modified | 
currentLocationGooglePlaceId | 
isHighPriority | 
isArchived | 
isDeleted | 
studentArchiveReasonId | 
archiveNotes | 
archiveDate | 
startDate | 
recoveryDate | 
studentTags | Array&lt;[StudentTag](#student-tag)&gt;
studentCoursePreferences | Array&lt;[StudentCoursePreference](#student-course-preference)&gt;
studentSchoolPreferences | Array&lt;[StudentSchoolPreference](#student-school-preference)&gt;
studentLocationPreferences | Array&lt;[StudentLocationPreference](#student-location-preference)&gt;
studentCurrentPipelineStages | Array&lt;[StudentCurrentPipelineStage](#student-current-pipeline-stage)&gt;
studentPipelineStageStepCompleted | Array&lt;[StudentPipelineStageStepCompleted](#student-pipeline-stage-step-completed)&gt;
customPropertyValues | Array&lt;[CustomPropertyValue](#custom-property-value)&gt;
studentSecondaryContacts | Array&lt;[StudentSecondaryContact](#student-secondary-contact)&gt;
studentStudyRecords | Array&lt;[StudentStudyRecord](#student-study-record)&gt;
quotes | Array&lt;[Quote](#quote)&gt;
studentQuotes | Array&lt;[StudentQuote](#student-quote)&gt;
owner | [User](#user)
currentLocationGooglePlace | [GooglePlace](#google-place)
nationality | [Country](#country)
files | Array&lt;[File](#file)&gt;
studentEnrollments | Array&lt;[StudentEnrollment](#student-enrollment)&gt;
photo | [Photo](#photo)


### Queries

```shell
#example of using studentsGetList

curl https://api.edvisor.io/graphql \
  -X POST \
  -H "Authorization: Bearer MY_API_KEY" \
  -H 'content-type: application/json' \
  -d '{"query":"query CustomQueryName($pagination: PaginationInput, $filter: StudentsFilterInput) {studentsGetList(pagination: $pagination, filter: $filter) {count, data {studentId}}}","variables":{"pagination":{"limit":10,"offset":0},"filter":{"isDeleted":false}}}'
```

Query | Return object
--- | ---
student(studentId: &lt;Int&gt;) | [Student](#student)
students(studentIds: Array&lt;Int&gt;) | Array&lt;[Student](#student)&gt;
studentsGetList(pagination: &lt;PaginationInput&gt;, filter: &lt;StudentsFilterInput&gt;) | [ListResult](#list-result)

### Mutations

Mutation | Return object
--- | ---
createStudent(input: &lt;StudentInput&gt;) | [Student](#student)
createWeb2LeadStudent(input: &lt;StudentInput&gt;) | [Student](#student)
updateStudent(studentId: &lt;Int&gt;, input: &lt;StudentInput&gt;) | [Student](#student)
deleteStudents(studentIds: Array&lt;Int&gt;) | [Student](#student)
uploadStudentFiles(studentId: &lt;Int&gt;, fieldName: &lt;String&gt;) | [File](#file)
uploadStudentPhoto(studentId: &lt;Int&gt;, fieldName: &lt;String&gt;) | [File](#file)