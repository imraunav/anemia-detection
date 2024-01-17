# anemia-detection
This repository contains my codes and results for detecting *Anemia* using *Palpable palm images*.


### Infer image of a palm using model of choice

```python
python3 -u infer_palm.py [model-name] [path-to-img]
```

- `path-to-img` must be a path to an image
- `model-name` should strictly be one of `convnexttiny`, `efficientnetv2b0`, `efficientnetv2b1`, `efficientnetv2b2`
- Script returns a string, either `Anemia` or `Non-anemia`

> Example
>
> ```
> python3 -u infer_palm.py convnexttiny "Anemic-269 (4).png"
> ```

Please keep the `weights` in the same `working-dir` where the script is being called from.
