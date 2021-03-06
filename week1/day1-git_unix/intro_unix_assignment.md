# Basic Practicing with Unix

This assignment will give you some practice navigating around the terminal
and using some of the commands we have talked about. Because we will be
working with the terminal throughout the entirety of this program and you
will be building up familiarity with it throughout the program, this
assignment will be fairly brief.

1.) Open up your terminal and navigate to your home directory.

2.) In your home directory, create a new directory called
`test_directory`.

3.) Navigate into `test_directory`, and print the working directory
to the screen. Is the pathname printed to the screen an absolute path
or relative path?

4.) Create two files, calling them `test_file1.txt` and `test_file2.txt`.

5.) Use `ls` to make sure that the files are in fact in the directory.

6.) Copy `test_file1.txt` to a new file, calling it `test_file3.txt`. How
many files are there in your directory now?

7.) Rename `test_file3.txt` to `test_file4.txt`. How many files are there
in your directory now?

8.) Within `test_directory`, create a new directory called `inner_directory`.

9.) In one command, move all of the files from `test_directory` into the
`inner_directory`.

10.) In one command, delete `inner_directory` and all its contents.

11.) Navigate back to your root directory, and delete `test_directory` using
`rmdir`. Why does `rmdir` work here (**Hint**: think about what's left in
`test_directory`)?

# Intermediate Practicing with Unix

0.) You will be using some new commands in the steps below. Read the manual for these new commands: `less`, `grep`, and `sort`. You can access the manual using the `man` command. E.g. run `man less` to read the manual for the `less` command. (Tip: To exit `man`, press 'q' on your keyboard.)

1.) Use `cd` to navigate into the `data/` directory. You should see two files: `2015_sp100.csv` and `plot_stock_prices.py`.

2.) Use `less` to peek at the file (`2015_sp100.csv`). It contains daily stock prices for stocks in the [S&P 100 Index](https://en.wikipedia.org/wiki/S%26P_100) for the year 2015. Notice the lines of the file are in random order.

3.) Use `grep` to print all the lines having prices for Google (symbol: GOOG). Use *bash file redirection* to store these GOOG lines into a file named `2015_goog.csv`.

4.) Use `sort` to sort the lines in `2015_goog.csv`. Use *bash file redirection* to store the sorted lines into a new file named `2015_goog_sorted.csv`.

5.) The Python script `plot_stock_prices.py` knows how to plot stock price data files. Run that script, and use *bash file redirection* to input the file `2015_goog_sorted.csv` into the script's *stdin*.

6.) Combine steps 3, 4, and 5 above into one command using *bash pipes*.
