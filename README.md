# Assignment-3
- This repository contains the source code of the 3 part assignment.
- Architecture, Tradeoffs have been provided in the README files for individual parts

# Summary:
- The solution is designed to be:
  - Deterministic: Predictable, rule based behavior
  - Testable: Isolated validation with standard tools
  - Portable: This solution runs anywhere with Python installed
  - Extensible: Ready to plug into larger systems
  - Evaluation simplicity - No environment setup required. Just install numpy and pytest

- The focus is correctness, maintainability and production-aligned structure rather than framework complexity.
- Tradeoffs:

| Decision              	| Trade-off                      	| Reason                                  	|   	|   	|
|-----------------------	|--------------------------------	|-----------------------------------------	|---	|---	|
| No external libraries 	| Less automation vs portability 	| Ensures zero setup and reproducibility  	|   	|   	|
| Strict validation     	| Less forgiving input           	| Prevents ambiguous interpretation       	|   	|   	|
| Class-based design    	| Slightly more structure        	| Enables scalability and maintainability 	|   	|   	|


- Assumptions:
  - Inputs follow a predictable and semi-structured format
  - Guardrails definitions are explicit (no inference required)
  - Deterministic validation is preferred over heuristic interpretation

- Validation: How to trust the solution works:
  The implementation is validated using Python's inbuilt ```unittest``` framework.
  What is tested?
  - Correct parsing of valid guardrails.
  - Proper error handling for invalid inputs
  - Structureal validation of required fields
  - Stability across edge cases.
 

- AI assistant used for assistance - Github Copilot and ChatGPT.
