# SMILES Viewer Lite

A simple web application that allows users to visualize molecular structures from SMILES (Simplified Molecular Input Line Entry System) strings. 

This application provides an easy-to-use interface where users can input a SMILES string along with desired dimensions for the molecular image, and it generates a visual representation of the molecule.

Available here: https://shoval.github.io/smiles-viewer-lite/

## Features

- **URL Parameter Input**: Accepts a SMILES string as a URL parameter for quick access.
- **Interactive Form**: If no SMILES string is present in the URL, a form is provided for manual input.
- **Custom Dimensions**: Users can specify the width and height for the generated molecular image.
- **Embeddable**: The URLs of this application can be embedded in other web services, such as Notion.

## Usage

You can access the page without parameters, and a form will be presented where you can manually enter the SMILES string and image dimensions.

But preferably you should provide the SMILES string directly as a parameter in the URL like so:
`https://shoval.github.io/smiles-viewer-lite/?smiles=[SMILES-string]`

**⚠️ Note**: The SMILES string must be escaped for it to work. You can use the built-in form to generate the URL if you encounter any problems.

You may also provide image dimensions (in pixels) directly in the URL:
`https://shoval.github.io/smiles-viewer-lite/?smiles=[SMILES-string]&width=300&height=200`

## Examples

Below are three examples demonstrating how to use SMILES Viewer Lite:

1. **Aspirin**:  
   https://shoval.github.io/smiles-viewer-lite/?smiles=CC%28%3DO%29OC1%3DCC%3DCC%3DC1C%28%3DO%29O

2. **Caffeine** (with dimensions):  
   https://shoval.github.io/smiles-viewer-lite/?smiles=CN1C%3DNC2%3DC1C%28%3DO%29N%28C%28%3DO%29N2C%29C&width=300&height=200

3. **2-Butylcyclohexanol** (simple formula - no need for escaping):  
   https://shoval.github.io/smiles-viewer-lite/?smiles=CCCCC1CCCCC1O

## Credits and Acknowledgements

This project uses SmilesDrawer 2.0 for rendering the molecular structures from SMILES strings. SmilesDrawer is an open-source project developed and maintained by the [Reymond Research Group](https://gdb.unibe.ch/) at the University of Bern.

For more information about SmilesDrawer, visit their GitHub repository: [SmilesDrawer 2.0](https://github.com/reymond-group/smilesDrawer).

## License

This project is open-sourced under the [MIT License](https://opensource.org/licenses/MIT).
