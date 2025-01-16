# Mall Customer Segmentation with KMeans and DBSCAN

This project demonstrates the clustering of mall customers based on their spending habits and income using the `Mall_Customers.csv` dataset. The project applies Exploratory Data Analysis (EDA), implements KMeans and DBSCAN clustering techniques, and deploys a web app built with Streamlit using Docker and Render.

## Watch the Video 📺

[![YouTube Video](https://img.shields.io/badge/YouTube-Watch%20Video-red?logo=youtube&logoColor=white&style=for-the-badge)](https://youtu.be/8SftgRodXiU)

![output](https://github.com/user-attachments/assets/40d664ec-98e4-4b11-85da-3d0cbd27cc11)


## Files in the Repository

1. **Clustering.ipynb**: Jupyter Notebook containing EDA, KMeans, and DBSCAN clustering implementation.
2. **Dockerfile**: Used to containerize the Streamlit application.
3. **Mall_Customers.csv**: Dataset containing information about mall customers.
4. **app.py**: Streamlit web application script to visualize clustering results and interact with the data.
5. **k_means.pkl**: Saved KMeans clustering model.
6. **requirements.txt**: List of Python dependencies for the project.

## Features

- **Exploratory Data Analysis (EDA)**: Understanding the structure, distribution, and relationships in the data.
- **Clustering**: KMeans and DBSCAN applied to cluster customers based on two variables (Annual Income and Spending Score).
- **Interactive Web Application**: Visualizes clustering results and allows user interaction via a Streamlit app.
- **Containerization**: The application is containerized using Docker and deployed on Render for easy accessibility.

## Technologies Used

- Python: Data analysis, clustering, and web application
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `streamlit`
- Docker: Containerization
- Render: Cloud deployment platform

# Demo:

![Screenshot 2025-01-14 153736](https://github.com/user-attachments/assets/40472caf-d7a5-4331-8df8-531833c6e5d8)


## Getting Started

### Clone the Repository

```bash
git clone <repository_url>
cd <repository_name>
```

### Dataset

The `Mall_Customers.csv` file is used for clustering customers based on spending patterns. Ensure it is in the same directory as other files.

### Setup Python Environment

Install the required Python libraries by running:

```bash
pip install -r requirements.txt
```

### Running the Application Locally

1. Run the Streamlit app using the command:
   ```bash
   streamlit run app.py
   ```
2. Open the browser and go to `http://localhost:8501` to view the application.

### Build and Run the Docker Container Locally

1. Build the Docker image:
   ```bash
   docker build -t mall-segmentation-app .
   ```
2. Run the Docker container:
   ```bash
   docker run -p 8501:8501 mall-segmentation-app
   ```
3. Access the application at `http://localhost:8501`.

### Deployment on Render

1. Build the Docker image and push it to Docker Hub:

   ```bash
   docker login
   docker tag mall-segmentation-app <your-dockerhub-username>/mall-segmentation-app
   docker push <your-dockerhub-username>/mall-segmentation-app
   ```

2. Deploy to Render by providing the Docker Hub image link during the setup process in Render.

## Usage

- Visualize the data distribution and clustering results.
- Compare the performance of KMeans and DBSCAN for customer segmentation.

## Future Enhancements

- Extend the clustering analysis by including more features.
- Implement additional clustering algorithms for comparison.
- Improve UI/UX of the Streamlit application.


## Acknowledgments

- Dataset: Mall Customer Segmentation dataset from [Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).

## 🚀 Thanks

**If you found it useful, leave a ⭐ here!**

```bash
Author: DataScientist00
Data Scientist
Email: nikzmishra@gmail.com

```
