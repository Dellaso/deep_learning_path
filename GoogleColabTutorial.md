# Google Colab Tutorial

### 1. if the .py is in the /content folder, how import it
```
from filebasicop import addnum
addnum(2)
```

### 2. if the .py is in  the /content/my_project, how import it
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

### 5.mount google drive
```
from google.colab import drive
drive.mount('/content/drive/')
```

### 6. remove file
```
!rm hello.py
or
rm -rf custom_data_cnn.py
or
!rm -rf _config.yml updated_custom_data_cnn.py
```

### 7. remove foler
```
!rm -rf own_data_cnn_implementation_keras/
```

### 8. create folder
```
!mkdir my_project
```
