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

### 9. Check your Folder Data

```
!ls Drive/test
```

### 10. Make zip file of your Data

```
from google.colab import files
import zipfile
import sys
foldername = 'your folder or filename'
zipfile.ZipFile('Drive/'+foldername + '.zip', 'w', zipfile.ZIP_DEFLATED)
```

### 11. Downloading the data from the colab

```
from google.colab import files
files.download('Drive/test.zip')
```


### other src:
- https://juejin.im/post/5c05e1bc518825689f1b4948#heading-31
