#What regular expressions do you use to extract all the dates in this blurb: http://bit.ly/regexexercise2 and to put them into the following format YYYY-MM-DD?

# The following expression should find all three variants of date formats:

# /d matches any single digit (0-9). with [1,2] matching the previous token between one and two times, followed by a punctuation to match any character. This is repeated once more. Lastly comes a punctuation mark followed by *? Which matches the beforehand token zero or unlimited, or as few times as possible. /d[4] matches the previous token four times:

\d{1,2}.\d{1,2}.*?\d{4}
