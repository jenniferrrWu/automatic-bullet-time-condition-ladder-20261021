# Depth原配方重跑与首图随机性对照

3简单案例：原配方seed42重跑3条，seed123/456分别输入Depth与ReCam原生末帧作成对对照12条，共15条新调用。完整原动作、原动态深度/遮罩、固定30°数值机位、prompt、CFG1/LoRA1/50步/81帧保持。不是仅首图测试。

metadata/plan.json保存全部输入、条件、旧输出和代码SHA；variants/<组>/records与raw保存新记录和原生输出；progress.json/queue_state.json定位实时状态；logs/为运行日志。旧结果不覆盖，不训练、不替换生成首帧。最终接续仍须使用实际Stage2模型的真实末帧。运行成功和质量分开，随机性结论待验收。
