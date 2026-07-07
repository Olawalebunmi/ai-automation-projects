Post-UTME Student Support Lead Management Workflow

Overview

This project showcases a **Lead Management Workflow** built with **Zapier** to automate student support and follow-up processes for a Post-UTME tutorial center.

The workflow captures student feedback, identifies students who require additional academic support, categorizes them based on their subject needs, and automatically sends personalized follow-up emails.

By automating these processes, tutorial centers can improve student engagement, streamline communication, and provide targeted intervention for students who need it most.


Workflow Features

Lead Capture
- Collects student feedback through **Typeform**.

Lead Qualification
- Filters students who indicate they are:
  - **Not Very Prepared**
  - **Not Prepared At All**

for their upcoming Post-UTME examination.

Data Standardization
- Uses **Formatter by Zapier** to capitalize student names for consistency.

Smart Lead Routing
- Uses a **Lookup Table** to automatically categorize students based on the subject they need the most help with.

Automated Follow-Up
- Routes students through different support paths.
- Delays communication by 1 day.
- Sends personalized support emails via Gmail.

Workflow Architecture


Typeform Submission
        │
        ▼
Filter by Zapier
(Not Very Prepared OR Not Prepared At All)
        │
        ▼
Formatter
(Capitalize Student Name)
        │
        ▼
Lookup Table
(Subject → Category)
        │
        ▼
Paths

├── Science
│     ├── Delay (1 Day)
│     └── Gmail Follow-Up
│
├── Arts
│     ├── Delay (1 Day)
│     └── Gmail Follow-Up
│
└── Commercial
      ├── Delay (1 Day)
      └── Gmail Follow-Up


Subject Categorization Logic

The workflow uses a Lookup Table to group subjects into academic categories.

| Subject | Category |
|----------|----------|
| Mathematics | Science |
| Physics | Science |
| Chemistry | Science |
| Biology | Science |
| English Language | Arts |
| Government | Arts |
| Literature | Arts |
| Economics | Commercial |

Filter Logic

Only students who selected one of the following responses proceed through the workflow:

- Not Very Prepared
- Not Prepared At All

This ensures that support efforts are focused on students who may require additional academic assistance.

Path Conditions

Science Path
Triggered when the Lookup Table output equals:

Science


Arts Path
Triggered when the Lookup Table output equals:

Arts


Commercial Path
Triggered when the Lookup Table output equals:


Commercial

Delay Logic

A **1-day delay** is applied before follow-up emails are sent.

### Benefits
- Allows time for response review.
- Prevents immediate email overload.
- Creates a more natural follow-up experience.
- Improves student engagement.


Automated Email Follow-Up

Students receive personalized support emails based on their academic category.

Example Email

Hello Olubunmi Olawale,

Thank you for your feedback.

We have identified that you may benefit from additional support in your art subjects.

We will share study materials and revision guidance shortly.

Best regards,
Promise Keeper Tutorials


Tools Used

- Typeform
- Zapier
- Formatter by Zapier
- Paths by Zapier
- Delay by Zapier
- Gmail


Benefits

- Automated student support
- Faster follow-up process
- Improved student engagement
- Better lead qualification
- Reduced manual administrative work
- Scalable workflow design

Learning Outcomes

This project demonstrates practical experience with:

- Workflow Automation
- Lead Management
- Conditional Logic
- Data Transformation
- Lookup Tables
- Email Automation
- Educational Process Automation
- No-Code Development


Author

**Olubunmi Olawale**

- AI Machine Learning Data Annotator Specialist
- Data Analyst
- AI Automation Enthusiast
- Workflow Builder


License

This project is available for educational and portfolio purposes.