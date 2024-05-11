# age-detection
Source: https://pyimagesearch.com/2020/04/13/opencv-age-detection-with-deep-learning/
This code uses given dataset and deep learning to train the machine into detecting one's age. 

<ins>Customized Code</ins>
```python
def setArgs(image_name):
  args = {
    "image": image_name,
    "face": "face_detector",
    "age": "age_detector",
    "confidence": 0.5
}

  return args

def upload_files():
  from google.colab import files
  uploaded = files.upload()
  for k, v in uploaded.items():
    open(k, 'wb').write(v)
  return list(uploaded.keys())
```
Upload_files uploads image files that are age detected.
![Screenshot 2024-05-11 at 12 27 08 PM](https://github.com/olqvesk/age-detection/assets/125726282/f89a8330-bc37-413e-b1d2-36391582e3dc)

<ins>Result</ins>  
![download (1)](https://github.com/olqvesk/age-detection/assets/125726282/b5444a71-f490-43b8-983c-ccaaf44efd29)
