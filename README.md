# QR-code-python
#You can use Python to run a simple QR-code and share it with your friends:)
import qrcode (install qrcode Module)
qr=qrcode.QRCode(
    version=1,
    box_size=10,
    border=5
)
data="type character"
qr.add_data(data)
qr.make(fit=True)
img=qr.make_image(fill="black",back_color="white")
img.save("QRcode.png")
