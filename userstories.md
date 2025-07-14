| ID  | User Story List                                                                                |
|-----|---------------------------------------------------------------------------------------------|
| US1 | As a user, I want to enter my mood as a text description, so that I can track how I feel. |
| US2 | As a user, I want the app to analyze the sentiment of my mood text, so that I can understand my emotional state. |
| US3 | As a user, I want my mood entries to be saved automatically, so that I don’t lose them.    |
| US4 | As a user, I want to view my past mood entries in a list, so that I can reflect on my mood history. |
| US5 | As a user, I want to see a graph of my mood over time, so that I can identify trends.       |
| US6 | As a user, I want the app to handle empty states gracefully, so that I don't see errors.    |
| US7 | As a user, I want each mood entry to include the date, so that I know when I wrote it.      |
| US8 | As a user, I want to enter my mood as a text description, so that I can track how I feel. |
| US9 | As a user, I want the app to analyze the sentiment of my mood text, so that I can understand my emotional state. |
| US10 | As a user, I want my mood entries to be saved automatically, so that I don’t lose them.    |
| US11 | As a user, I want to view my past mood entries in a list, so that I can reflect on my mood history. |
| US12 | As a user, I want to see a graph of my mood over time, so that I can identify trends.       |
| US13 | As a user, I want the app to handle empty states gracefully, so that I don't see errors.    |
| US14 | As a user, I want each mood entry to include the date, so that I know when I wrote it.      |
| US15 | As a user, I want each mood entry to include the date, so that I know when I wrote it.      |
|------|---------------------------------------------------------------------------------------------|

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

