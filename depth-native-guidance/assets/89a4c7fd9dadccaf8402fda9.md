# DepthDirector原生CFG对照

三例×静态/动态深度两组=6条新调用，分别相对各自CFG1基线只将原生cfg_scale提高为5。首图仍为实际ReCam原生末帧，完整81帧源动作、相对动作prompt、深度/遮罩、seed42、50步均保持对应基线不变。无内容latent改写、无自定义采样或首帧替换、无训练。CFG5是原生接口支持的参数，效果尚未验证，不称官方推荐值。

variants.json定位两组与基线，metadata/input_binding.json核真实输入及SHA。variants/<组>/records/depthdirector/level3/<case>.json和models/depthdirector/level3/raw/<case>/native_v1/保存调用/原始生成输出。实际cfg_scale、负prompt与模型前向次数在actual_call.json。progress.json/queue_state.json定位实时状态；旧结果保留。
