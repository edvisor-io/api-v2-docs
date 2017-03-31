# Webhooks

## Introduction

In addition to the available GraphQL API, Edvisor.io can register webhooks so you can 
synchronise the data in your agency account with an external service or system. When 
registering a webhook, you’re able to subscribe to specific events so that you only 
receive the events (synchronize the data) that you want. 

For example, if you’d like keep the student information in your external CRM up-to-date with 
changes made to students in your Edvisor.io account, you can register a webhook that 
subscribes to the “student:update” event.  When a student is updated on Edvisor.io, we will 
then send the updated information to a pre-set URL.

Sample Webhook:

Webhook endpoint: `https://api.your-agency.com/webhook/edvisor`

Events subscribed: `student:create`, `student:update`

What happens: When a student is updated or created, we will send a `POST https://api.your-agency.com/webhook/edvisor` request with a body containing the changes that represent the event.

## Responding to a webhook

To acknowledge receipt of a webhook, your endpoint should return a 2xx HTTP status code. Any 
other information returned in the request headers or request body is ignored. All response 
codes outside this range, including 3xx codes, will indicate to Edvisor.io that you did not 
receive the webhook. This does mean that a URL redirection or a "Not Modified" response will 
be treated as a failure.

If a webhook is not successfully received for any reason, Edvisor.io will continue trying 
to send the webhook once every 15 minutes for up to 3 days. 

## Available events

### Student

* student:create
* student:update
* student:delete

### School

* school:create
* school:update
* school:delete

### Offering

* offering:create
* offering:update
* offering:delete

### Quote

* quote:create
* quote:update
* quote:delete

### Promotion

* promotion:create
* promotion:update
* promotion:delete

### Student enrollment

* studentEnrollment:create
* studentEnrollment:update
* studentEnrollment:delete

## Event Object

The event object that is sent along with the webhook request will be structured like the following:

> Sample Event object:

```json
{
  "created": "2017-03-31T19:12:43.687Z",
  "user": {
    "userId": 1,
    "firstname": "John",
    "lastname": "Garcia",
    "email": "john.garcia@education-agency.com"
  },
  "type": "student:update",
  "data": {
    "after": {
      "studentId": 1,
      "email": "frank@email.com"
    },
    "before": {
      "studentId": 1,
      "email": ""
    }
  }
}
```

Attribute | Description
--- | ---
created | Timestamp of when this event occured
user | Information regarding the creator of this event
user.userId | 
user.firstname | 
user.lastname | 
user.email | 
type | Event name (ie. `student:create`)
data | 
data.after | The object affected AFTER the event has taken place
data.before | the object BEFORE the event took place
