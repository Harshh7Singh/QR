# QR
I Created a QR Scanner of Youtube By Using Python
Firstly you used Install the function of qrcode and PIL


import qrcode
from PIL import Image
qr=qrcode.QRCode(version=1,error_correction=qrcode.constants.ERROR_CORRECT_H,box_size=5,border=4,)
qr.add_data("https://www.youtube.com/@groi4986")
qr.make(fit=True)
img = qr.make_image(fill_color="black",back_color="red")
img.save("Grow Ideas.png")
