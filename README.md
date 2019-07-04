# Deploy Sneaker Classify [fast.ai](https://www.fast.ai) model with [Render](https://render.com) as Web App 


This repo is used to deploy a [fast.ai](https://github.com/fastai/fastai) model on Render.

The app described here is up at https://sneaker-collection.onrender.com/. Test it with your sneaker images.

You can test your changes locally by installing Docker and using the following command:

```
docker build -t fastai-v3 . && docker run --rm -it -p 5000:5000 fastai-v3
```
