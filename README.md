We trained a MobileNetV2 teacher achieving 97.3% validation accuracy.
Using knowledge distillation, a lightweight student CNN was trained.
After full INT8 quantization, the model preserved accuracy (80.4%) while reducing size to ~13 KB, enabling real-time inference on ESP32-CAM.

| Model TFLite | Accuracy |
|-------|-----------|
| [FP32](https://github.com/Dilara0880/esp32-cam_cat-dog_classification/blob/main/models/student_v2_fp32.tflite) | 0.8011 |
| [INT8](https://github.com/Dilara0880/esp32-cam_cat-dog_classification/blob/main/models/student_v2_int8.tflite) | 0.8039 |
