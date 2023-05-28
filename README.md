# fake-images
Detecting AI-generated images using PyTorch's ConvNet 

* Note - The entire dataset was not uploaded to GitHub due to size constraints. The dataset is located here: https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images

To load the model from the .pt file; 

```
model = torch.jit.load('model.pt')
model.eval() 
```

The first implementation (pushed on May 28th) records:
- A training loss of ~0.117468 after 5 epochs
- An average testing loss of ~0.1572
- An accuracy of ~ 94%

What can be done to improve this is: 
- Utilizing the validation dataset to modify hyperparameters
- Find more sources of training data
- Run for more epochs
- Improving architecture
