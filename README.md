# SFT-DPO-LLM-Fine-Tuning-Object-Sorting
Comparing Supervised Fine-Tuning (SFT), Direct Preference Optimization (DPO),  and Sequential SFT-DPO for object sorting with reasoning using a generative AI model.


1. Supervised Fine-Tuning (SFT)
2. Direct Preference Optimization (DPO)
3. Sequential SFT-DPO

## Evaluation Metrics

| Metric | Description |
|--------|-------------|
| **FCR** | Format Compliance Rate – Did the model output the correct format? |
| **OPA** | Object Position Accuracy – Were objects in the correct order? |
| **EMR** | Exact Match Rate – Did the model get both format AND order correct? |

## Key Findings
| Strategy | FCR | OPA | EMR |
|----------|-----|-----|-----|
| SFT | 75% | 1% | 0% |
| DPO | 95% | 21% | 0% |
| SFT-DPO | 100% | 100% | 100% |

## Key Insights

1. **SFT alone** learned the reasoning format (75% FCR) but failed at spatial reasoning (1% OPA)
2. **DPO alone** improved both format (95% FCR) and reasoning (21% OPA)
3. **Sequential SFT-DPO** achieved perfect scores on all metrics
4. Sequential fine-tuning is a powerful alignment pipeline for teaching content comprehension and format adherence

## Tools Used

- Python
- Transformers
- LoRA (Low-Rank Adaptation)
- TRL (Transformer Reinforcement Learning)
- PyTorch

- Python
- Transformers
- LoRA (Low-Rank Adaptation)
- TRL (Transformer Reinforcement Learning)
- PyTorch

