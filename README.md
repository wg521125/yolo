# yolo
yolo人气猫的pt转ncnn模型  
使用方法,  
1.克隆项目git clone  https://github.com/wg521125/yolo.git  
2.移动到改目录cd yolo  
3.安装本项目pip install -e .  
4.安装另外需要的依赖pip install -r requirements.txt  
5.pt模型转onnx模型,都是cmd命令行操作,注意修改路径  
yolo export model=bestv11.pt format=onnx  
6.onnx模型转ncnn模型,都是cmd命令行操作,注意修改路径  
pnnx bestv11.onnx  inputshape=[1,3,640,640]  
