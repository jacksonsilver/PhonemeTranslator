# PhonemeTranslator
A tool for measuring words based on their phonetic "harshness". The user provides input words, phenomes and their corresponding harshness values, and is given a file containing the data pertaining to each word's overall harshness score based on their IPA pronounciation.

# SET UP
  1. Download code from GitHub and extract it to a secure directory.
  2. Ensure you have Python downloaded by running python --version in your terminal.
  3. In your terminal, run this line:
       pip install -r requirements.txt .
     This will ensure python has all of the necessary libraries used in the program

# PREPARE FILES
  1. Your map file should be an .xlsx file, where column 1 has phenomes found in IPA, and column 2 contains their corresponding value.
     The order in which you put the phenomes in the map file is the order in which they are processed for each word. Meaning if you have "ab",
     "a", "b" in your map file in that order, instances of "ab" together are checked for, and then "a" and "b" on their own are processed.
     Please note that "ab" and "ba" are considered different.
  2. Your input file should be an .xlsx file where column 1 has all of the words you would like to process. Besides the order in which they appear
     in the output file, the order in this input file does not matter.
  3. Your output file should be an empty .xlsx file. 

# TO RUN
  1. In your terminal, run this line:
        python translator.py "map file name".xlsx "input file name".xlsx "output file name".xlsx
  3. To run the test files, you can run:
        python translator.py eng map.xlsx input.xlsx output.xlsx
