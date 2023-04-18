# Part 1__ Test Cases <br>

## Feature: Schedule (a Visit) <br>
 <br>

### Scenario 1: Verify that "User" can navigate to "schedulePage" from the "homePage" <br>
**Given**: "User" is on the "homePage" of zoomcare.com <br>
**When**: "User" clicks on "Schedule" header   (// can add or replace with a "Schedule a Visit" button) <br>
**Then**: the "schedulePage" should load successfully <br>
**And**: the "schedulePage" should contain all necessary elements <location\>, <appointment type\>, <date\> <br>

**Acceptance Criteria:** <br>
1. The "Schedule" header should be visible and clickable on the homePage. <br>
2. The "Schedule a Visit" button should be visible and clickable on the homePage. <br>
3. Clicking on the "Schedule" header or "Schedule a Visit" button should take the user to the schedulePage within 'XX' seconds.<br>
4. The schedulePage should contain a <location\> field, which allows the user to select a zoomcare location from a drop-down list of available locations.<br>
5. The schedulePage should contain an <appointment type\> field, which allows the user to select an appointment type from a drop-down list of available appointment types.<br> 
6. The schedulePage should contain a <date\> field, which allows the user to select an available date from a calendar or date picker.<br>
7. The schedulePage should display error messages if the user makes invalid selections or if any required fields are left blank.<br>
8. The schedule Page should provide visit scheduling details, including clinic info, provider info, and next availability info etc.<br>
9. The schedulePage should be accessible and meet the WCAG 2.1 A/AA accessibility guidelines. <br>
10. The schedulePage all buttons, fields, and links should be functional and respond to user interactions. <br>

### Scenario 2: Verify that "User" can schedule a "Clinical Care" visit with an valid appointment info
**Given**: "User" is on the "schedulePage" <br>
**When**: "User" selects valid appointment information <br>
**And**: "User" should see provider availability under "Clinical Care" <br>
**Then** "User" should be able to schedule the "Clinical Care" visit <br>

**Acceptance Criteria:** <br>
1. The elements should be visible and clickable on the "schedulePage" (location, type, date, btnRefresh etc). <br>
2. The user should be able to select a valid location, appointment type, and date for the visit. <br>
3. Once the user has made a valid selection, the schedulePage should display the available appointment provider and times for the selected location and appointment type. <br>
4. The schedulePage should show the availability of all providers who can offer the selected appointment type at the selected location on the selected date. <br>
5. The provider available time slot should be accurate and up-to-date, reflecting any changes or cancellations in real-time. <br>
6. The user can click "More" to see all available time slots. <br>

### Scenario 3: Verify that "User" can schedule a "VideoCare" visit with an valid appointment info
**Given**: "User" is on the "schedulePage" <br>
**When**: "User" selects valid appointment information <br>
**And**: "User" should see provider availability under "VideoCare" <br>
**Then** "User" should be able to schedule the "VideoCare" visit <br>

**Acceptance Criteria:** <br>
1. The elements should be visible and clickable on the "schedulePage" (location, type, date, btnRefresh etc). <br>
2. The user should be able to select a valid location, appointment type, and date for the visit. <br>
3. Once the user has made a valid selection, the schedulePage should display the available appointment provider and times for the selected location and appointment type. <br>
4. The schedulePage should show the availability of all providers who can offer the selected appointment type at the selected location on the selected date. <br>
5. The provider available time slot should be accurate and up-to-date, reflecting any changes or cancellations in real-time. <br>
6. The user can click "More" to see all available time slots. <br>

### Scenario 4: Verify that "User" can modify appointment info
**Given**: "User" is on the "schedulePage" <br>
**When**: "User" selects valid appointment information <br>
**And**: "User" should see providers availability <br>
**Then**: "User" modify appointmnet info
**Then** "User" should be able to see the new schedule for the new visit <br>

**Acceptance Criteria:** <br>
1. The user should be able to modify selected visit info. <br>

### Scenario 5: Verify that "User" canNOT schedule a visit with an invalid appointment info
**Given**: "User" is on the "schedulePage" <br>
**When**: "User" selects invalid appointment information <br>
**Then**: "User" should not be able to schedule the visit <br>

**Acceptance Criteria:** <br>
1. The user should see error message for location error "We are unable to retrieve your location."  <br>
2. The user should only be able to select visit times in today or future (// side note: looks like it only display two month for now)
3. Once the user has made a valid selection, the schedulePage should display the available appointment provider and times for the selected location and appointment type. <br>

### Scenario 6 Verify that "User" canNOT schedule a visit without entering required info
**Given**: "User" is on the "schedulePage" <br>
**When**: "User" selects invalid appointment information <br>
**Then**: "User" should not be able to schedule the visit <br>

**Acceptance Criteria:** <br>
1. The user should see error message for location error "We are unable to retrieve your location."  <br>
2. The user should only be able to select visit times in today or future (// side note: looks like it only display two month for now)
3. Once the user has made a valid selection, the schedulePage should display the available appointment provider and times for the selected location and appointment type. <br>

### Scenario 7: Verify that "User" can see Health Insurance Acceptance and cost info
**Given**: "User" see provider list after selecting vist info <br>
**When**: "User" clicks on the "Info | $" icon <br>
**Then**: "User" can see Health Insurance Acceptance and cost info <br>

**Acceptance Criteria:** <br>
1. User should see Health Insurance Acceptance and cost info after click "Info | $" icon <br>

### Scenario 8: Verify that "User" can view clinic services list
**Given**: "User" see provider list after selecting vist info <br>
**When**: "User" clicks on the "View Clinic Services" link <br>
**Then**: "User" can see services provided by this clinic <br>

**Acceptance Criteria:** <br>
1. User should see Health Insurance Acceptance and cost info after click "Info | $" icon <br>

### Scenario 9: Verify that "User" can view clinic location from GoogleMap
**Given**: "User" see provider list after selecting vist info <br>
**When**: "User" clicks on the "Map" icon <br>
**And**: "User" navigated to GoogleMap <br>
**Then** "User"can see services provided address in GoogleMap <br>

### Scenario 10: Verify that "User" can view clinic location from GoogleMap
**Given**: "User" see provider list after selecting vist info <br>
**When**: "User" clicks on the "Map" icon <br>
**And**: "User" navigated to GoogleMap <br>
**Then** "User"can see services provided address in GoogleMap <br>

### Scenario 11: Verify system timeout after user inactivity
**Given**: system timeout after "User" not interacted in the "Schedule Page" for "20" minutes <br>
**When**: "User" perform any operation after system timeout <br>
**Then**: "User" should refresh web page <br>
**Then** "User" can interact with system again <br>

**Acceptance Criteria:** <br>
1. System should timeout after 'XX' minutes of user inactivity <br>
 <br>
 <br>
 <br>


# Part 2__Automation Instructions
