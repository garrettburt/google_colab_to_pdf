# google_colab_to_pdf


## Usage

Past the below code into the last cell of your Google Colab .ipynb file

```python
# Replace FOLDERLOCATION to have the folder location of your Colab File
notebook_path_folder = '/content/drive/My Drive/FOLDERLOCATION/'
# Replace this with the current name of your .ipynb file
file_name_input = 'filename.ipynb'

#%%capture
!wget -nc https://raw.githubusercontent.com/garrettburt/google_colab_to_pdf/master/colab_pdf.py
from colab_pdf import colab_pdf
colab_pdf(file_name = file_name_input, notebookpath = notebook_path_folder)
```
