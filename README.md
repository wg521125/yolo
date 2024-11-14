# yolo
yolo人气猫的pt转ncnn模型
使用方法,
1.克隆项目
git clone  https://github.com/wg521125/yolo.git
2.移动到改目录
cd yolo
3.安装本项目
pip install -e .
4.pt模型转onnx模型
yolo export model=bestv11.pt format=onnx
5.onnx模型转ncnn模型
pnnx bestv11.onnx  inputshape=[1,3,640,640]