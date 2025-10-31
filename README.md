It looks like the download link didn’t load properly on your end — that can sometimes happen in temporary sessions.

Let’s fix it:
You can recreate the README manually by copying this Markdown content into a new file named **`README.md`** on your computer:

---

```markdown
# 🦐 Shrimp Larvae Detection with YOLO

This project demonstrates how to **export a trained YOLO model** for shrimp larvae detection. It uses the [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) framework to handle model loading and exporting to different formats.

---

## 📁 Project Overview

The purpose of this script is to **export a trained YOLO model** (in this case, `YOLOshrimp.pt`) into a different format for deployment or optimization.  
The dataset used is defined in the `data.yaml` file located at:

```

Shrimp-larvae-detection-1/data.yaml

````

---

## 🧠 Requirements

Make sure you have Python 3.8+ installed and install the following dependencies:

```bash
pip install ultralytics
````

---

## 💻 Code Explanation

```python
from ultralytics import YOLO

# Load the custom-trained YOLO model
model = YOLO('YOLOshrimp.pt')

# Export the model to the specified format using the dataset configuration
model.export(format='imx', data="Shrimp-larvae-detection-1/data.yaml")
```

### 🔍 What Each Line Does:

* `from ultralytics import YOLO`
  Imports the YOLO class from the Ultralytics library.

* `model = YOLO('YOLOshrimp.pt')`
  Loads your pre-trained YOLO model (in this case, trained on shrimp larvae images).

* `model.export(format='imx', data="Shrimp-larvae-detection-1/data.yaml")`
  Exports the model to the **IMX** format using the provided dataset configuration file.

---

## ⚙️ Supported Export Formats

YOLO supports exporting to multiple formats (besides `'imx'`), including:

* `'onnx'` – For cross-platform inference
* `'torchscript'` – For PyTorch-based deployment
* `'engine'` – For NVIDIA TensorRT
* `'coreml'` – For iOS/macOS apps
* `'tflite'` – For TensorFlow Lite mobile devices

You can specify any of these formats by changing the `format` argument.

---

## 📦 Output

After running the script, the exported model will be saved in a directory such as:

```
runs/export/
```

You can use this exported file for **deployment**, **edge inference**, or **integration with other systems**.

---

## 🧾 License

This project uses the [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) framework.
Please follow its license terms when redistributing or modifying.

---

## 🙌 Acknowledgements

* [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) for the detection framework
* Dataset and model training for shrimp larvae detection (user-provided)

```

---

If you’d like, I can regenerate the actual file again so you can download it directly — would you like me to do that?
```
