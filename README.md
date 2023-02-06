 Init repo
_👀 This is a possible solution that  **AI-Exercise** x/y axis [🔗demo](https://github.com/natasa-plulikova/AI-Exercise)


## Anomaly detection

*Anomaly detection is a process in machine learning that identifies data points, events, and observations that deviate from a data set’s normal behavior.* 

anomaly detection use cases can be categorized into three types depending on the type of the data available. 
-Supervised anomaly detection aims to learn a model by using labeled data that represents previous failures or anomalies. 
-In the unsupervised setting, no labeled data is provided. 
-The third category, semi-supervised anomaly detection, relies on a small amount of labeled data to validate and select the best performing model trained on normal data (or data with no anomalies). 


## Isolation Forests

Isolation forest (IF) is a machine learning algorithm for anomaly detection.Isolation Forest is based on the Decision Tree algorithm. And since there are no pre-defined labels here, it is an unsupervised model.


It isolates the outliers by randomly selecting a feature from the given set of features and then randomly selecting a split value between the max and min values of that feature.


**The idea behind Isolation Forest is that, on average, outliers will be closer to the root node (i.e. at a lower depth) than normal instances.**

![Alt text](https://github.com/Andrea-Monserrat/Anomalies-detection/blob/main/IF.png)

Technically, this translates into the fact that, if we fit a decision tree on all the observations, outliers should be found closer to the root of the tree than “normal” instances.

▶︎ More info in the references.

## Install

```For this project I have decided to use H2O as the main library for ML.

Conda install:
 >>conda install -c h2oai h2o<<
```

## What is H2O?

H2O is a Java-based software for data modeling and general computing. The H2O software is many things, but the primary purpose of H2O is as a distributed (many machines), parallel (many CPUs), in memory (several hundred GBs Xmx) processing engine.

 🌟The advantage that H2O offered me over other packages was the use of very large data.  🌟
- this is the[🔗official documentation](https://docs.h2o.ai/h2o/latest-stable/h2o-py/docs/intro.html#:~:text=H2O%20from%20Python%20is%20a%20tool%20for%20rapidly,Java-based%20software%20for%20data%20modeling%20and%20general%20computing.)
-[Isolation Forest documentation](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/data-science/if.html?highlight=isolation%20forest)



## Future Proposal

Isolation forest with Scikit Learn to compare results of both algorithms.
[🔗official documentation](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.IsolationForest.html)

> ▶︎ Notes


 ▶︎ There are other things that I would like to try to improve the model, one of them is SHAP statistics. The hypothesis is that it could give me the importance feature for the exercise.[🔗idea] (https://medium.com/dataman-in-ai/explain-your-model-with-the-shap-values-bc36aac4de3d),(https://stats.stackexchange.com/questions/386558/feature-importance-in-isolation-forest)




## References for this project

-[What is anomaly detection?](https://developer.ibm.com/learningpaths/get-started-anomaly-detection-api/what-is-anomaly-detection/) 
-[Isolation Forest](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf)
-[Quantile Encoder: Tackling High Cardinality Categorical Features in Regression Problems](https://arxiv.org/pdf/2105.13783.pdf)



All new contributions and feedback are welcome! 
