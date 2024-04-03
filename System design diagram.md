![Blank diagram](https://github.com/LakshmiLavanyaJavvadi/TS_AWS_Assignments/assets/136936999/a17bceea-b0e8-4368-b3a3-6dd6b2b73f68)

<ins>**Components:**</ins>

**Walmart POS System:**

* Generates purchase transaction events whenever a customer makes a purchase at Walmart.

**Event Bus:**

* Receives purchase transaction events from the POS system and distributes them to downstream services.

**Event Processor:**

* Consumes purchase transaction events from the event bus.
* Filters relevant events and triggers the email survey process.

**Email Survey Service:**

* Manages the creation, sending, and tracking of email surveys to customers.
* Receives requests from the event processor to send survey emails.

**Email Delivery Service:**

* Handles the actual sending of survey emails to customers.
* Interacts with external email delivery providers or SMTP servers.

**Survey Response Collector:**

* Receives and processes survey responses submitted by customers.
* May include a web server or API endpoint for handling survey responses.

<ins>**Workflow:**</ins>

* Walmart POS System generates purchase transaction events.
* Events are published to the event bus.
* Event processor filters purchase events and triggers the email survey process.
* Email survey service generates and sends survey emails to customers.
* Customers receive survey emails and provide responses.
* Survey responses are collected and processed by the survey response collector.
