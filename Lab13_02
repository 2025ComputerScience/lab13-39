import pytesseract
from PIL import Image
import cv2
import numpy as np
from google.colab import files 

#1:上傳圖片
print("請上傳圖片 (建議：白紙黑字，字寫粗一點)")
uploaded = files.upload()

for fn in uploaded.keys():
    image = Image.open(fn)

    #2:OCR辨識
    #lang='eng':辨識英文
    #psm6:適合辨識一個整齊的文字區塊
    text = pytesseract.image_to_string(image, lang='eng+chi_tra', config='--psm 11')

    #3:顯示結果
    print("OCR 辨識結果:")
    print("-" * 40)
    print(text)
