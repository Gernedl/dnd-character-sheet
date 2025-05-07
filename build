#!/bin/sh

mkdir -p output

for file in data/*.json; do
    name=$(basename "$file" .json)
    sed "/\/\* #data# \*\//{
        r $file
    }" ./character-sheet.html > "output/${name}.html"
done

