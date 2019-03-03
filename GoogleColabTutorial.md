# Google Colab Tutorial

### 1. if the .py is in the /content folder
```
from filebasicop import addnum
addnum(2)
```

### 2. if the .py is in  the /content/my_project
```
import sys
sys.path.insert(0, '/content/my_project')

from filebasicop import addnum
addnum(2)
```

### 3.get project from github
```
!git clone https://github.com/NVlabs/stylegan.git
```

### 4.upload file
```
from google.colab import files
uploaded = files.upload()
```

### 5.from google.colab import files
```
uploaded = files.upload()
```
