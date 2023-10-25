# H_point-Torso_angle-calculation-using-deep-learning
Computer vision algorithms to predict H-point and torso angle

Read H_point.txt to get a brief understanding about H-point and torso angle

A deep learning approach is presented where the CAD model of the seat is directly converted into a point
cloud format, which is fed into a neural network architecture. Material data is also fed into the network at
a later stage to finally predict the H-point coordinates and torso angle. The target values obtained from the
simulations performed over previous years are used to determine the H-point coordinates.

Various deep learning architectures are implemented specially Pointnet, Pointnet++, DGCNN, and
GAPnet where the layers are modified for this project and a regression layer added in the end. Motivation
from other architectures are also taken such as human pose estimation or combining the layers of the
previously mentioned architectures to take advantage of the specialties of each architecture.

An analysis is performed for all the architectures with an aim to minimize the difference between the
predicted coordinates and the target coordinates with an aim to reduce this difference below fifteen
millimeters. To obtain this various hyper-parameters in the neural network model are changed and the
performance analyzed.

Finally, this whole process is automated with the only input from the user being the finite element cad file
of the seat and the model outputs the H-point coordinates and torso angle. This approach reduces the total
time by a great margin where it was taking more than fifteen hours reduced to a couple of minutes.
