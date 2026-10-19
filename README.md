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

- 🔴 **Red / Yellow / White** = High importance
  - The model paid a lot of attention to these areas.
  - Changes in these pixels would strongly affect the prediction.

- 🟢 **Green / Light Blue** = Medium importance
  - These regions contributed somewhat to the model's decision.

- 🔵 **Dark Blue / Black** = Low importance
  - These areas had little or no influence on the prediction.

#### Example: Brain Tumour Detection

If an AI predicts **"Tumour"**:

✅ A good saliency map will highlight the tumour region.

❌ A concerning saliency map might highlight areas outside the brain, suggesting the model is focusing on irrelevant information.

#### Important Limitation

A saliency map shows **where the model is looking**, but not **why**.

It tells us:

> "These pixels were important."

It does **not** tell us:

> "These pixels support the tumour prediction."


---
## What was Built:

We built a Convolutional Neural Network to ...


<img src="https://raw.githubusercontent.com/KeithQuille-TUDublin/ethicon26Health/refs/heads/main/Training%20performance.png">


---

## Your Challenge

You will investigate two sets of AI predictions:

### PredictionTumor

The AI predicted that a tumour is present.

### PredictionNotTumor

The AI predicted that a tumour is not present.

For each case:

1. Examine the MRI scan.
2. Examine the saliency map.
3. Decide whether the AI appears to be reasoning sensibly.
4. Decide whether you would trust the prediction.

Do not worry about being medically correct.

Focus on whether the AI appears trustworthy.

---

## Questions

For every case discuss:

### 1. Would you trust this prediction?

Rate from:

- 1 = Do Not Trust
- 2 = Mostly Do Not Trust
- 3 = Unsure
- 4 = Mostly Trust
- 5 = Completely Trust

### 2. Why?

What evidence supports your decision?

### 3. What concerns do you have?

Does the AI appear to focus on sensible areas of the scan?

### 4. What additional information would help?

What would you want to know before using this system in a hospital?

