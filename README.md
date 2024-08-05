# Group26_AfricanFabricStyleGAN-Batiq
<h1 align="center">🌍 Generating African Batik Prints Using StyleGAN </h1>

<p align="justify">
  Welcome to the Batiq project! This repository contains the code and resources for generating African Batik prints using StyleGAN. We aim to leverage the power of deep learning to create unique and authentic Batik designs, celebrating the rich heritage of African culture.
</p>

## Project Overview 💡
This project aims to develop a machine-learning model to generate African Batik prints using StyleGAN. The primary goal is to produce unique Batik designs that artisans and designers can use. The project involves data collection, model development, validation, testing, and creating a user-friendly interface for generating new prints.

## Dataset 📊
We used a kaggle dataset containing images of African Batik prints. We preprocess the data by resizing images and normalizing pixel values. [Link to Kaggle dataset here](https://www.kaggle.com/datasets/mikuns/african-fabric)

## Data Preprocessing 📋
The data preprocessing involves:
- Resizing images to a consistent size for model input.
- Normalizing pixel values to the range [-1, 1].

## Feature Engineering 🔍
Feature engineering steps include:
- Extracting style and content features from the images.
- Using AdaIN (Adaptive Instance Normalization) to combine content and style features.

## Model Training 🧑🏻‍💻
The StyleGAN model is built using TensorFlow and Keras. We trained the model on the dataset, adjusting hyperparameters such as the number of layers, the number of neurons per layer, and the learning rate. We used techniques like regularization and dropout to prevent overfitting.

## Evaluation and Optimization 📈
Once the model was trained, we evaluated its performance using various metrics. We computed metrics such as Frechet Inception Distance (FID) to assess the quality of generated images. Optimization techniques, including parameter tuning and cross-validation, were employed to enhance model performance.

## Usage 💪🏻
To run the project locally, follow these steps:
1. Clone this repository:
    ```bash
    git clone [https://github.com/yourusername/Batiq.git](https://github.com/ladymargehagan/Group26_AfricanFabricStyleGAN-Batiq)
    ```
2. Navigate to the project directory:
    ```bash
    cd Batiq
    ```
3. Create a virtual environment:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
4. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```
5. Run the `app.py` script to start the Streamlit application and generate new Batik prints:
    ```bash
    streamlit run app.py
    ```

## Hosting 🌐

### Local Server
1. Ensure you have followed the installation steps.
2. Run the Streamlit application locally:
    ```bash
    streamlit run app.py
    ```
3. Access the application in your web browser:
    ```
    http://localhost:8501
    ```

## Results and Discussion 📊

#### Performance Metrics
- **Frechet Inception Distance (FID):** averagely 25

 **Generated Batik Prints**:
   - [Generated Batik Prints](image_2.png)
   - [Generated Batik Prints](image_1.png)
   - [Generated Batik Prints](image_3.png)
   - These figures show a selection of Batik prints generated by our StyleGAN model.


#### Model Details
- **Model Architecture:** The StyleGAN model consists of several layers with adaptive instance normalization (AdaIN). The optimizer used is Adam.
  
- **Hyperparameters:** 
latent dimensionality = 512
image size = 512
channels = 3
batch size = 8
epochs = 400

#### Evaluation
- **Training Performance:** The model was trained for 400 epochs to generate higher-quality images. The FID score reduced and did not fluctuate towards the end of the training process.
- **Example Outputs:** The model's generated prints were visually assessed to ensure quality and diversity.

#### Discussion
- **Strengths:** The StyleGAN model effectively captured the intricate patterns and designs of Batik prints, making it suitable for generative art applications. The model achieved a low FID score, indicating high-quality outputs.
- **Limitations:** The images generated were not as high quality as anticipated due to the computational limitations of colab. 
- **Areas for Improvement:** Future work could explore alternative model architectures, such as using pre-trained models, increasing the number of layers, and using more images for training.


## YouTube Video 📹
A demonstration video showing how the application works is available on YouTube. You can watch it [here](https://youtu.be/PXudPfDK-II).
---

