## Dependencies

OpenCV 3.4.0+

The demo base on [OpenCV](https://github.com/opencv/opencv) DNN module. 
hisi3519，face minisize:60,image size:640x480,time:4.1s,there is no any optimize or accelerate,if use ncnn,it maybe be fast.

## compile
##### you need compile opencv-3.4.3:
##### This is my share:http://note.youdao.com/noteshare?id=7c75c721d5a085a7a3fcd7f34a5fcf90&sub=3321B03A622D4D809815785BA1877977
then,compile the cpp.
##### arm-hisiv500-linux-g++ -Wno-psabi -I /home/june/arm/opencv-3.4.3/output/include/opencv/  -I /home/june/arm/opencv-3.4.3/output/include/opencv2/ -I /home/june/arm/opencv-3.4.3/output/include/ -L /home/june/arm/opencv-3.4.3/output/lib -lopencv_core -lopencv_dnn -lopencv_objdetect -lopencv_imgcodecs -lopencv_imgproc -lpthread -lrt -std=c++11 -o fast-mtcnn fast-mtcnn.cpp `pkg-config --cflags --libs opencv`

##### or you can run directly excutable file after copy some library files into /lib   (not only the opencv library):
./fast-mtcnn

## Anthor
+ Jack Yu
+ June
