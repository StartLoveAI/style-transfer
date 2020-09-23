# 项目

基于tensorflow2.0实现的梵高画作风格的图像迁移

## 说明

### 环境配置

```html
python3.6.5

第三方库：requirements.txt
```

### 迁移学习

- [迁移学习](https://sqdxwz.top/post/nUZlZ-2OR/)
- 使用预训练模型`VGG`

### 仓库

本仓库包括以下：

- `requirements.txt`：第三方库；
- `train.py` 、 `model.py` 、 `settings.py` 、 `utils.py`；
- `style_img`：风格图像（提供了6种风格图像，如果想要尝试其他，可以去百度下载）；
- `test_img`：要转化风格的图像；
- `output_img`：转化完成图像；
- `samples`：预览结果；


## 使用

配置相应环境：
```python
pip install -r requirements.txt
```

据个人需求，修改`settings.py`中的配置参数

运行项目：
```python
python train.py
```

训练完成后在输出目录（默认`./output_img`）下能看到生成的图片，默认每个`epoch`保存一次生成的图片。
