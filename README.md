# ClearMap_data

### annotation data
The original data was downloaded by 

```bash
wget https://idiscodotinfo.files.wordpress.com/2016/05/clearmap_ressources_mouse_brain.zip
```

I then replace the spaces in the fold names to "_" and put the data in [`osf`](https://osf.io/c7qm6/).

You can download by:

```bash
curl -O -J -L https://osf.io/c7qm6/download
```

### test data

test data was in `osf` as well: https://osf.io/t6nhm/
download using [osfclient](https://github.com/osfclient/osfclient)

```bash
pip install osfclient
osf -p t6nhm clone

# unzip the data, data was in .7z format
conda install -c bioconda p7zip

# x will maintain the folder structure, and unzip 001 will unzip all the other 002,003..
# the 7z files are splitted.

7za x haloperidol.7z.001
7za x saline.7z.001

```
