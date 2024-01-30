# Problem Set 3
You have accepted the invitation in GitHub Classroom. If you have not cloned your copy of the repo (`ps3-yourusername`) down to your own machine using GitHub Desktop, do so now.

You will be adding two new Python files to your repo:

* `ps3-part1.py`
* `ps3-part2.py`

You will then commit and push these new files to your repo on GitHub on the internet using GitHub Desktop. If you don't remember how to do this, please review the instructions in Problem Set 1.

If you are having trouble with GitHub come to office hours. 

**NEW!** I now expect you to write comments in your code! One point will be deducted if you do not provide comments explaining your code. Here's what I would like commented this time:

* Before every function, describe what it does and what its arguments are (if any).
* Before every variable, explain what value it is holding.

**NEW!** Now at the top of very files, you will include your honor pledge. The first four lines (comments) of every Python file should be this information. You will lose one point if you don't include these four lines.

* The name of the file.
* Your name.
* The date.
* "This code is my own work. I did not share my code or look at the code of another student. I did not consult ChatGPT, CoPilot, or another large language model."

## Part 1: Creating the perfect playlist

Using IDLE, open a new file and save it into your `ps3-yourusername` repo as `ps3-part1.py`. This program will contain the following:

1. A `main()` function that does the following:

* Create an empty list variable called `songlist`.
* Ask the user to enter a song they'd like in their playlist.
   - While they enter anything but "DONE", append that song to `songlist`, and ask for another song.
   - When they enter "DONE", stop asking them for more songs.
* Call the function `save_playlist()` passing in the `songlist` argument. (See below.)
* Call the function `print_playlist()`,


2. A function `save_playlist(mylist)` where `mylist` is a list variable. This function will do the following:

* Open a file called `my_playlist.txt` for writing.
* Write out each element in the list argument `mylist` to `my_playlist.txt`, where each song is preceded by `Song X: ` where `X` is the number of the song in the list. Remember to insert a new line after each song.
* Close `my_playlist.txt`

3. A function called `print_playlist()`, which does the following:

* Open the file `my_playlist.txt` for reading.
* Print out each line in the file. Remember to remove the new line or to suppress the automatic new line with `print()`!
* Close the file `my_playlist.txt`
* Print the number of songs in the playlist.

4. A call `main()` at the end of the program.

Here's a sample run of this program. Your output should look the same, but of course with different song names. You may use any fancy tricks with `print()` and string manipulation to make your output look like the sample.

<img src="part1.png" width=500>

## Part 2: Maximizing the value of a mathematical function  

A lot of what we do in the machine learning part of data science is try to maximize (or minimize) the value of some mathematical function $f(x)$. We will see later how this can help us provide the mostly likely predictions or classifications when we give input to a model.

One way to do this is to sweep through possible values for $x$ and see which one gives us the maxmimum (or minimum) output. You start by setting $x$ to be some small starting value, calculate $f(x)$ with that value of $x$, and then you slowly it increase $x$ by some regular interval, each time calculating $f(x)$ until you $x$ reaches some larger ending value. You keep track of which value of $x$ gave you the largest (or smallest) output. 

In this problem, we might want to find the value of $x$ that maximizes $f(x)$ where $f(x)$ is the quadratic function you all remember from high school:

$f(x) = ax^2 + bx + c$

The user will supply the values for $a$, $b$, and $c$. You will start with $x=0$ and increment $x$ by 0.01 until you after hit $x=1$. At the end, you will report the maximum value of $f(x)$ over $0 \le x \le 1$, and the value of $x$ that gave this maximum value.

Here's what your program should contain

1. Write a `main()` function that asks the user for $a$, $b$, and $c$.

2. Write a function called `max_while(a, b, c)` that calculates the value of $x$ that maximizes the quadratic function and then reports that maximum value and $x$ **USING A WHILE LOOP**.

3. Write a function called `max_while(a, b, c)` that calculates the value of $x$ that maximizes the quadratic function and then reports that maximum value and $x$ **USING A FOR LOOP**.

Your input and output messages must conform to the following examples: 

   

