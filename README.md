# Portfolio
DeepLearning Project Porfolio

***
<h2>#1. Project - Brain Tumor MRI Image Classification</h2> 

- Background
<p>Automated classification techniques using AI has consistently shown higher accuracy than manual classification.<br/>
  Hence, I used Deep Learning Algorithms to detect and classify brain tumor.</p>
<p>인공지능을 적용한 자동 분류 기법은 수동 분류 보다 높은 정확도를 보여왔습니다.<br/>
  따라서, 딥러닝 알고리즘을 사용하여 뇌종양 탐지 및 분류를 수행하였습니다.<p>

<h3>First try</h3>
- Summary
	<p>(1). Data Source<br/>
		- https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri</p>
	<p>(2). Data Preprocessing<br/>
		- ImageDataGenerator<br/>
      		- rescale: 1./255<br/>
      		- image size: (244, 244)<br/>
      		- color mode: rgb<br/>
	  	- class mode: sparse<br/></p>
	<p>(3). Model & Algorithms<br/>
	  	- Transfer Learning(TL)<br/>
      	  	        - MobileNet<br/>
	  	- Fine Tunning<br/>
		 	- Two hidden layers<br/>
      		        - Activate function: softmax<br/></p>
	<p>(4). Report<br/>
    	- loss: 0.0551, accuracy: 0.9850<br/>
	- val_loss: 1.2912, val_accuracy: 0.7487<br/>
	- Problems(문제): Overfitting and Low Accuracy(과대적합과 낮은 정확도)<br/></p>
 
![First_Train](https://github.com/kkyukkyu99/Portfolio/blob/main/First_Train.png)

<p>(5). Solution<br/>
- Solve overfitting problem by mixing and redistributing<br/>
- 데이터를 섞은 후 재분배하여 과대적합 문제를 해결한다.<br/></p>
