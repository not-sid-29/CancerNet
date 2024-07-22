# CancerNet: A Machine Learning Approach to detecting cancers <br>

### 1. Data Collection: 
- dataset used: [Multi-Cancer Dataset](https://www.kaggle.com/datasets/obulisainaren/multi-cancer/data)
- **Data Card**<br>
- The given dataset contains various kinds of images per type of cancers. <br>
- Details of the dataset are as below ⇓ <br>
 **Cancer	                   |  Classes	 |  Images** : <br>

Acute Lymphoblastic Leukemia |	4	  |   20000 <br>
Brain Cancer	             |   3	   |   15000 <br>
Breast Cancer	             |   2	   |  10000 <br>
Cervical Cancer	           |   5	   |   25000 <br>
Kidney Cancer	             |   2	   |   10000 <br>
Lung and Colon Cancer	     |   5	   |   25000 <br>
Lymphoma	                 |   3	   |   15000 <br>
Oral Cancer	               |   2	   |   10000 <br>

*Each Sub-Class contains 5000 Images*<br>

> - main classes = 8<br>
> - Sub-classes  = 26<br>
> - Format   = JPEG <br>
> - Dimensions  = 512x512px
---
### 2. Model Creation and Training: <br>
- Utilized an ensemble of *Vision Transformers*(ViT) models,
- Reduced `error_rate` to **0.03** (approx. 0.3%)
- Implemented GradientAccumulation to save around 10% GPU memory while training the models
---
### 3. Interface:<br>
- Created a simple gradio application to demonstrate the working of the app

---
**Future TODOs**:
- To employ a larger ensemble of pretrained to models to boost robustness of the overall predictions.
- Deploy the gradio app, and provide a better user interface
