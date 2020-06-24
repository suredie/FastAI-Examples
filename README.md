# FastAI-Examples
Deep learning examples and paper reproduction with Fast AI library.

- HelloWorld

    - Hello_World_with_FastAI.ipynb: A basic classification example with MNIST sample dataset. Use Fast AI only, without any customization.
    - Use_Pretrained_Models.ipynb: Use pretrained model provided by `Cadene` or `pytorchcv`.
    - Use_Customized_Model.ipynb: Train self-defined model.
    - Save_Features.ipynb: Extract the activations of a module in the model as the features; Visualize the features after dimension reduction using TSNE.

- TransferLearning

    - Domain_Adaptation_Gradient_Reversal.ipynb: Reimplement algorithm in paper [Unsupervised Domain Adaptation by Backpropagation](https://arxiv.org/abs/1409.7495), without consideration for weighting between classification loss and domain discrimination loss.
    
        - Organize data into a csv file to comply with data interfaces of `Fast AI`.
        - Customize the classification headers.
        - Customize loss function.

### ToDo
- HelloWorld

    - When use `SaveModelCallback`, how to prevent the Learner from automatically loading the best model?

- Transfer Learning

    - Domain_Adaptation_Gradient_Reversal.ipynb: Change `__name__` of functions created using `partial`.
    - Domain_Adaptation_Gradient_Reversal.ipynb: Create a scheduler to account for weighting between classification loss and domain discrimination loss.

