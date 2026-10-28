# Baseball Practice Planner — Test Log

**Project:** AI 101 Midterm — Baseball Practice Planner

**Website:** https://maxhansen7.github.io/baseball-practice-planner/

**Testing Date:** October 27, 2026

## Test 1: Normal Input

**Steps:**
1. Select Hitting.
2. Enter October 27, 2026.
3. Enter 30 minutes.
4. Click Add Practice.

**Expected Result:** The hitting practice appears in the schedule.

**Actual Result:** The hitting practice appeared with the correct date and duration and a Mark Complete button.

**Result: PASS**

## Test 2: Invalid Input

**Steps:**
1. Select Fielding.
2. Enter October 27, 2026.
3. Enter 0 minutes.
4. Click Add Practice.

**Expected Result:** The website rejects the invalid duration.

**Actual Result:** The browser displayed a warning stating that the value must be greater than or equal to 1.

**Result: PASS**

## Test 3: Repeated Use

**Steps:**
1. Add a Hitting practice for 30 minutes.
2. Add a Fielding practice for 30 minutes.
3. Add a Throwing practice for 20 minutes.
4. Check the Practice Schedule.

**Expected Result:** Multiple practices appear without deleting earlier activities.

**Actual Result:** All three practices appeared in the schedule in date order.

**Result: PASS**

## Test 4: Keyboard Accessibility

**Steps:**
1. Enter valid practice information.
2. Use Tab to navigate through the form.
3. Navigate to Add Practice.
4. Press Enter.

**Expected Result:** The form can be submitted using the keyboard.

**Actual Result:** Keyboard navigation initially stopped after moving to the date field. After troubleshooting Mac keyboard navigation, Tab navigation worked and Enter submitted the practice.

**Result: PASS**

## Test 5: Narrow-Screen Test

**Steps:**
1. Open the live website in Safari.
2. Enter Responsive Design Mode.
3. Set the screen to an iPhone-sized resolution of 393 × 852.
4. Check the layout and add a practice.

**Expected Result:** The website fits the narrow screen and allows practices to be added.

**Actual Result:** The form and buttons were visible without horizontal clipping, and a practice was successfully added.

**Result: PASS**

## Troubleshooting and Retest

**Problem:** During keyboard testing, Tab initially moved only to the Practice Date field.

**Action Taken:** Checked Safari and macOS keyboard navigation settings and repeated the test.

**Retest:** Successfully navigated to Add Practice using Tab and submitted using Enter.

**Final Result: PASS**

**Note:** This was a keyboard navigation troubleshooting step, not a confirmed source-code change.

## Known Limitation

Practice activities disappear after refreshing the webpage because permanent browser storage has not been implemented.
