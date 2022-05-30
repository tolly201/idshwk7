1. 本实验是基于Python3的实验，将使用docopt库和来自RobinDavid的LSB-Steganography项目。相关库可以通过以下代码下载。
    pip install docopt
    git clone https://github.com/RobinDavid/LSB-Steganography
2. 你可以通过在shell中键入以下指令将信息隐藏至图片中：
    python (The path where there saves LSB-Steganography/LSBSteg.py) encode -i (path of the source picture) -o (path of the output picture) -f (path of the information to encode)
    e.g. python LSB-Steganography/LSBSteg.py encode -i D:\py\NIDSweek13\input.png -o D:\py\NIDSweek13\test.png -f D:\py\NIDSweek13\myinfo.txt
3. 你可以通过以下指令解密隐藏的信息
    python (The path where there saves LSB-Steganography/LSBSteg.py) decode -i (path of the picture hided information) -o (path of the output information)
    e.g. python LSB-Steganography/LSBSteg.py decode -i D:\py\NIDSweek13\test.png -o info2.txt
4. 本方法通过改变RGB值的末位将信息隐藏至图片中，对图片的改变程度较少，人眼无法分辨。不自然的像素点值可能无法通过机器检测。图片的大小将直接影响能够保存的数据长度。
1.  This test will use the docopt lib and LSB-Steganography lib created by RobinDavid.You can easily get them by inputing these orders in shell. This test is based on python3.
    pip install docopt
    git clone https://github.com/RobinDavid/LSB-Steganography
2.  This order is aimed at encoding the information in the picture.
    python (The path where there saves LSB-Steganography/LSBSteg.py) encode -i (path of the source picture) -o (path of the output picture) -f (path of the information to encode)
    e.g. python LSB-Steganography/LSBSteg.py encode -i D:\py\NIDSweek13\input.png -o D:\py\NIDSweek13\test.png -f D:\py\NIDSweek13\myinfo.txt
3. This order is aimed at decoding the information in the picture.
    python (The path where there saves LSB-Steganography/LSBSteg.py) decode -i (path of the picture hided information) -o (path of the output information)
    e.g. python LSB-Steganography/LSBSteg.py decode -i D:\py\NIDSweek13\test.png -o info2.txt
4. Hiding infomation by changing one bit of the RGB code means little change to picture where people can hardly realize it. However, the size of picture will directly determine the length of cipher. It mean