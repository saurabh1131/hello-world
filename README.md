# CLA - WiFi Auth Failure | Approach -1 (Just the Vector module) :

### Code file signficance:
 1. text_vectorization.py - Training Vectorizer Model for each node i.e. RC/class/family
 2. inference_engine.py - Distance calculations and Inference engine 
 3. inference_API.py - REST Api service using Flask framework
 4. requirements.txt - Contains all the required python libs/pkgs.
 
### Directory/Folder significance:
 1. data - Contains data to be trained using the vector model(CountVectorizor)
 2. error_logs - If an unhandled error encountered, such error will be captured and respective symptoms will be reported along with the error dump.
 3. new_symptoms - Whenever a new Syslog/error message hits the trained vector models and if the model has less confidence, then such messages are recorded separately for model improvements. Extra attention required for such symptoms.
 4. text_vectors - Saved model as a pickle for each node i.e. RC/class/family
 
### Module driver instruction:

1. Install all the needed dependencies using the requirements.txt file
2. Command to be executed for inference/predictions -> "python inference_API.py"
3. As defined, the app would run on the 8080 localhost port. Use curl or postman as follows:

![Alt text](SS/Screen%20Shot%202020-09-29%20at%203.13.15%20PM%20(2).png?raw=true "Title")
