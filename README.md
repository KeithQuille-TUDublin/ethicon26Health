<img src="https://thumb.wikimedia.org/wikipedia/commons/thumb/0/06/TU_Dublin_Logo.svg/330px-TU_Dublin_Logo.svg.png?utm_source=commons.wikimedia.org&utm_campaign=index&utm_content=thumbnail&_=20200525121240">


# Ethicon: Can We Trust Medical AI?

## Welcome

In this Ethicon, you will act as an AI ethics review panel for a hospital considering the use of an Artificial Intelligence (AI) system to assist with brain tumour diagnosis.

The AI has analysed a number of MRI scans and has made predictions about whether a tumour is present.

Alongside each prediction, the AI also provides a **saliency map** showing the parts of the image that influenced its decision.

Your task is not to decide whether the AI is correct and trustworthy.

Your task is to decide:

> Should the AI be trusted?

---

## What is a Saliency Map?

A saliency map is a visual explanation of where the AI focused its attention when making a prediction.

The highlighted areas show which parts of the MRI image were most influential in the AI's decision.

Think of a saliency map as the AI answering:

> "These are the areas I considered important."

<br>
Below is an example of a saliency map (often called an AI heatmap):
<br>

<img src="https://debuggercafe.com/wp-content/uploads/2021/05/cam_exmp_2.jpg" width="800px">

### What Do the Colours in a Saliency Map Mean?

A **saliency map** highlights the parts of an image that were most important to an AI model when making a prediction.

#### Colour Interpretation

- **Red / Yellow / White** = High importance
  - The model paid a lot of attention to these areas.
  - Changes in these pixels would strongly affect the prediction.

- **Green / Light Blue** = Medium importance
  - These regions contributed somewhat to the model's decision.

- **Dark Blue / Black** = Low importance
  - These areas had little or no influence on the prediction.


#### Important Limitation

A saliency map shows **where the model is looking**, but not **why**.

It tells us:

> "These pixels were important."

It does **not** tell us:

> "These pixels support the tumour prediction."


---
## What was Built:

We built a Convolutional Neural Network to identify Brain Tumours, via MRI scans. The model reported an accuracy of 85% during training, on never before seen scans, seems amazing, the below is the training plots for the model: 


<img src="https://raw.githubusercontent.com/KeithQuille-TUDublin/ethicon26Health/refs/heads/main/Training%20performance.png">

---

## Your Challenge

You will investigate two sets of AI predictions based on your hospital MRI scans (to see if the AI is trustworthy for use):

### PredictionTumor

The AI predicted that a tumour is present.

Located in folder: [PredictionTumor folder](https://github.com/KeithQuille-TUDublin/ethicon26Health/tree/d052ff31c95a7e952c54847d869d08ab5326416c/PredictionTumor)

### PredictionNotTumor

The AI predicted that a tumour is not present.

Located in folder: [PredictionNotTumor folder](https://github.com/KeithQuille-TUDublin/ethicon26Health/tree/d052ff31c95a7e952c54847d869d08ab5326416c/PredictionNotTumor) 



## Challenge:
### For each Saliency map and prediction:

1. Examine the MRI scan.
2. Examine the saliency map.
3. Decide whether the AI appears to be reasoning sensibly.
4. Decide whether you would trust the prediction (simple yes no)

### For the overall model:
1. For the overall model, have a small statement (max 200 words) on what you think of it, both from a view point on accuracy and the saliency maps!

### Hints:
Do not worry about being medically correct.

Focus on whether the AI appears trustworthy.

There are 60 images, arranged in folders based on the AI prediction **NOT** the actual diagnosis, so you are unsure if the prediction was correct or not! Each image has a random ID 1-60 to help you when you are sorting your answers! Best of luck!



