# Auto-Populate-Caller-Email-on-Incident-Form-Glide-Ajax
Developed a ServiceNow solution to automatically populate the Email ID field when a user selects a Caller on the Incident form. This implementation demonstrates communication between the client side and server side using GlideAjax and Script Include.

*Business Requirement*
When a service desk agent selects a Caller while creating an Incident, the corresponding email address should automatically populate in the Email ID field without requiring the user to search manually.

*Workflow*

User selects Caller
        │
        ▼
onChange Client Script
        │
        ▼
GlideAjax Request
        │
        ▼
Script Include
        │
        ▼
GlideRecord (sys_user)
        │
        ▼
Return Email Address
        │
        ▼
Update Email ID field


*Key Concepts Learned*
-Difference between Client-side and Server-side scripting.
-Why GlideAjax is required instead of GlideRecord in Client Scripts.
-Passing parameters using addParam().
-Receiving parameters with this.getParameter().
-Querying records using GlideRecord.
-Returning data from Script Include to Client Script.
-Updating form fields dynamically using g_form.setValue().
-Creating reusable server-side logic using Script Includes.
-DOM manipulation  used to read data 
