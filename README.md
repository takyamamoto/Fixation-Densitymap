# Fixation Density Map
Fast Python implementation Generating Heatmaps from eye tracking data  

## Requirement
- Python == 3.6  
- OpenCV >= 3.0  
- tqdm

## Usage
Open `Fixpos2Densemap.py`  
Replace below with loading your data
```
fix_arr = np.random.randn(num_subjects,3)
fix_arr -= fix_arr.min()
fix_arr /= fix_arr.max()
fix_arr[:,0] *= W
fix_arr[:,1] *= H
```
Data shape must be `number of participate x 3(x, y, fixation)`  
fixation can be 1

## Demo
This image does **not** use actual human eye tracking data: this uses toy data  
<img src="https://github.com/takyamamoto/Fixation-Densitymap/blob/master/output.png" width=40%>

## Other implementation
[TobiasRoeddiger/GazePointHeatMap](https://github.com/TobiasRoeddiger/GazePointHeatMap): Easy to use Python command line based tool to generate a gaze point heat map from a csv file.  
[jjguy/heatmap](https://github.com/jjguy/heatmap): Python module to create heatmaps  
