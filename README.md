# Advanced PDF Compression for AI (Work in progress)

A sophisticated system for optimizing PDFs for AI models, with advanced token optimization, multi-objective compression techniques, and detailed statistics tracking.

## Features

- **Advanced Token Optimization**: Minimize token usage for specific AI models (GPT, Claude, LLaMA) using information theory and dynamic programming
- **Multi-Objective Compression**: Balance size reduction, semantic preservation, and token efficiency
- **Coordinated Technique Application**: Intelligently apply compression techniques based on document characteristics
- **Comprehensive Statistics Tracking**: Monitor and analyze compression performance with detailed metrics
- **Modern GUI**: User-friendly interface with visualization and interactive controls

## Installation

## Usage

### Quick Start

The easiest way to get started is to use the interactive launcher:

```bash
./launch.py
```

This will:
1. Check if all dependencies are installed
2. Let you choose between GUI, CLI, or running tests
3. Guide you through the options for your selected mode

You can also use command-line options with the launcher:

```bash
# Launch the GUI
./launch.py --gui

# Launch the GUI with pre-loaded files
./launch.py --gui --files file1.pdf file2.pdf

# Launch the CLI with specific files and options
./launch.py --cli --files file1.pdf --format json --level aggressive

# Run tests
./launch.py --test --test-file test_integration.py
```

### Running the GUI

To launch the advanced GUI directly:

```bash
python run_advanced_gui.py
```

Command-line options:
- `--files FILE1 FILE2 ...`: Pre-load PDF files
- `--output-dir DIR`: Set initial output directory
- `--config FILE`: Load configuration from file
- `--debug`: Enable debug mode with additional logging

### Using the GUI

1. **File Selection Tab**:
   - Select PDF files to process
   - Choose output directory
   - Set basic options (format, optimization level)

2. **Advanced Techniques Tab**:
   - Enable/disable specific compression techniques
   - Configure technique parameters
   - Set optimization priorities
   - Visualize technique interactions

3. **Statistics Tab**:
   - View real-time compression metrics
   - Analyze historical performance
   - Export detailed reports

### Configuration Files

The system supports configuration files in both JSON and YAML formats. Example configuration files are provided:

- `example_config.json`: JSON configuration template
- `example_config.yaml`: YAML configuration template

These files demonstrate all available options and can be used as a starting point for your own configurations.

To use a configuration file:

```bash
# With the launcher
./launch.py --gui --config example_config.json

# Or directly with the GUI
python run_advanced_gui.py --config example_config.yaml
```

You can also load configuration files from within the GUI using the "Load Configuration" button.


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

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. 
