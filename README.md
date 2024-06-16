HARVESTIFY 🌿
FARMGENIUS: A MACHINE  LEARNING-BASED APPROACH  FOR SUSTAINABLE  AGRICULTURE
DISCLAIMER ⚠️
This is a proof-of-concept project. The data used here comes with no guarantees from the creator. Do not use it for making farming decisions; the creator is not responsible for any consequences. However, this project showcases the potential of using ML/DL in precision farming if developed on a larger scale with authentic and verified data.

MOTIVATION 💪
Agriculture is a major sector that impacts a country’s economic growth.

In a country like India, a significant portion of the population depends on agriculture for their livelihood. Many new technologies, such as Machine Learning and Deep Learning, are being applied to agriculture to assist farmers in optimizing their yield.

This project presents a website with the following applications: Crop recommendation, Fertilizer recommendation, and Plant disease prediction.

In the crop recommendation application, users can provide their soil data, and the application will predict the best crop to grow.

For the fertilizer recommendation application, users can input their soil data and the type of crop they are growing. The application will predict nutrient deficiencies or excesses and recommend improvements.

In the plant disease prediction application, users can upload an image of a diseased plant leaf. The application will identify the disease and provide background information and suggestions for treatment.
HOW TO USE 💻
Crop Recommendation system: Enter the corresponding nutrient values of your soil, state, and city. Note that the N-P-K (Nitrogen-Phosphorus-Potassium) values should be the ratio between them. Refer to this website for more information.
Note: When you enter the city name, make sure to enter mostly common city names. Remote cities/towns may not be available in the Weather API from where humidity and temperature data is fetched.

Fertilizer suggestion system: Enter the nutrient contents of your soil and the crop you want to grow. The algorithm will identify nutrient deficiencies or excesses and recommend suitable fertilizers.

Disease Detection System: Upload an image of a leaf from your plant. The algorithm will identify the crop type and whether it is diseased or healthy. If diseased, it will provide information about the disease and suggestions for treatment.
Note that, for now, it only supports the following crops:

<details>
  <summary>Supported crops
</summary>
Apple
Blueberry
Cherry
Corn
Grape
Pepper
Orange
Peach
Potato
Soybean
Strawberry
Tomato
Squash
Raspberry
</details>
HOW TO RUN LOCALLY 🛠️
Ensure you have git, Anaconda or miniconda installed on your system.
Clone the project with git clone https://github.com/Gladiator07/Harvestify.git or download and unzip the code.
Note: The master branch doesn't contain the updated code used for deployment. To download the updated code used for deployment, use the following command:
bash
Copy code
❯ git clone -b deploy https://github.com/Gladiator07/Harvestify.git 
The deploy branch contains only the code required for deploying the app (the rest of the code used for training the models and data preparation can be accessed on the master branch).
It is recommended to clone the deploy branch for running the project locally. The following steps apply only if you have cloned the deploy branch.
Once the project is cloned, open the Anaconda prompt in the project directory and execute:
lua
Copy code
conda create -n harvestify python=3.6.12
conda activate harvestify
pip install -r requirements.txt
Finally, run the project with:
Copy code
python app.py
Open the localhost URL provided after running app.py to use the project locally in your web browser.
