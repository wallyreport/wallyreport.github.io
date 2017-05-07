```bash
#!/bin/sh
# file name: mkmdlinks.sh i.e. "Make Markdown Links"
# Creates a markdown formated menu of links
# base on the list of files with md extensions
# in the directory

rm $1
echo "#" $1 "\n" >> temp.txt

for f in `ls *.md`;
do
	echo "- ["$f"]("$f")" >> temp.txt
done

mv temp.txt $1
```
