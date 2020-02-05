Context

A dataset generated via our tele-calling operations is available here. We have a small team of tele-callers who make calls to users who have applied for jobs on our job assistant (you can try it by sending a “hi” on WhatsApp to +91-1234-123-123). The goal is to gauge their interest in the job and then push them to go for the interview and get hired. In some cases, we might make calls to a list of leads received from a 3rd party. For instance, to a list of drivers received from a driving school to place them in a job at a cab company. Our tele-callers generally make follow-up calls to leads who don't answer the phone (RNR status) or who demonstrate interest (to get them to go for the interview/on-boarding).
Content

● leads ○ id (unique identifier) ○ userId (foreign key reference to our internal users table) ○ name (lead’s name) ○ phoneNumber (lead’s phone number) ○ city (lead’s city) ○ state (lead’s state) ○ source (source of the lead) ○ isExternal (false if the lead was acquired via the job assistant; true if the lead was acquired via a 3rd party source) ○ createdAt (date/time of creation of the table entry) ○ receivedAt (date/time when the lead was received by us)

● lead_calls ○ Id (unique identifier) ○ telecallerId (foreign key reference to telecallers table) ○ leadId (foreign key reference to leads table) ○ client (name of the client/company/employer who the call was made for) ○ status (status of the call) ○ comments (comments entered by the telecaller) ○ calledAt (date/time of the call) ○ createdAt (date/time of creation of the table entry)

● telecallers ○ Id (unique identifier) ○ name (telecaller’s name) ○ phoneNumber (telecaller’s phone number) ○ createdAt (date/time of creation of the table entry)
Acknowledgements

Please use appropriate visualization and/or modeling techniques to back your responses. Feel free to slice and dice the dataset along various features to arrive on insights.
Inspiration

Here are the questions I'd like you to answer: 1. How efficient and effective are our tele-calling operations? 2. What are three things you would recommend we do to the efficiency and effectiveness of our tele-calling operations? 3. What are some other ways in which we can utilize this dataset to add value to Business, Operations or Product?
