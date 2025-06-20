# final_tensorf
数据使用自己拍摄的水杯图片77张在images下，由colmap进行稀疏重建估计相机参数后，在LLFF中转换为llff数据集，测试集每8张留出1张。同[原版nerf](https://github.com/kwrous/final_nerf)\
images_4为使用四倍下采样脚本downsample_images.py生成\
TensoRF实现\
克隆https://github.com/apchenstu/TensoRF  并配置相应的环境\
配置文件为my_object.txt将其放入configs下\
将train.py放入TensoRF目录下\
将images、images_4、sparse、my_object.db、poses_bounds.npy放入TensoRF\data\nerf_llff_data\my_object中\
在TensoRF目录终端中输入\
python train.py --config configs/my_object.txt 开始训练\
输入python train.py --config configs/lego.txt --render_path 1输出在新的轨迹下渲染环绕物体的视频\
终端输入tensorboard --logdir= logs启用tensorboard


