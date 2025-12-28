import pytesseract
from PIL import Image
import cv2

uploaded = files.upload()

# 開啟圖片
for fn in uploaded.keys():
    image = Image.open(fn)

# OCR 辨識英文
text = pytesseract.image_to_string(image, lang='eng+chi_tra', config='--psm 6')

print("OCR 辨識結果:")
print("-" * 40)
print(text)
