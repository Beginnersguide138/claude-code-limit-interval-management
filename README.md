# Claude Code API Reset Timetable

This project is a static HTML page that displays a timetable for Claude Code API usage limit resets, which occur every **5 hours**.  
It is designed to help track reset times, remaining time until the next reset, and token usage status.

---

## Features

- **Fixed Base Time**:  
  The timetable is generated from a fixed UNIX timestamp `1755331200` as the base reset time.
  
- **5-Hour Intervals**:  
  All reset times are calculated in 5-hour increments from the base time.

- **Countdown Timer**:  
  Displays a live countdown to the next reset at the top of the page.

- **Progress Bar**:  
  Shows the elapsed percentage of the current 5-hour interval.

- **Theme Toggle**:  
  Switch between light and dark modes with proper color adjustments for readability.

- **Responsive Design**:  
  Works on both desktop and mobile devices, with a card view for smaller screens.

- **Date Jump Navigation**:  
  Quickly scroll to a specific date in the timetable.

- **Highlighting**:  
  Today's reset times are highlighted for quick reference.

- **Hide Past Times**:  
  Past reset times are automatically hidden from the table.

- **"Used" Checkbox**:  
  Each row has a checkbox to mark when the token for that interval has been used.  
  Checked rows are grayed out to indicate usage.

---

## How to Use

1. Open `index.html` in your browser.
2. The **Next Reset** field is pre-filled with the fixed base UNIX timestamp.
3. The timetable will auto-generate showing upcoming reset times.
4. Use the **checkboxes** to mark intervals where tokens have been used.
5. Toggle between **light** and **dark** themes as desired.
6. Use the **Jump to Date** field to navigate to a specific date in the table.

---

## Technical Details

- **HTML5**, **CSS3**, and **JavaScript** only — no external dependencies.
- Uses `setInterval` for real-time countdown and progress bar updates.
- Dark mode styles are explicitly defined to ensure text remains visible.
- Responsive layout achieved with CSS media queries.

---

## License

This project is licensed under the MIT License.
