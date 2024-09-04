# google_colab_to_pdf


## Usage

Paste the below code into the last cell of your Google Colab .ipynb file

```python
# Replace FOLDERLOCATION to have the folder location of your Colab File
notebook_path_folder = '/content/drive/My Drive/FOLDERLOCATION/'
# Replace this with the current name of your .ipynb file
file_name_input = 'FILENAME.ipynb'

#%%capture
!wget -nc https://raw.githubusercontent.com/garrettburt/google_colab_to_pdf/master/colab_pdf.py
from colab_pdf import colab_pdf
colab_pdf(file_name = file_name_input, notebookpath = notebook_path_folder)
```

* Replace the `FOLDERLOCATION` string with the location of the .ipynb file in your Google Drive
* Replace the `FILENAME` string with the exact name of your .ipynb file

## Notes

* Google drive default mounting location: 'content/drive/My Drive/'
* .pdf File will be written to the same location as your .ipynb file
* .pdf conversion uses LaTeX for conversion
