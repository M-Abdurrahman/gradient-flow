# gradient-flow
 A useful method to plot gradient flow in PyTorch writen by RoshanRane
original source https://discuss.pytorch.org/t/check-gradient-flow-in-network/15063/7

Use the **plot_grad_flow** function to plot the gradient flow by plugging it after the loss.backward() during the training as follows:
'''
loss = self.criterion(outputs, labels)  
loss.backward()
plot_grad_flow(model.named_parameters())
'''
