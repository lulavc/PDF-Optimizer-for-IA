# PDF Compression for AI

A sophisticated system for optimizing PDFs for AI models, with advanced token optimization, multi-objective compression techniques, and detailed statistics tracking.

## Features

- **Advanced Token Optimization**: Minimize token usage for specific AI models (GPT, Claude, LLaMA) using information theory and dynamic programming
- **Multi-Objective Compression**: Balance size reduction, semantic preservation, and token efficiency
- **Coordinated Technique Application**: Intelligently apply compression techniques based on document characteristics
- **Comprehensive Statistics Tracking**: Monitor and analyze compression performance with detailed metrics
- **Modern GUI**: User-friendly interface with visualization and interactive controls

## Architecture

The system is built with a modular architecture:

- **Core Components**:
  - `TokenOptimizer`: Advanced token optimization for specific models
  - `CompressionCoordinator`: Coordinates application of compression techniques
  - `MetadataTracker`: Tracks and analyzes compression statistics

- **UI Components**:
  - `AdvancedCompressionGUI`: Main GUI with tabbed interface
  - Interactive visualizations and controls

## Mathematical Foundation

The system implements sophisticated mathematical models:

1. **Token Optimization**: Formalized as entropy minimization problem
   ```
   min H(T|S) = -∑ p(s) ∑ p(t|s) log p(t|s)
   ```

2. **Multi-Objective Optimization**: Vector optimization problem
   ```
   min F(D,α,β,γ,δ) = [f_size(D,α,β,γ,δ), f_semantic(D,α,β,γ,δ), f_token(D,α,β,γ,δ)]
   ```

3. **Technique Interactions**: Modeled as weighted graph with synergy/conflict edges

## License

This project is licensed under the MIT License - see the LICENSE file for details.
