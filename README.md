# final_tensorf
TensoRF实现\
克隆https://github.com/apchenstu/TensoRF  并配置相应的环境\
配置文件为my_object.txt将其放入configs下\
将data文件夹、train.py放入TensoRF目录下\
在TensoRF目录终端中输入\
python train.py --config configs/my_object.txt 开始训练\
输入python train.py --config configs/lego.txt --render_path 1输出在新的轨迹下渲染环绕物体的视频\
终端输入tensorboard --logdir= logs启用tensorboard


