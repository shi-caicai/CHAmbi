# CHAmbi

This repo is for the paper "CHAmbi: A New Benchmark on Chinese Ambiguity Challenges for Large Language Models".

CHAmbi, a specialized Chinese multi-label disambiguation dataset formatted for Natural Language Inference. It comprises 4,991 pairs of premises and hypotheses, including 824 examples featuring a wide range of ambiguities.

此存储库适用于论文“CHAmbi：大型语言模型中文歧义挑战的新基准”.

CHAmbi，一个中文多标签消歧数据集，采用自然语言推理格式。它包含 4,991 对前提和假设，其中824 对具有广泛的歧义性。



## Data Format 数据格式

Our dataset is distributed in json format. Here's an example:

```
{
    "premise":"学生的天职是读好书。",
    "hypothesis":"学生的天职是把书读好。",
    "premise_ambiguous":true,
    "hypothesis_ambiguous":false,
    "labels":"neutral,entailment",
    "disambiguations":[
        {
            "premise":"学生的天职是阅读好书。",
            "hypothesis":"学生的天职是把书好。",
            "label":"neutral"
        },
        {
            "premise":"学生的天职是把书读好。",
            "hypothesis":"学生的天职是把书读好。",
            "label":"entailment"
        }
    ],
    "category":"停顿",
    "id":4,
    "source":"crawler"
}

```



## License 许可协议

- the Creative Commons Attribution 4.0 International (CC BY 4.0) , which permits unrestricted use, distribution, and reproduction in any medium, provided the original work is properly cited.



## Potential uses 潜在用途

Potential uses include, but are not limited to: 1) Comparative Studies: Researchers can leverage the dataset to compare results across different models, thereby fostering innovation and advancements in the field. 2) Benchmarking: The dataset serves as a robust benchmark for evaluating new algorithms. 3) Training model: Researchers can leverage the dataset to fine-tune and train ambiguity detectors, etc.

潜在用途包括但不限于：1）比较研究：研究人员可以利用数据集比较不同模型的结果，从而促进该领域的创新和进步。 2）基准测试：该数据集可作为评估新算法的可靠基准。3) 训练模型：研究人员可以利用数据集微调训练出歧义检测器等等
