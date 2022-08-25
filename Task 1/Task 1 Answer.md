1. A customer informed their consultant that they have developed several formulations of petrol that gives different characteristics of burning pattern. The formulations are obtaining by adding varying levels of additives that, for example, prevent engine knocking, gum prevention, stability in storage, and etc. However, a third party certification organisation would like to verify if the formulations are significantly different, and request for both physical and statistical proof. Since the formulations are confidential information, they are not named in the dataset.


Please assist the consultant in the area of statistical analysis by doing this;


a. A descriptive analysis of the additives (columns named as “a” to “i”), which must include summaries of findings (parametric/non-parametric). Correlation and ANOVA, if applicable, is a must.

Summary:

> i. Size: 214 sample and 9 features

> ii. All features are continuous variable.

> iii. no missing and infinity values in all features.

> iv. ![Screenshot 2022-08-23 225924](https://user-images.githubusercontent.com/67685003/186301733-6d1191e0-5089-43ad-8b3b-525e6a8a5488.jpg)
From this table, it shows that the mean and median (50%) of all feature are close to each other, this means all feature has a symmetrical distribution.

> v. 
> 
> ![Screenshot 2022-08-24 101053](https://user-images.githubusercontent.com/67685003/186302188-5dd60d24-8f12-475d-b72b-0174d4035014.jpg)

>The variance of all feature are quite low except for feature c and g. Feature a has the lowest variance with 0.000009 that means the difference between mean and other value are very small and this feature is consistent.

> vi. 
> 
> ![Task_1_corr](https://user-images.githubusercontent.com/67685003/186316499-4ab54439-a7ae-4358-8f17-529385a0f92d.jpg)

>From the heatmap of correlation of the data set, it shows that most of the feature are negetively correlated to other feature. Features a and g are highly positive correlated (0.81) with each other. On the other hands, features a and h are the weak correlated (-0.00039).

b. A graphical analysis of the additives, including a distribution study.

Summary:

> i. 

>![task_1_hist](https://user-images.githubusercontent.com/67685003/186647649-d81e870b-3a21-4fcd-b46e-67ee8dd2f7bd.jpg)

> From the histrogram of the features, feature a, b, c and g are normally distributed and feature f, h and i are right skewed distribution.

> ii.
>![task_1_box_a](https://user-images.githubusercontent.com/67685003/186667547-2b8dfeef-88c5-458b-8437-cebac2f3f3e1.jpg)
>![task_1_box_b](https://user-images.githubusercontent.com/67685003/186667595-9716388d-cab2-4bb5-8f1a-7710a6e5cbd3.jpg)
>![task_1_box_c](https://user-images.githubusercontent.com/67685003/186667634-8c37b244-3b23-4b05-8858-a73323f1af77.jpg)
>![task_1_box_d](https://user-images.githubusercontent.com/67685003/186667644-231641ec-084c-416f-9a87-fd28b9a30f10.jpg)
>![task_1_box_e](https://user-images.githubusercontent.com/67685003/186667647-ca6e8c0c-a42e-499d-911c-5be5ccf20b15.jpg)
>![task_1_box_f](https://user-images.githubusercontent.com/67685003/186667649-5930e778-29da-4195-9c4c-44a5b5e79a69.jpg)
>![task_1_box_g](https://user-images.githubusercontent.com/67685003/186667651-4c99d582-3eda-469f-918f-57241217f186.jpg)
>![task_1_box_h](https://user-images.githubusercontent.com/67685003/186667656-886cc4a7-1418-40bd-81f7-00ae873c09b0.jpg)
>![task_1_box_i](https://user-images.githubusercontent.com/67685003/186667660-c22e0b48-c455-40f3-a55b-36e3482b1398.jpg)

>The boxplot of the feature show that outliers occur in this data set. Most of the feature h value are 0.


c. A clustering test of your choice (unsupervised learning), to determine the distinctive number of formulations present in the dataset.


(refer attachment : ingredients.csv)
