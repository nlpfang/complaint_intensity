# Analyzing the Intensity of Complaints on Social Media
The official implementation of findings of NAACL 2022 paper ''[Analyzing the Intensity of Complaints on Social Media](https://arxiv.org/abs/2204.09366)''. Here, we release the annotated corpus and code for this work.

## Our annotated corpus
This Weibo data is collected from August 2020 to May 2021 through the official API, which contains 3103 posts, Our Weibo dataset can be found at `Data`folder. For more details about the Weibo dataset, please contact [fangming@smail.nju.edu.cn](fangming@smail.nju.edu.cn). Thanks!

### About our corpus

In this work, we create the post complaint intensity dataset, where intensity values are between -1 and +1. Data collection, preprocessing and annotation process of the data are discussed in detail in our paper. The statistics of our corpus are as follows:  

|                                                                **Hashtag**                                                               | **Num.** |
|:----------------------------------------------------------------------------------------------------------------------------------------:|----------|
| #代表建议让学生在校内完成家庭作业# (#The representative suggested that students should complete their homework on campus#)                 | 762      |
| #江苏明确教师不得用手机布置作业# (#Jiangsu Province makes it clear that teachers are not allowed to use mobile phones to assign homework#) | 534      |
| #院士不建议普通孩子学奥数# (#Academician does not recommend ordinary children to learn Mathematical Olympiad#)                             | 627      |
| #西安外国语大学封闭管理# (#Close management of Xi'an International Studies University#)                                                    | 598      |
| #人大法硕复试30余人成绩0分# (#More than 30 people scored 0 in the postgraduate examination of law at Renmin University#)                   | 582      |

### Corpus format

+ Preprocessing:
  
    + For each post, we filtered out posts with less than 10 words and more than 200 words. And we removed the name of the author, loca-
tion tags, and URLs. 
    + We combine Weibo posts from different hashtags together and then split them into 80% for training, 10% for validation, and 10% for test.
    
    
+ All annotated post are stored in `data.csv` file under `Data` folder. There are two columns "post" and "intensity" respectively, where "post" is the post after preprocessing, and "intensity" is the complaint intensity corresponding to this post.  
   
<br/>   
Code will be uploaded soon.
