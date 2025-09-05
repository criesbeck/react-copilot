# Name

- The app is called TeamTime.

# Users

- Users are software development teams who do mob programming.

# Value proposition

An easy to use rotation timer for mob programming sessions with drivers and navigators.

# Key features
Mobile-friendly one-screen design with 
  - large timer
  - one large button to start and stop the timer
  - a list of the team members, in shuffled order, with a checkmark next to each name, and the name of the current driver team clearly highlighted
Simple management operations:
  - You can tap names to uncheck them and they will be skipped in the rotation.
  - At the start of a rotation, you can bump the rotation time for the remainder of the session up or down in one-minute increments. 
Alert features:
  - A beep sounds when one minute is left in the current turn.
  - The timer changes color when one minute is left.
  - An alarm sounds when time is up.

# Example scenario

Here is an example session.

- Alice, Bob, Cathy, and Dave are a team of developers.
- Alice, Cathy, and Dave meet to do mob programming for 90 minutes.
- Alice starts the app on her phone. 
- It shows a countdown timer, set to 10 minutes, a start button, and a shuffled list of team member names with checkmarks.
- The first name is highlighted. It happens to be Bob.
- Alice unchecks Bob because he is not there. The highlight moves to Dave.
- Dave sits at the keyboard and starts the timer. He begins entering code suggested by the other team members. 
- Pizza arrives, so Dave stops the timer and grabs a slice. After a few minutes, he starts the timer to continue his turn.
- A beep at 9 minutes warns the team is almost time to rotate.
- Whem time goes to zero, an alarm sounds. Dave stops. The highlight moves to Cathy
- Cathy taps the start button to begin her turn.

# Coding notes

- Use setInterval() to implement the timer.
- Use AudioContext to play sounds.
- Define and import a MockAudioContext class for unit testing sounds. 

# Testing notes
- Define unit tests for skipping team members in the rotation.
- Define unit tests for when Start and Stop should appear.
- Define unit tests for when sounds should happen.
