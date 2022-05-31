模型部署的探索<br/>

基本思路:<br>
pytorch　--->onnx-->tensorRT/onnxruntime<br>
onnx:是个中间产物，因为你开发的时候可能会用不同的框架写，比如tensorflow pytorch。如果你想把你的pytorch模型部署到目标平台或者把pytorch转成tf<br/>
首先要用onnx进行转换成中间的一个东西，即ONNX<br/>
tensorRT/onnxruntime/ncnn:是个推理引擎 转换后的形成的.onnx就放到这几个推理引擎上推理(具体这三个的区别自行百度)