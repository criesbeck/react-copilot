# Name

- The app is called TeamTime.

# Users

- Users are software development teams who do mob programming.

# Value proposition

- The app makes it easy to manage time and rotations during mob programming sessions.
- Key features include:
  - A countdown timer that can be started, stopped, and reset.
  - A stored list of team members with the ability to mark who is present.
  - A configurable rotation time for each team member.
  - Audible alerts when time is almost up and when time is up.
  - Automatic rotation of the active team member when time is up.

# Example scenario 1

This is an example scenario of how the app is used.

- Alice, Bob, Cathy, and Dave are a team of developers.
- Alice, Cathy, and Dave meet to do mob programming for 90 minutes.
- Alice opens the app on her phone.
- The first screen shows the team members with checkboxes next to each member, an editable field that says that 10 minutes is the rotation time, and a Continue button.
- Alice unchecks Bob because he is absent, then clicks Continue.
- The main screen appears with a big countdown timer set to the rotation time in minutes and seconds, a Start button, and the names of the three team members.
- The names are in shuffled order, with the first name highlighted.
- The team member whose is first clicks Start and begins entering code dictated by the other team members. 
- The timer begins counting down. The button name changes to Stop.
- One minute before time is up, the app beeps a warning and the timer begins to blink.
- When time is up, an alarm sounds, the timer stops, and the button name changes to Rotate.
- The team member who was typing stops and clicks Rotate.
- The list of names rotates to put the next team member first and highlighted. The timer resets to the rotation time. The button name changes to Start.
- The next team member clicks Start, and the process repeats.

# Coding notes

- Use setInterval() to implement the timer.
- Use AudioContext to play sounds.

# Testing notes
- Define unit tests for selecting team members present and rotation time.
- Define unit tests for Start and Stop.
- Define unit tests for when sounds happen and that Rotate appears when time runs out.
- Define and import a MockAudioContext class for unit testing sounds. 
