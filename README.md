# CLA - WiFi Auth Failure | Approach -1 (Just a vecotr module) :

### Code file signficance:
 1. text_vectorization.py - Training Vectorizer Model for each node i.e. RC/class/family
 2. inference_engine.py - Distance calculations and Inference engine 
 3. inference_API.py - REST Api service using Flask framework
 4. requirements.txt - Contains all the required python libs/pkgs.
 
### Directory/Folder significance:
 1. data - Contains data to be trained using vector model(CountVectorizor)
 2. error_logs - 
 3. new_symptoms - whenever new syslog/error message hits trained model and if model has less confidence, then such messages are recorded separately for model improvements. Extra attention required for such messages.
 4. text_vectors - Pickle model for each node i.e. RC/class/family

![Alt text](SS/Screen%20Shot%202020-09-29%20at%203.13.15%20PM%20(2).png?raw=true "Title")
