# moveit_pro_sam3

ROS package containing SAM 3 ONNX models for image segmentation.

## Usage

Submodule this repository into a user workspace to make the models available in the `moveit_pro_sam3` package for use by MoveIt Pro Behaviors.

## Model license and use restrictions

The ONNX model files in [`models/`](models/) are exports of Meta's SAM 3 model and are distributed under the [SAM License](LICENSE). By using or redistributing these models, you agree to that license.

The SAM License includes restrictions that downstream users must follow. In particular:

- Do not use the SAM Materials for military or warfare purposes, activities subject to the International Traffic in Arms Regulations (ITAR), nuclear industries or applications, espionage, or the development or use of guns or illegal weapons.
- Comply with applicable trade controls, privacy laws, and data-protection laws.
- Redistribute the models and derivative works only under the SAM License and include a copy of the license.
- Acknowledge the use of the SAM Materials when publishing research results produced with them.

This summary is provided for convenience and does not replace the full [SAM License](LICENSE).

## Provenance

The files in `models/` are the `*-q4f16.onnx` assets from [jamjamjon/assets, release `sam3`](https://github.com/jamjamjon/assets/releases/tag/sam3), renamed as listed below. They are third-party ONNX exports of Meta's SAM 3 model with q4f16 weight quantization (4-bit weights, float16 activations), produced for the [usls](https://github.com/jamjamjon/usls) project. PickNik performed no training, fine-tuning, or other modification.

| File | Upstream asset | SHA-256 |
| --- | --- | --- |
| `sam3_decoder.onnx` | `decoder-q4f16.onnx` | `8496d685a950604626c3e6b972c21f5b4b876b15ce98b9b899875f392947b83c` |
| `sam3_geometry_encoder.onnx` | `geometry-encoder-q4f16.onnx` | `6717167a4454e063ab71895b5c03d067ce7386437fb489d1484feb2ca3abf741` |
| `sam3_text_encoder.onnx` | `text-encoder-q4f16.onnx` | `639ba5a9991b012d3290fbba27eb8dbcebdc86ed9f747572d7bea1678317d8d1` |
| `sam3_vision_encoder.onnx` | `vision-encoder-q4f16.onnx` | `9c00c5db8739f4c0cd0158a916f0e9755e0240bb35abca2934ab308e72cb2d6e` |

## Package licensing

The ONNX model files in `models/`, and derivative works of those models, are governed by the [SAM License](LICENSE). All other files in this repository are governed by the [BSD 3-Clause License](LICENSE.build), unless a file states otherwise.
