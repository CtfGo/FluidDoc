## [ torch 参数更多 ]torch.cos
### [torch.cos](https://pytorch.org/docs/1.13/generated/torch.cos.html#torch-cos)

```python
torch.cos(input,
          *,
          out=None)
```

### [paddle.cos](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/cos_cn.html#cos)

```python
paddle.cos(x,
           name=None)
```

其中 Pytorch 相比 Paddle 支持更多其他参数，具体如下：
### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| input |  x  | 表示输入的 Tensor，仅参数名不一致。  |
|  out  |  -  | 表示输出的 Tensor，Paddle 无此参数，需要进行转写。    |


### 转写示例
#### out：指定输出
```python
# Pytorch 写法
torch.cos(torch.tensor([1.4309, 1.2706]), out=y)

# Paddle 写法
paddle.assign(paddle.cos(paddle.to_tensor([1.4309, 1.2706])), y)
```
