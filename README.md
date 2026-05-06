# BreizhCrops Crop Classification

This 


### Code and Data

The code is available at [COMP0173_Crop_Classiciation](COMP0173_Crop_Classification.ipynb), produced in Google Colab. To reproduce the results:
1. Create a Google Drive folder entitled 'COMP0173_Applying_New_Context' in your main drive; within this, create a folder entitled 'data' (this will match the data path to that used in the code: DATA_PATH = '/content/drive/MyDrive/COMP0173_Applying_New_Context/data'). The code for mounting the drive is available in the .ipynb file.
2. Run code cell 1 (!pip install breizhcrops)
3. Due to an unresolvable compatibility issue, the datasets must then be downloaded in the following way:
   - In code cell 2, change "dataset = bzh.BreizhCrops("frh03", level="L2A")" to "dataset = bzh.BreizhCrops("frh01", level="L2A")". Run this cell.
   - In code cell 3, change "REGIONS_TO_EXTRACT: List[str] = ["frh04"]" to "REGIONS_TO_EXTRACT: List[str] = ["frh01"]" and run this cell to locally download (X_raw_frh01.npy and y_raw_frh01.npy)
   - Repeat this process for frh02, frh03, and frh04. You should now have files named X_raw_frh0X.npy and y_raw_frh0X.npy for X=1,2,3,4 locally downloaded; if not, please change the names to this form.
   - Upload all files to the "data" folder in your Google Drive.
   - Mount Google Drive using code cell 4, and run code cell 5 to confirm the following output:
```text
Listing files in: /content/drive/MyDrive/COMP0173_Applying_New_Context/data

y_raw_frh01.npy
y_raw_frh02.npy
X_raw_frh02.npy
X_raw_frh01.npy
y_raw_frh04.npy
X_raw_frh04.npy
X_raw_frh03.npy
y_raw_frh03.npy
```


The remainder of the .ipynb file will now be reproducible.

________________

Code documenting my reproduction of the initial baseline is available at [COMP0173_Baseline_Replication](COMP0173_Baseline_Replication.ipynb); instructions for replication of this code is included in the .ipynb file.


  
