# Sequential API vs Functional API

## What is the difference?

- **Sequential API**: Sequential API is a simple, linear stack of layers where each layer has exactly one input tensor and one output tensor.
- **Functional API**: Functional API allows for more complex model architectures, including models with multiple inputs, multiple outputs, shared layers, and branching.

## Why use one over the other?

- **Sequential API**: Suitable for simple models where the data flows sequentially through each layer.
- **Functional API**: Provides more flexibility and customization options for building complex models with non-linear data flows and shared layers.

## When to use each API?

- **Sequential API**: Preferable for straightforward, single-input, single-output models such as simple feedforward neural networks or convolutional neural networks (CNNs).
- **Functional API**: Ideal for more advanced architectures like multi-input/multi-output models, models with skip connections, or models with shared layers.

## Where can each API be applied?

- **Sequential API**: Commonly used in scenarios where the model architecture is straightforward and follows a sequential flow of data.
- **Functional API**: Useful in more diverse and complex scenarios where the model architecture requires non-linear connections, branching, or sharing of layers.

## Who benefits from using each API?

- **Sequential API**: Beginners or users who need to quickly build simple neural networks with minimal complexity.
- **Functional API**: Advanced users or researchers who require more control and customization over their model architectures.

## How do they differ in terms of implementation?

- **Sequential API**: Models are created by adding layers sequentially using the `Sequential` class constructor.
- **Functional API**: Models are created by defining input tensors, connecting layers using functional composition, and then defining the model using the `Model` class constructor.