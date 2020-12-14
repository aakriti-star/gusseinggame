#!/usr/bin/env bash

function greet {
	echo "Congratulations! You have given the right answer!"
}
control=0
while [[ $control -eq 0 ]]
do
	echo "Type the number of files in current directory:"
	read response
	echo "You entered : $response"
	numfiles=(*)
	numfiles=${#numfiles[@]}
	echo "the number of files is: $numfiles"
	if [[ response -eq numfiles ]]
	then
		greet
		control=1
	elif [[ response -gt numfiles ]]
	then
		echo "Incorrect guessed number too high,Try again"
	else
		echo "Incorrect guessed number too low,Try again"
	fi
done
