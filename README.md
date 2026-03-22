# Community Issue Reporting Website
A dynamic multi-page website enabling local community members to report and track 
civic issues such as potholes, broken streetlights, and environmental or safety 
concerns. Built with HTML, CSS, and JavaScript, no backend or database used.

## Pages

Home (index.html)
- Overview of the platform's purpose
- Displays resolved issues with response times to build community trust

Report an Issue (report.html)
- Form for submitting issues with name, email, phone, title, urgency, and description
- Submitted issues appear dynamically below the form with auto-generated issue IDs
- Color-coded urgency: red (urgent), green (low priority), brown (moderate)

Issues Table (issues.html)
- Table of multiple hard-coded issues displaying date, title, urgency, and category
- Categories: Environment, Traffic, Safety
- Allows community members to check existing issues before submitting duplicates
- Admin login on the same page — correct credentials expand the table with additional columns including cost per issue and government approval status
- Admin can edit issue costs and delete duplicate issues
- Totals for spent and pending budget update dynamically on delete

Contact (contact.html
- Simple contact form collecting name, email, and subject
- On submission, a personalised alert confirms receipt: 
  "Hello [name], thank you for your message. We have received your message 
  about [subject] and will get back to you shortly."
- Includes a background video for visual presentation

## Technologies
- HTML, CSS, JavaScript
- 4 separate CSS files (one per page)
- Media assets: images and video

## Notes
No database used — submitted issues are stored in-memory and reset on page refresh. 
Hard-coded issues in the table simulate real database content.
Admin password is hard-coded in JavaScript (no reset password functionality).
