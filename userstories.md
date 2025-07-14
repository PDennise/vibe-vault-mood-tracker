| ID  | User Story List                                                                                                      |
|-----|----------------------------------------------------------------------------------------------------------------------|
| US1 | As a user, I want to enter my mood as a text description, so that I can track how I feel.                            |
| US2 | As a user, I want the app to analyze the sentiment of my mood text, so that I can understand my emotional state.     |
| US3 | As a user, I want my mood entries to be saved automatically, so that I don’t lose them.                              |
| US4 | As a user, I want to view my past mood entries in a list, so that I can reflect on my mood history.                  |
| US5 | As a user, I want to see a graph of my mood over time, so that I can identify trends.                                |
| US6 | As a user, I want the app to handle empty states gracefully, so that I don't see errors.                             |
| US7 | As a user, I want each mood entry to include the date, so that I know when I wrote it.                               |
| US8 | As a user, I want to enter my mood as a text description, so that I can track how I feel.                            |
| US9 | As a user, I want the app to analyze the sentiment of my mood text, so that I can understand my emotional state.     |
| US10 | As a user, I want my mood entries to be saved automatically, so that I don’t lose them.                             |
| US11 | As a user, I want to view my past mood entries in a list, so that I can reflect on my mood history.                 |
| US12 | As a user, I want to see a graph of my mood over time, so that I can identify trends.                               |
| US13 | As a user, I want the app to handle empty states gracefully, so that I don't see errors.                            |
| US14 | As a user, I want to export my mood data to CSV format and have my moods classified into common emotions            |
|        so that I can better understand my emotional patterns and analyze them using spreadsheet software.                  |
| US15 | As a user, I want each mood entry to include the date, so that I know when I wrote it.                              |
| US16 | As a developer, I want to add unit tests, so that I can ensure the code is working as expected and catch bugs early.|
|------|---------------------------------------------------------------------------------------------------------------------|

# ✅ User Stories, Acceptance Criteria & Tasks – Mood Tracker

---

## US1 – Mood Entry

**User Story:**  
As a user, I want to enter my mood as a text description, so that I can track how I feel.

**Acceptance Criteria:**
- The user is prompted to write about their mood.
- The input is saved and acknowledged with a success message.

**Tasks:**
- [ ] Prompt user for mood input.
- [ ] Store mood in a variable.
- [ ] Display confirmation message.

|------|---------------------------------------------------------------------------------------------|

## US2 – Sentiment Analysis

**User Story:**  
As a user, I want the app to analyze the sentiment of my mood text, so that I can understand my emotional state.

**Acceptance Criteria:**
- The text is analyzed using NLP.
- A polarity and subjectivity score is returned.

**Tasks:**
- [ ] Use TextBlob to analyze the text.
- [ ] Extract `polarity` and `subjectivity` values.
- [ ] Display sentiment scores (optional).

|------|---------------------------------------------------------------------------------------------|

## US3 – Save to JSON

**User Story:**  
As a user, I want my mood entries to be saved automatically, so that I don’t lose them.

**Acceptance Criteria:**
- Each entry is stored in a local JSON file.
- If the file does not exist, it is created.

**Tasks:**
- [ ] Create function to load JSON data.
- [ ] Append new entry to the list.
- [ ] Write updated list back to file.

|------|---------------------------------------------------------------------------------------------|

## US4 – View Entries

**User Story:**  
As a user, I want to view my past mood entries in a list, so I can reflect on my mood history.

**Acceptance Criteria:**
- User can select an option to see past entries.
- Entries are printed in a readable format.

**Tasks:**
- [ ] Create function to load and display JSON content.
- [ ] Format and print each entry (date, mood, sentiment).

|------|---------------------------------------------------------------------------------------------|

## US5 – Plot Mood Graph

**User Story:**  
As a user, I want to see a graph of my mood over time, so I can identify trends.

**Acceptance Criteria:**
- A line graph of polarity values over time is shown.
- The x-axis has dates, y-axis has polarity scores.

**Tasks:**
- [ ] Load moods from file.
- [ ] Extract dates and polarities.
- [ ] Use matplotlib to plot data.

|------|---------------------------------------------------------------------------------------------|

## US6 – Handle Empty State

**User Story:**  
As a user, I want the app to handle empty states gracefully, so I don’t see errors.

**Acceptance Criteria:**
- If no data exists, user sees a friendly message.
- App doesn’t crash when plotting or viewing entries.

**Tasks:**
- [ ] Check if mood list is empty before using it.
- [ ] Print fallback message if data is missing.

|------|---------------------------------------------------------------------------------------------|

## US7 – Timestamping

**User Story:**  
As a user, I want each mood entry to include the date, so I know when I wrote it.

**Acceptance Criteria:**
- Each mood entry has the current date in `YYYY-MM-DD` format.

**Tasks:**
- [ ] Use `datetime.now()` to get today’s date.
- [ ] Include date in saved JSON entry.

|------|---------------------------------------------------------------------------------------------|

## US8 – CLI Menu with Multiple Options

**User Story:**
As a user, I want a clear command-line menu to add mood entries, view past entries, or exit, so that navigation is simple and intuitive.

**Acceptance Criteria:**
- A menu is displayed on program start with options (Add, View, Exit).
- User can select options by typing corresponding numbers.
- Invalid choices prompt user to try again.

**Tasks:**
- [ ] Implement CLI menu with options.
- [ ] Validate user input for menu choices.
- [ ] Loop menu until user chooses to exit.

|------|---------------------------------------------------------------------------------------------|

## US9 – Input Validation: Prevent Empty Input

**User Story:**
As a user, I want the app to prevent saving empty mood entries, so that my data is meaningful.

**Acceptance Criteria:**
- If user inputs empty or whitespace-only mood text, app prompts for re-entry.
- Empty input is never saved to the data file.

**Tasks:**
- [ ]Add validation check for empty input.
- [ ]Display error message for invalid input.
- [ ]Loop until valid input is received.
|------|---------------------------------------------------------------------------------------------|

## US10 – Load Previous Entries at Startup

**User Story:**
As a user, I want the app to load existing mood entries automatically when started, so I can continue from where I left off.

**Acceptance Criteria:**
- Mood entries are loaded from JSON file on program start.
- If no file exists, start with empty data without errors.

**Tasks:**
- [ ] Implement loading function on startup.
- [ ] Handle missing or empty data file gracefully.

|------|---------------------------------------------------------------------------------------------|

## US11 – Clear Messages and Feedback

**User Story:**
As a user, I want clear feedback messages after each action, so I always know if my input was successful or if errors occurred.

**Acceptance Criteria:**
- Confirmation messages appear after saving data.
- Error messages appear for invalid inputs.
- Informational messages guide the user through actions.

Tasks:
- [ ] Add success messages after saving.
- [ ] Add error messages for invalid operations.
- [ ] Improve user prompts and feedback text.

|------|---------------------------------------------------------------------------------------------|

## US12 – Update or Delete Entry (Optional Stretch Goal)

**User Story:**
As a user, I want to be able to update or delete past mood entries, so I can correct mistakes or remove unwanted records.

**Acceptance Criteria:**
- User can select an entry to edit or delete.
- Changes are saved back to the JSON file.
- Deletion requests ask for confirmation.

Tasks:
- [ ] Implement listing with entry selection.
- [ ] Add update functionality.
- [ ] Add delete functionality with confirmation prompt.

|------|---------------------------------------------------------------------------------------------|

## US13 – Tag Moods Manually

**User Story:**
As a user, I want to tag moods with keywords (e.g. #happy, #anxious), so I can categorize my feelings more easily.

**Acceptance Criteria:**
- User can input optional tags during mood entry.
- Tags are saved with the mood entry in JSON.

Tasks:
- [ ] Add prompt for mood tags on entry.
- [ ] Validate and save tags with entries.
- [ ] Display tags when viewing entries.

|------|---------------------------------------------------------------------------------------------|

## US14 – Export Data to CSV

**User Story:**
As a user, I want to export my mood data to CSV format and have my moods classified into common emotions (like happy, sad, anxious), so that I can better understand my emotional patterns and analyze them using spreadsheet software.

**Acceptance Criteria:**
- User can export all mood entries to CSV file.
- Exported file includes date, mood text, polarity, subjectivity, and any tags.

**Tasks:**
- [ ] Implement CSV export function.
- [ ] Add menu option for export.
- [ ] Validate successful file writing and notify user on success or failure.

|------|---------------------------------------------------------------------------------------------|

## US15 – Track Mood by Time of Day

**User Story:**
As a user, I want to optionally record the time of day when I enter my mood, so I can see patterns across different times.

**Acceptance Criteria:**
- Mood entries include time in addition to date.
- Graph or listing can display mood by time.

**Tasks:**
- [ ] Capture current time on entry.
- [ ] Save time info in data model.
- [ ] Update display functions to show time.

|------|---------------------------------------------------------------------------------------------|

## US16 - Implement unit testing for core functions

**User Story:**
As a developer, I want to add unit tests, so that I can ensure the code is working as expected and catch bugs early.

**Acceptance Criteria:**
- At least key functions (e.g., mood analysis, saving/loading data) have test cases.
- Tests return pass/fail results in the CLI.
- Developer can run tests with a single command (e.g., python -m unittest).

**Tasks:**
- [ ] Set up unittest or pytest.
- [ ] Write tests for key modules (e.g., mood_analyzer, mood_storage).
- [ ] Add test runner instructions to README.

|------|---------------------------------------------------------------------------------------------|

**MoSCoW List**

| ID  | User Story - 🟥 Must Have                         |
| --- | --------------------------------------------------|
| US1 | Mood entry: Enter mood as text                    |
| US2 | Sentiment analysis with TextBlob                  |
| US3 | Save entries to JSON                              |
| US7 | Timestamp each entry with current date.           |
| US8  | CLI menu with multiple options (Add/View/Exit)   |
| US9  | Validation: Prevent empty input from being saved |
| US10 | Load previous entries at startup                 |



| ID  | User Story - 🟧 Should Have                                      |
| --- | -----------------------------------------------------------------|
| US4 | View past entries in a list                                      |
| US6 | Handle empty states gracefully (no crash if no data)             |
| US11 | Clear messages/feedback for each action                         |
| US12 | Allow user to update or delete an entry (optional stretch goal) |



| ID  | User Story - 🟩 Could Have                  |
| --- | --------------------------------------------|
| US5 | Plot mood graph with matplotlib             |
| US13 | Tag moods manually (e.g. #anxious, #happy) |
| US14 | Export data to CSV                         |
| US15 | Track mood by time of day                  |
| US16 | Implement unit testing for core functions  |



**Here's a breakdown of each category:**

**Must-have:**
These are essential requirements that are critical for the project's success. Without these, the project cannot be considered complete. 
**Should-have:**
These are important requirements that are highly desirable but not absolutely necessary for the project's core functionality. They should be included if possible, but can be postponed or dropped if necessary. 
**Could-have:**
These are desirable features that are nice to have but not essential. They can be included if time and resources allow, but are the first to be cut if necessary. 
**Won't-have:**
These are requirements that are not planned for the current project iteration or release. They may be considered for future iterations or not at all. 