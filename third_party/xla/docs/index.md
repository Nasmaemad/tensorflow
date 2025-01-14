# XLA

XLA (Accelerated Linear Algebra) is an open-source compiler for machine
learning. The XLA compiler takes models from popular frameworks such as PyTorch,
TensorFlow, and JAX, and optimizes the models for high-performance execution
across different hardware platforms including GPUs, CPUs, and ML accelerators.
For example, in a
[BERT MLPerf submission](https://blog.tensorflow.org/2020/07/tensorflow-2-mlperf-submissions.html),
using XLA with 8 Volta V100 GPUs achieved a ~7x performance improvement and ~5x
batch-size improvement compared to the same GPUs without XLA.

As a part of the OpenXLA project, XLA is built collaboratively by
industry-leading ML hardware and software companies, including
Alibaba, Amazon Web Services, AMD, Apple, Arm, Google, Intel, Meta, and NVIDIA.

## Key benefits

-   **Build anywhere**: XLA is already integrated into leading ML frameworks
    such as TensorFlow, PyTorch, and JAX.

-   **Run anywhere**: It supports various backends including GPUs, CPUs, and ML
    accelerators, and includes a pluggable infrastructure to add support for
    more.

-   **Maximize and scale performance**: It optimizes a model's performance with
    production-tested optimization passes and automated partitioning for model
    parallelism.

-   **Eliminate complexity**: It leverages the power of
    [MLIR](https://mlir.llvm.org/) to bring the best capabilities into a single
    compiler toolchain, so you don't have to manage a range of domain-specific
    compilers.

-   **Future ready**: As an open source project, built through a collaboration
    of leading ML hardware and software vendors, XLA is designed to operate at
    the cutting-edge of the ML industry.

## Documentation

To learn more about XLA, check out the guides below. If you're a new XLA
developer, you might want to start with [XLA architecture](architecture.md) and
then read [Code reviews](code_reviews.md).

-   [Aliasing in XLA](aliasing.md)
-   [XLA architecture](architecture.md)
-   [Broadcasting](broadcasting.md)
-   [Code reviews](code_reviews.md)
-   [XLA custom calls](custom_call.md)
-   [Developing a new backend for XLA](developing_new_backend.md)
-   [Operation semantics](operation_semantics.md)
-   [Shapes and layout](shapes.md)
-   [Tiled layout](tiled_layout.md)
-   [Setting up LSP with clangd](lsp.md)
