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

The files in `models/` were produced by converting an upstream Meta SAM 3 checkpoint to ONNX without training or fine-tuning by PickNik. The exact checkpoint revision and export commands were not recorded in this repository.

## Package licensing

The ONNX model files in `models/`, and derivative works of those models, are governed by the [SAM License](LICENSE). All other files in this repository are governed by the [BSD 3-Clause License](LICENSE.build), unless a file states otherwise.
