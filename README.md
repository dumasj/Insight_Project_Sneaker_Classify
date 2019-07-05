# Deploy Sneaker Classify [fast.ai](https://www.fast.ai) model with [Render](https://render.com) as Web App 


This repo is used to deploy a [fast.ai](https://github.com/fastai/fastai) model on Render. The Sneaker Classifier app uploads a personal sneaker image and returns it’s dollar value in the sneaker resale market. The app described here is up at https://sneaker-collection.onrender.com/. Test it with your sneaker images.

The guide used for production deployment to Render for this repo is at https://course.fast.ai/deployment_render.html.


## Deploy

1. Create a new Web Service on Render. You will need to grant Render permission to access your GitHub repo in this step.

2. On the deployment screen, pick a name for your service and use Docker for the Environment. The URL will be created using this service name.

3. Click Save Web Service. Your service will begin building and should be live in a few minutes at the URL displayed in your Render dashboard. You can follow its progress in the deploy logs.

4. Keep the GitHub repo you create current. Render integrates with your repo and automatically builds and deploys changes every time you push a change.

## Testing

To run the app server locally (check the requirements.txt file for system requirements), run this command:

```
python app/server.py serve
```

If you have Docker installed, you can test your app locally by running the following command at the root of your repo:

```
docker build -t Insight_Project_Sneaker_Classify . && docker run --rm -it -p 5000:5000 Insight_Project_Sneaker_Classify

```

Go to http://localhost:5000/ to view the app.
