# Benchmark Prompts Repository

This repository contains prompts and evaluation materials used by Kombai for benchmarking frontend code generation from figma and text inputs.

## Repository Structure

```
benchmark-prompts/
├── eval-prompts/
│   ├── functional-eval/
│   │   ├── criterion-generation.txt
│   │   └── functionality-eval.txt
│   ├── guidelines-eval/
│   │   ├── criterion.txt
│   │   └── guidelines-eval.txt
│   └── visual-eval/
│       ├── criterion-generation.txt
│       └── visual-eval.txt
├── figma-prompts/
│   ├── figma-ids.csv
│   ├── figma-links.txt
│   └── figma-images/
│       └── [40+ design images]
└── text-prompts/
    └── [text prompt files]
```

## Folder Descriptions

### eval-prompts/
Contains prompts used for the three evaluation types: functional, visual, and guidelines evaluation.

#### functional-eval/
- **`criterion-generation.txt`**: Prompt to create functional criteria based on the image of the figma design
- **`functionality-eval.txt`**: Prompt to evaluate functionalities in the generated code

#### visual-eval/
- **`criterion-generation.txt`**: Prompt to generate visual evaluation criteria from figma images
- **`visual-eval.txt`**: Prompt to compare generated UI screenshots with reference images based on visual criteria

#### guidelines-eval/
- **`criterion.txt`**: Manually curated guidelines specific for frontend code and their explanations
- **`guidelines-eval.txt`**: Prompt to check if the generated code is following the established guidelines

### figma-prompts/
Contains Figma designs used to generate code. Only includes information for community designs; some proprietary Figma links have been omitted.

- **`figma-links.txt`**: Links to community designs used in the benchmark
- **`figma-ids.csv`**: CSV file containing file IDs and node IDs for Figma designs
- **`figma-images/`**: Directory containing 40+ images of all designs used for evaluation reference

### text-prompts/
Contains text prompts used to generate code.

- **Txt Files**: Individual text prompts for code generation tasks

## Usage

This repository serves as a comprehensive benchmark for evaluating frontend code generation capabilities across multiple dimensions:

1. **Functional Evaluation**: Tests whether generated code implements the required functionality
2. **Visual Evaluation**: Compares visual output against reference designs
3. **Guidelines Evaluation**: Ensures code follows frontend development best practices
