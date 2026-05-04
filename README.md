# DSA 210 Project Milestone 2:
# The Effect of Animated Thumbnails on Video Game Mods Metrics

My goal is to uncover the effectiveness of animated thumbnails on various mod metrics within the Steam Workshop platform. ML methods were applied at this time.

## Machine Learning

Linear regression was applied to the personal dataset exclusive feature Cumulative Subscribers, over 60 days. The animated thumbnails created a regression line higher than what was obtained from static thumbnails, and these two lines do not intersect.

![img1](ML%20Charts/Animated_Thumbnail_LR.png)
![img2](ML%20Charts/Static_Thumbnail_LR.png)
![img3](ML%20Charts/LR_Comparison.png)

What we can also observe is that the mean subscriber count per day from animated thumbnails is higher than those of static thumbnails, in all 60 days.

![img4](ML%20Charts/Scatterplots_Comparison.png)
