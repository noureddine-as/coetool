# coetool
coetool is a cli or gui program to convert from .coe files (memory map for a ROM in an FPGA) to image files and the other way around, load an image and generate .coe file. Original author: http://jqm.io/files/coetool/

# What I did:
changed some places to fit my requirements：convert an image to .coe file in RGB888, not the original RGB332.

# denpendencies: 
python3 + PyQt5 + PIL

# Added features
This version is based on `https://github.com/shushm/coetool`. It adds support for exporting Coe format files intended to BRAM initialization. The outputs have been tested with Vivado 2018.1.

This version also supports exporting the images as C arrays of uint8_t or uin64_t (8 Bytes packed) elements.

# How to use

- 1: launch the tool (GUI mode)
    ```bash
    python3 coetoolgui.py
    ```
- 2: load the image (supports all PIL-compatible formats: png, gif, jpeg, pgm, ...)

- 3: File > Save as the target format.

# Examples

The `example_inputs` contains example images from google.
The `example_outputs` contains example pre-generated files.

# License:
GPL
