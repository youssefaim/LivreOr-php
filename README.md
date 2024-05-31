# LivreOr-php
HTML Form:
The code begins with an HTML form that allows users to submit their comments.
The form has the following input fields:
Name: A text input field where users can enter their name.
Mail: Another text input field for users to provide their email address.
Comments: A textarea where users can write their comments about the website.
There are two buttons within the form:
“Envoyer” (Submit): When clicked, this button triggers the form submission.
“Afficher les avis” (Show Reviews): When clicked, this button displays the last five comments left by site visitors.
PHP Processing:
The PHP code processes the form data after submission.
If the “Envoyer” button is clicked:
It checks if the user has provided a name, email, and comments.
If all fields are provided, it echoes a thank-you message along with the user’s name.
It appends the user’s information (name, email, timestamp, and comments) to a file named “livre2.txt”.
If the “Afficher les avis” button is clicked:
It reads the contents of the “livre2.txt” file.
The comments are stored in a multidimensional array.
The array is reversed to display the most recent comments first.
The code then generates an HTML table displaying the last five comments:
Each row includes the comment number, commenter’s name, email, timestamp, and the actual comment.
If there are fewer than five comments, it displays only the available comments.
If neither button is clicked, it prompts users to leave their comments and click “Envoyer.”
Styling:
The background color of the webpage is set to “#ffcc00” (a light yellow shade).
