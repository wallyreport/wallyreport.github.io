```bash
#!/bin/sh
# file name: appmdlinks.sh i.e. "Append Markdown Link"
# Add a markdown formated link to the menu of links
# use: appmdlinks.sh newfile.md menu.md


echo "- ["$1"]("$1")" >> $2
```
