# yolo
yolo人气猫的pt转ncnn模型    
使用方法, 首先是前激活环境, 然后按照以下步骤操作:

1.克隆项目  
git clone  https://github.com/wg521125/yolo.git 
2.移动到改目录  
cd yolo 
3.安装本项目    
pip install -e .    
4.安装另外需要的依赖    
pip install -r requirements.txt 
5.pt模型转onnx模型,都是cmd命令行操作,注意修改路径
  
yolo export model=bestv11.pt format=onnx    
6.onnx模型转ncnn模型,都是cmd命令行操作,注意修改路径 
pnnx bestv11.onnx  inputshape=[1,3,640,640] 
