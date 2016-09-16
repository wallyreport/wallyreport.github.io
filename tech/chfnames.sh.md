```bash
#!/bin/sh
# file name: chfnames.sh i.e. "Change File Name"
# Changes the names of all files in a directory
# Especially used to replace one character in each file name
# such as changing underscores to dots

for f in `ls`; 
	do 
		# new=$(echo $f | sed -e 's/_/\./g'); 
		# mv "$f" "$new"
		mv "$f" "${f//_/.}"; 
	done
```
