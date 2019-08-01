```python
from sys import argv
import subprocess

worm = argv
name = str(worm[0])
print (name)

for i in range(0,10):
    folderName = 'Mal'+ str(i)
    subprocess.call(['md', folderName])
        #'mkdir' in linux
    subprocess.call(['copy',name,folderName])
        # 'cp' in linux
    
```
