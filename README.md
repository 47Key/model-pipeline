# Model Pipeline - Docker, Tensorflow, Flask
* Include the tokenizer & model config files in /app, model should use the folder name "BILSTM", and tokenizer as "tokenizer.json"
* Make sure the model directory structure is standard, and doesn't use the version structure as per "Tensorflow/Serving" requires.
* Start in the current directory, run docker build -t model-pipeline .
* Once the image is built, run the command docker run -p 5000:5000 -t model-pipeline
* Begin making requests the endpoint using the /predict endpoint, and a data argument in the raw JSON.

* Query the endpoint (Body Raw JSON):
{"data": ["Full Stack Developer", "Radiology Technologist", "Store Sales Associate"]}
