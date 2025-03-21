# Bannerutils

## Overview
The **Bannerutils** is a command-line tool that converts text into stylish ASCII art banners. It supports multiple font styles, text alignment, and width customization. The tool is inspired by TAAG and utilizes the **pyfiglet** library for rendering text.

## Features
- Convert text into ASCII banners using a variety of fonts.
- Supports different text alignments (left, center, right).
- Adjustable banner width for better formatting.
- Copy generated banners directly to the clipboard.
- List available fonts with descriptions.

## Requirements
This script requires **Python 3.x** and the following dependencies:
- `pyfiglet` (for ASCII text rendering)
- `pyperclip` (for clipboard functionality)
- `argparse` (for command-line argument parsing)

If not installed, the script will automatically attempt to install missing packages.

## Installation
You can install the tool via **pip** or **GitHub**.

### Install via pip:
```sh
pip install bannerutils
```

### Install from GitHub:
1. Clone this repository:
   ```sh
   git clone https://github.com/jfrzz/bannerutils.git
   ```
2. Navigate to the directory:
   ```sh
   cd bannerutils
   ```
3. Run the script:
   ```sh
   python bannerutils.py --help
   ```

## Usage
Basic command format:
```sh
python banner.py "Your Text Here" [-f FONT] [-w WIDTH] [-a ALIGN] [--fonthelp]
```

### Example Commands
1. Generate a simple ASCII banner:
   ```sh
   python banner.py "Hello, World!"
   ```
2. Use a specific font:
   ```sh
   python banner.py "Hello" -f slant
   ```
3. Adjust banner width:
   ```sh
   python banner.py "Wide Text" -w 100
   ```
4. Center-align text:
   ```sh
   python banner.py "Centered" -a center
   ```
5. List available fonts with descriptions:
   ```sh
   python banner.py --fonthelp
   ```

## Available Fonts
The tool supports various fonts, including:
- **slant**: Slanted letters for a stylish effect.
- **big**: Large and bold text.
- **bubble**: Rounded bubble-like letters.
- **digital**: Digital clock-style font.
- **gothic**: Fancy gothic-style text.
- **isometric**: Multiple 3D isometric variations.
- **starwars**: Inspired by Star Wars title fonts.
- And many more!

To see the full list, run:
```sh
python -m pyfiglet -l
```

## Clipboard Support
After generating the banner, the script prompts you to copy it to the clipboard. Simply enter `y` to copy or `n` to skip.

## License
This project is open-source and available under the MIT License.

## Author
Created by **[@JfrzxCode]**

---
