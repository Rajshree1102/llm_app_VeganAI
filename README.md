# Overview
The Vegan Food Dataset RAG Project is designed to combine retrieval-augmented generation (RAG) techniques with a curated dataset of vegan foods, ingredients, and recipes. This project aims to deliver relevant information and generate meaningful insights on vegan diets through retrieval of data and natural language generation. It can be used to answer query related to vegan recipes.

# Features 
1) Recipe Retrieval: Retrieve vegan recipes from a dataset based on user inputs (e.g., dish name, ingredients).
2) Ingredient Information: Provide detailed information about vegan ingredients.
3) Recipe Generation: Automatically generate new vegan recipes using ingredients provided by the user.
4) Query-based Interaction: Supports natural language querying for quick and relevant responses on vegan food topics.

# Dataset
The project utilizes a curated Vegan Food Dataset, which includes:
1) A wide range of vegan recipes.
2) Nutritional data for ingredients and dishes.
3) Steps for making dishes.
4) Detailed information about ingredients to make recipes.

# Demo Video Link
https://drive.google.com/file/d/1jQC4O-wTrkX1NYAWHw_leMstsgHhAeJ5/view?usp=sharing

# Demo Usage
Here's the link to the demo use of this application.
# Installation
To set-up HogwartsBot, follow the steps below:

- Clone the repository in your **VSCode terminal**:

    `git clone https://github.com/Rajshree1102/llm_app_VeganAI`

   - Go into this Directory:
     'cd llm_app_VeganAI'

- Run the application using **Docker**:

    `docker build -t veganai .`\
    `docker run -p 8000:8000 veganai`
    
    Running the docker container may take upto 3-4 minutes.
- Use either Postman or ThunderClient API service to give prompt requests:
 
    URL : `http://localhost:8000/v1/pw_ai_answer`
    
    - Here's how to do it in **Thunder Client**:

        - Set the **HTTP** method to **POST**.
        - Go to the **Headers** tab.
        - Add a header with:

                Key: Content-Type
                Value: application/json
        Setting the Content-Type as `application/json` is necessary for most APIs to correctly parse and understand the JSON data you send in the request body.

        - **Body**: Click on the Body tab, select JSON format, and enter the following JSON:

                {
                    "prompt": "Enter your prompt"
                }



# License
This project is licensed under the MIT License. See the **LICENSE** file for more details.




