# Usecase Narrative

| Use Case Name | Generate Report |
|---------------|--------------------------------------|--------------------------------------|
| Actor         | Admin |
| Pre-condition | Must have data taken from the detection of vehicle through the use of OpenCV |
| Description   | The system would generate all traffic reports with graphs |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Request traffic report | Step 2. Validates if system has already data to compile. |
| | | Step 3. If system has data, creates a compilation of all traffic condition reports and send it to the Admin. else it would prompt a message “no data”. |
| Alternate Path | Alt Step 2. If none. Go back to Step 1 |
| | Alt Step 3. Admin can cancel generate report request and would display a confirmation message if it would continue to cancel the request. Go back to Step 1|


| Use Case Name | Load Video File |
|---------------|--------------------------------------|--------------------------------------|
| Actor |Admin |
| Description |The Admin will load a video fill that will be fed into the system to detect the traffic |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Select Upload | Step 2. Validates if it's a video file |
| | | Step 3. If it is. Proceed to Step  4 |
| | | else if none cancel. Go back to Step 1 |
| | Step 4. Upload selected video | Step 5. Upload Video file to the system for the system to analyze. |
| Alternate Path | Alt Step 2. If prompts a message “System does not support this file extension”. Go back to Step 1 |


| Use Case Name | Receive SMS |
|---------------|--------------------------------------|--------------------------------------|
| Actors | End User, Admin |
| Pre-condition | For End Users they must subscriber to receive an SMS report |
| Description | Users will receive an SMS in a specific time and road they have subscribed to, Admin will receive all road condition in any time |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Users waiting for SMS | Step 2. Will send an SMS to User prior their specific time and road. |
| Alternate Path | Alt Step 2. If the User failed to receive a message, user may request for a text message on their subscribed service. |


| Use Case Name | View Road Status |
|---------------|--------------------------------------|--------------------------------------|
| Actors | End User, Admin |
| Description | Displays all road status of current date, user may select current previous, or specific date |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Users Selects Action | Step 2. Displays Current, Previous, Specific Day. |
| | | Step 3. If User selects Current. Proceed to Step 4 | 
| | | else if User selects Previous. Proceed to Step 6 |
| | | else if User selects for a specific day. Proceed to Step 8 |
| | Step 4. Selects Current day | Step 5. Displays all current road status with indicators. |
| | Step 6. Selects Previous day | Step 7. Displays the previous traffic condition with indicators. |
| | Step 8. Selects Specific day | Step 9. Validates if the day if the system has data on that specific date. |
| | | Step 10. Display the traffic condition on that specific day. |
| Alternate Path | Alt Step 5. If user selects current day on again it will reload the page. |
| |Alt Step 6. If user selects previous it would load the traffic condition previous to that. |



| Use Case Name | Register |
|---------------|--------------------------------------|--------------------------------------|
| Actor | End User |
| Description | User would fill out the necessary biodata or information of the user and subscribe to a service |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Selects Register and fill in the information | Step 2. Validates if the user has filled out the necessary information. |
| | | Step 3. If user has completed necessary information, prompts a message and choice “Do you want to subscribe to a road ? ( Yes / No)“. |
| | | Step 4. If Yes. Proceed to Step 5. |
| | |else Proceed to Step 9. |
| | Step 5. | Step 6. Selects a road to subscribe |
| | | Step 7. Register the user as a subscriber to a road. 
| | | Step 8. If the user has successfully subscribed. Proceed to Step 10. |
| Step 9. | Step 10. Complete Registration. |
| Alternate Path | Alt Step 2. If user inputted missing information. Go back to Step 1. |
| | Alt Step 5. If the user cancel to subscribe during Registration. Go back to Step 3. |
| | Alt Step 8. If not. Go back to Step 6. |


| Use Case Name | Send SMS Road Query |
|---------------|--------------------------------------|--------------------------------------|
| Actors | End User, Admin |
| Pre-condition | End User must be a registered user for them to send an SMS query |
| Description | Users sends an SMS to the system |
| Typical Course of Event | Actor Action | System Response |
| |Step 1. Send SMS query | Step 2. Executes Query |
| | | Step 3. Post Road Status |
| Alternate Path | Alt Step 2. If query's syntax is incorrect send a message that the query is unacceptable or incorrect. Go back step 1. |


| Use Case Name | Manage Users |
|---------------|--------------------------------------|--------------------------------------|
| Actor | Admin |
| Pre-condition | Users must be registered through the web application. |
| Description | The admin can create, read, update and delete the users registered in the web application. |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Admin selects manage users option. | Step 2. The registered users is viewed in the page as a list of names |
| | Step 3. Delete user(s) go to Step 4. | Step 4. The selected user will be deleted. |
| | Step 5. Create user(s)  go to Step 6. | Step 6. A form will be rendered to be filled by the admin. |
| | Step 7. Edit user(s) go to Step 8. | Step 8. A form will be rendered with the user(s) information. |
| Alternate Path | Alt Step 3. Admin can cancel any action with a prompt asking to proceed anyway. Go back to Step 1. |


| Use Case Name | Manage Road |
|---------------|--------------------------------------|--------------------------------------|
| Actor | Admin |
| Pre-condition | Admin must load the video file first. |
| Description | The system will set imaginary boundary lines for getting data in that area of interest. |
| Typical Course of Event | Actor Action | System Response |
| | Step 1. Manages the road. | Step 2. Validates if the video file is loaded. |
| | | Step 3. If system has the video file, it creates boundary lines and will start to get the area of the road and the vehicles speed.
| | | else it would prompts a message “no video file loaded”. |
| Alternate Path | Alt Step 3. Admin can cancel managing the road with a prompt asking to proceed anyway. Proceed to Step 1 |

