## IBM Cloud Deployment Commands (Frontend)

### Deployment URL
- Frontend Microservice: https://frontend.21w1m1zgyigi.us-south.codeengine.appdomain.cloud

### Deploy Frontend Microservice
cd /home/project
git clone https://github.com/ibm-developer-skills-network/dealer_evaluation_frontend.git
cd dealer_evaluation_frontend
ibmcloud ce application create --name frontend --image us.icr.io/${SN_ICR_NAMESPACE}/frontend --registry-secret icr-secret --port 5001 --build-source .

