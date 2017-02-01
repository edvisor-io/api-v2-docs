## Student Quote

Attribute | Description
--- | ---
studentQuoteId  | 
externalId | 
studentQuoteStatusId | The student quote status object
obscuredId | Used for generating the external link to the quote
studentId | The student that the quote is for
agentUserId | The staff member who created the quote
issued | Issued date
viewed | Viewed date
decisionMade | Decision made date
expires | Expiry date
language | 
notes | 
studentQuoteOptions | An array of options in the quote
studentQuoteOptions[].name | 
studentQuoteOptions[].is_accepted | 
studentQuoteOptions[].total_price | 
studentQuoteOptions[].price_currency | 
studentQuoteOptions[].notes | 
studentQuoteOptions[].position | 
studentQuoteOptions[].items | An array of line items for a particular option
studentQuoteOptions[].items[].offering_id | 
studentQuoteOptions[].items[].fee_id | 
studentQuoteOptions[].items[].promotion_id | 
studentQuoteOptions[].items[].name | 
studentQuoteOptions[].items[].provider_name | 
studentQuoteOptions[].items[].offering_accommodation_category_id | 
studentQuoteOptions[].items[].offering_course_category_id | 
studentQuoteOptions[].items[].price_amount | 
studentQuoteOptions[].items[].price_currency | 
studentQuoteOptions[].items[].per_unit_price_amount | 
studentQuoteOptions[].items[].price_duration_amount | 
studentQuoteOptions[].items[].price_duration_type_id | 
studentQuoteOptions[].items[].start_date | 
studentQuoteOptions[].items[].end_date | 
studentQuoteOptions[].items[].service_quantity | 
studentQuoteOptions[].items[].description | 


### Queries

* `studentQuote(id: <id>)`
* `studentQuotes(ids: [<ids>])`

### Mutations

* `createStudentQuote(input: <body>)`
* `updateStudentQuote(id: <id>, input: <body>)`
* `deleteStudentQuote(id: <id>)`