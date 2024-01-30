# Problem Set 3
You have accepted the invitation in GitHub Classroom. If you have not cloned your copy of the repo (`ps3-yourusername`) down to your own machine using GitHub Desktop, do so now.

You will be adding three new Python files to your repo:

* `ps3-part1.py`
* `ps3-part2.py`
* `ps3-part3.py`

You will then commit and push these new files to your repo on GitHub on the internet using GitHub Desktop. If you don't remember how to do this, please review the instructions in Problem Set 1.

If you are having trouble with GitHub come to office hours. 

**NEW!** I now expect you to write comments in your code! One point will be deducted if you do not provide comments explaining your code. Here's what I would like commented this time:

* Before every function, describe what it does and what its arguments are (if any).
* Before every variable, explain what value it is holding.

**NEW!** Now at the top of very files, you will include your honor pledge. The first four lines (comments) of every Python file you should include this information. You will lose one point if you don't include the honor pledge.

* The name of the file.
* Your name.
* The date.
* "This code is my own work. I did not share my code or look at the code of another student. I did not consult ChatGPT, CoPilot or another large language model."

## Part 1: Creating the perfect playlist

Using IDLE, open a new file and save it into your `ps3-yourusername` repo as `ps3-part1.py`. This program will containt the following:

1. A `main()` function that does the following:

* Create an empty list variable called `songlist`.
* Ask the user to enter a song they'd like in their playlist.
   - While they enter anything but "DONE", append that song to `songlist`, and ask for another song.
   - When they enter "DONE", stop asking them for more songs.
* Call the function `save_playlist()` passing in the `songlist` argument. (See below.)
* Call the function `print_playlist()`,


1. A function `save_playlist(mylist)` where `mylist` is a list variable. This function will do the following:

* Open a file called `my_playlist.txt` for writing.
* Write out each element in the list argument `mylist` to `my_playlist.txt`, where each song is preceded by `Song X: ` where `X` is the number of the song in the list. Remember to insert a new line after each song.
* Close `my_playlist.txt`

2. A function called `print_playlist()`, which does the following:

* Open the file `my_playlist.txt` for reading.
* Print out each line in the file followed by `GREAT CHOICE!`
* Close the file `my_playlist.txt`

Here's an example run of this program.

   

