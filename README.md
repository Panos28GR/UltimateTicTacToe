# UltimateTicTacToe
Artificial IntelligenceProject
Όδηγίες Εκτέλεσης:
1) Στο zip αρχείο του Project, μαζί με τον κώδικα περιέχεται και η μηχανή παιχνιδιού Ultimate Tic Tac Toe για τοπική χρήση
------------------------------------------------------------
2) Για compile σε Windows σύστημα εκτελούμε τις παρακάτω εντολές σε cmd:
cd [project folder]
dir /b /s *.java>sources.txt
md classes
javac -d classes @sources.txt
del sources.txt

Για compile σε Linux σύστημα εκτελούμε τις παρακάτω εντολές σε terminal:
cd [project folder]
mkdir bin/
javac -d bin/ `find ./ -name '*.java' -regex '^[./A-Za-z0-9]*$'`
------------------------------------------------------------
3) Για εκτέλεση χρησιμοποιούμε τις παρακάτω εντολές(σε οποιαδήποτε πλατφόρμα):
cd [project folder]
java -cp [project folder]\Engine\classes\com\theaigames\ bot.BotStarter bot.BotStarter 2>err.txt 1>out.txt
