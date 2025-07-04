🧠 MindSharp: The Soft Skills Guessing Game
MindSharp is a fun and educational web-based number guessing game designed to sharpen your logical thinking while promoting important soft skills such as problem solving, patience, and a growth mindset.

📋 Overview
Players try to guess a randomly selected number between 1 and 100 within 10 attempts. After each guess, the game provides feedback, tracks progress, and encourages soft skill development through motivational messaging.

🚀 Features
🎮 Game Mechanics
Random number between 1 and 100.

Max 10 attempts allowed.

Hints guide players toward the correct number.

Success and failure messages reinforce learning.

🌟 Soft Skills Emphasis
Feedback is framed to promote persistence, critical thinking, and resilience.

Visual cards explain the relevance of problem solving, patience, and growth mindset.

📱 Responsive Design
Fully mobile-optimized.

Adapts layout for smaller screen sizes using media queries.

🛠️ Technologies Used
Tech	Purpose
HTML5	Structure of the web page
CSS3	Styling and responsiveness
JavaScript (Vanilla)	Game logic and interactivity
CSS Variables (:root)	Centralized theme color management

📂 File Structure
This is a single-page application (SPA), so all the logic, layout, and styles are self-contained in one file:

text
Copy
Edit
index.html
🔧 How It Works
1. Initialization
On load, a random number is generated between 1 and 100.

The number of attempts starts at 0.

2. User Input
User enters a number and submits via the button or Enter key.

Input is validated to ensure it's between 1 and 100.

3. Game Logic
Compares the input with the target number.

Gives feedback:

Too high / too low hints.

Success message if correct.

Game over message if attempts run out.

Tracks and displays progress using a progress bar.

4. Restart
On win or loss, a “Play Again” button resets the game state.

⚠️ Fix Needed
There's a JavaScript syntax error in your code:

❌ Incorrect (missing backticks + quotes):
javascript
Copy
Edit
showFeedback(🎯 Perfect! You guessed the number in ${attempts} attempts!, 'success');
✅ Fix it using template literals (backticks):
javascript
Copy
Edit
showFeedback(`🎯 Perfect! You guessed the number in ${attempts} attempts!`, 'success');
Also fix these:

javascript
Copy
Edit
showFeedback(`"Success is no accident. It's the result of your persistence and effort." - Now apply this to your soft skills!`, 'hint');

showFeedback(`Game over. The number was ${targetNumber}. Remember, perseverance is key to mastering any skill.`, 'error');

showFeedback(`Your guess is too low. Try a higher number. You're honing your observation skills!`, 'hint');

showFeedback(`Your guess is too high. Try a lower number. Great job continuing to analyze and adjust!`, 'hint');
🖼️ Assets
You’re using placeholder images from https://placehold.co. These can be replaced with themed illustrations or icons related to each soft skill.

🧩 Future Enhancements (Optional)
Add localStorage to track best scores.

Include multiple difficulty levels.

Include soft skill quizzes after each round.

Make it a PWA (Progressive Web App) for offline play.
