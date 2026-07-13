As part of a course on Machine Learning I am undertaking there is a requirement to undertake a black box optimization (BBO) project. This is a task where you are attempting to optimise a function which cannot be directly observed, it can only be interrogated once per week. An initial limited set of data points are provided. In actual fact there are several functions to optimise, each has a different number of dimensions or features, from 2 to 8.

BBO is most relevant to solving problems where it is slow or expensive to evaluate the function being optimised, this could be because it requires an expensive simulation, drug trials or a significant length of time to get results (e.g. the financial impact of making a given set of changes to a business).

This project will help me in my career to understand how to optimise a complex problem where it is expensive to undertake trials.

Inputs and Outputs:

The model initially receives a set of input and output parameters, there are 8 functions in total to optimise ranging from 2 to 8 dimensions. The lowest dimensional problems have just 10 initial data points and the highest dimension has about 30. The input values are all constrained to be between 0 and 1, the output values are not constrained. Each week a new sample point can be selected for each function and evaluated by the black box function. The output is a scalar representing the output of the function that I'm trying to optimise at the given sample point. This new value can then be added to the data for the following week.

Challenge Objectives:

MY personal objective is to gain knowledge and work with tools that can be used to optimise black box optimisation problems. The main technical objective is to maximise each of the unknown functions constrained within the input region of 0-1 for each dimension. I will only be allowed to submit ten samples across the project and each will take a week to be analysed.

Technical Approach:

During the first three weeks I have been using a Gaussian Process model to represent knowledge of each function. I have been using the Upper Confidence Bound to select where to sample the function input space to gain knowledge on each of the hidden functions. I also use a number of metrics to give me a feel for whether I am exploring or being exploitive of the existing data. Some functions feel quite multimodal so these I am keen to explore, whereas others seem more singular, so I am more exploitive.
