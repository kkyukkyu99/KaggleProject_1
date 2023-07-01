# Portfolio
DeepLearning Project Porfolio

***
<h2>#1. Project - Brain Tumor MRI Image Classification</h2> 

- Background
<p>Automated classification techniques using AI has consistently shown higher accuracy than manual classification.<br/>
  Hence, I used Deep Learning Algorithms to detect and classify brain tumor.</p>
<p>인공지능을 적용한 자동 분류 기법은 수동 분류 보다 높은 정확도를 보여왔습니다.<br/>
  따라서, 딥러닝 알고리즘을 사용하여 뇌종양 탐지 및 분류를 수행하였습니다.</p>

- Summary

  <h3>First try</h3>
	
	1. Data Source
		- https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri
	
	2. Data Preprocessing
		- ImageDataGenerator
      		- rescale: 1./255
      		- image size: (244, 244)
      		- color mode: rgb
			- class mode: sparse
	
	3. Model & Algorithms
	  	- Transfer Learning(TL)
			- MobileNet(CNN)
	  	- Fine Tunning
  			- Activate function: softmax
			- optimizer: Adam
            - learning_rate: 1e-5
	
	4. Report
    	- loss: 0.0551, accuracy: 0.9850
		- val_loss: 1.2912, val_accuracy: 0.7487
		- Problems(문제): Overfitting and Low Accuracy(과대적합과 낮은 정확도)<br>
		![First_Training_Result](https://github.com/kkyukkyu99/Portfolio/blob/main/First_Training_Result.png)
	
	5. Solution
		- Solve overfitting problem by mixing and redistributing
		- 데이터를 섞은 후 재분배하여 과대적합 문제를 해결한다.

  <h3>Second try</h3>
  
  	6. Report
  	   	- loss: 0.0258, accuracy: 0.9925
  	   	- val_loss: 0.0386, val_accuracy: 0.9889<br>
		![Second_Training_Result](https://github.com/kkyukkyu99/Portfolio/blob/main/Second_Training_Result.png)
