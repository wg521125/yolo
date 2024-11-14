# yolo
yolo人气猫有一个易语言用的yolo模块,调用只支持ncnn模型,并且不是原生的yolo转ncnn模型, 
而是他根据网上一些大佬的步骤改写的pt转ncnn模型,所以才有这个项目来搞个专门的转换类型的环境,  
下面是易语言可用的人气猫的yolo模块地址:https://jiemowang.lanzouo.com/iiAs62f1ehhc, 里面有使用的例子.     
下面是本项目的使用说明: 
使用方法, 首先是前激活环境, 然后按照以下步骤操作:   
1.创建虚拟环境,环境名字可用自己喜欢的,比如yolov10 
conda create -n yolov10 python=3.12
2.激活虚拟环境  
conda activate yolov10  
3.克隆项目  
git clone  https://github.com/wg521125/yolo.git     
4.移动到改目录  
cd yolo 
5.安装本项目    
pip install -e .    
6.安装另外需要的依赖,requirements.txt这个文件在项目根目录下,可用直接使用    
pip install -r requirements.txt  
7.pt模型转onnx模型,都是cmd命令行操作,注意修改路径   
yolo export model=bestv11.pt format=onnx    
8.onnx模型转ncnn模型,都是cmd命令行操作,注意修改路径  
pnnx bestv11.onnx  inputshape=[1,3,640,640] 
