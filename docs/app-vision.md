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
- Timer appears set to 10 minutes, with the names shuffled to show Bob, Dave, Cathy, and Alice.
- Alice unchecks Bob because he is absent. The highlight moves to Dave.
- Dave taps Start to start the timer, and begins entering code suggested by the other team members. 
- Pizza arrives, so Dave taps Stop.  After finishing a slice, he taps Start to continue his turn.
- A beep at 9 minutes warns the team is almost time to rotate.
- An alarm at 10 minutes tells Dave to stop. The highlight moves to Cathy, and the button changes to Start.
- Cathy taps Start to begin her turn.

# Coding notes

- Use setInterval() to implement the timer.
- Use AudioContext to play sounds.
- Define and import a MockAudioContext class for unit testing sounds. 

# Testing notes
- Define unit tests for skipping team members in the rotation.
- Define unit tests for when Start and Stop should appear.
- Define unit tests for when sounds should happen.
