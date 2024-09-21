
# Using GPT as a computational annotator

This guide explain the process of employing GPT as a computational annotator within a PhiTag.

## Note
This project makes use of the [DWUG EN](https://zenodo.org/records/7387261) dataset. For word usages, we only provide the dataId of the original usages. To obtain the full data, please refer to the original dataset and match the usage identifiers with our dataIds.

## Step 1
Initiating GPT as an annotator begins with data preparation.

## Data Format

### Usage File

Please provide uses.tsv files in the general format outlined in the [Supported Tasks](/guide/guideline/supported-tasks.md) guide.

### Instance File
The instance file is a tab-separated file with the following columns:

**instanceID**: A unique ID for the instance.

**dataIDs**: A pair of dataIDs, corresponding to the dataID column in the uses.tsv file, for which the lemma is the same.

**label_set**: A scale, e.g. (1,2,3,4).

**non_label**: A non-label (-).

## Step 2: Project Creation
Follow this guideline [Explained: Project](/guide/guideline/explained-project.md) to create a project in PhiTag.


## Step 3: Phase Create
Follow this guideline [Explained: Phase](/guide/guideline/explained-phase.md) to create a project in PhiTag.

## Step 4: Add ChatGPT as a computaional annotator to your project

| ![](/guide/add-comp-annotator.gif) |
| :---------------------------------: |
|           Add GPT as a computational annotator          |


## Step 5: Annotate Phase
Here's a visual representation of how to utilize GPT as an annotator. You have the option to either use your own custom prompt or leverage the automatic prompting feature. The automatic prompting feature utilizes guideline and guideline + tutorial as prompts automatically.

| ![](/guide/annotate-phase-using-gpt.gif) |
| :---------------------------------:    |
|    Annotate Phase using GPT      |


## Test model with tutorial Phase
To evaluate the model's accuracy using the tutorial phase, you need to first create a tutorial phase. Follow the guidelines provided in
    [Explained: Create Tutorial Phase](/guide/guideline/explained-how-to-create-tutorial.md)


| ![](/guide/test-with-tutorial.gif)  |
| :-------------------------------------------: |
|    Test model with tutorial               |






