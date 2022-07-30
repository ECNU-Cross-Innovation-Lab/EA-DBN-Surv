# EA-DBN--Surv
Innovative models of liver cancer survival prediction based on cancer historical data analysis and statistical modeling emerge in endlessly.  Machine learning methods especially deep learning methods of survival analysis has received higher attention than troditional methods, which has been studied by more and more scholars and has been proved to have extraordinary performance. As we all know, however, the premise of achieving good performance is that a deep learning model must undergo a lot of hyperparameter tuning work. Aiming at the problem that it is difficult for a deep learning model to find the globally optimal hyperparameter combination, this paper establishes an evolutionary deep belief network(EA-DBN-Surv) model using evolutionary algorithm (EA) to help a deep belief network (DBN) find the optimal hyperparametric combination, which is used to predict the survival time of liver cancer. EA-DBN-Surv uses EA to automate the optimization process of 10 hyperparameters required for modeling to improve a traditional deep learning prediction model. The survival data of liver cancer patients from The Surveillance, Epidemiology, and End Results Program of the National Cancer Institute (SEER) were used in our experiment, and the prediction effect was compared with some excellent survival prediction methods(including RSF, Cox-Time, Cox-CC, DeepSurv and DeepHit). The comparison methods are all based on deep learning except RSF. The experimental results show that the c-index of EA-DBN-Surv is 0.7755 with automatically found excellent hyperparameters, which reaches the average level within the scope of the models included in the comparison. Further, the prediction error index Brier score is reduced to 0.0250. Compared with other models, a decrease of about 3 times of prediction error is achieved while maintaining the accuracy of prediction.
# Code running
The liver cancer data used here is from the SEER database ,which names Incidence-SEER Research Data, 9 Registries, Nov 2020 Sub (1975-2018). The filtered and integrated data set of the official annotation file is saved in `rowdata.csv` . Two steps of EA-DBN--Surv model are stored in two files respectively：`main2_EA-DBN-Surv_step1.py` and `main3_EA-DBN-Surv_step2.py` Step1 mainly using  EA to iteratively find the most suitable hyperparametric combination for the model，and step2 mainly use the result of the step1 to configure our model, then train and predict on the data set. If you have any questions about how the code runs, you can contact us through the contact information in the documentation.
