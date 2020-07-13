# ACM-Grand-Challenge-2020-BioMedia
ACM Grand Challenge 2020 BioMedia

# Sperm
biomedia-2020

# Tasks

The first two tasks relate to predicting common measurements used for semen quality assessment, For both tasks, participants are asked to perform video analysis over single frame analysis.  
- **motility**: predict the percentage of progressive, non-progressive, and immotile sperm in a given video sample.  
- **morphology**: predict the percentage of sperm with head defects, midpiece defects, and tail defects.  

# DataSet

https://github.com/simula/biomedia-2020/wiki/Dataset  

VISEM contains five CSV files:  
**semen_analysis_data.csv**: The results of standard semen analysis(标准精液分析).  
**fatty_acids_spermatozoa.csv**: The levels of several fatty acids in the spermatozoa of the participants(几种脂肪酸水平).  
**fatty_acids_serum.csv**: The serum levels of the fatty acids of the phospholipids (measured from the blood of the participant)(磷脂脂肪酸水平).  
**sex_hormones.csv**: The serum levels of sex hormones measured in the blood of the participants(性激素水平).  
**study_participant_related_data.csv**: General information about the participants such as age, abstinence time and Body Mass Index (BMI)(参与者一般信息：年龄、禁欲时间和体重指数等).  
**videos.csv**: Overview of which video-file belongs to what participants(哪个视频文件属于哪些参与者).  

# Metrics

Mean squared error, mean absolute error and the root mean squared error. 


# Methods

Lasso、LightGBM、Xgboost


# Results

**Motility**
Task | Mae | Mse | Rmse
----- |  ---- | ----- | -----
Non-progressive sperm motility | 6.99754 | 81.37438 | 8.92189
Progressive motility | 10.34852 | 171.49138 | 13.06471
Immotile sperm | 8.56650 | 180.13383 | 13.38379
Mean | 8.63752 | 144.33320 | 11.79013  



**Morphology**
Task | Mae | Mse | Rmse
----- |  ---- | ----- | -----
Head defects | 1.45439 | 4.15771 | 2.03593
Midpiece and neck defects | 7.78641 | 92.97207 | 9.63498
Tail defects | 5.43461 | 66.92127 | 8.14526
Mean | 4.89180 | 54.68368 | 6.60539

