#LLM #Meta

### Takeaways:
- trained only on open datasets
- trained without instruction
- trained mostly in English
- use rotary embedding

### Actions:
- read reference on Chinchilla scaling laws

### Scripts:
```shell
export LLAMA_DIR='/home/xuzhangda/data/remote_model/llama'; export LLAMA_OUT='/home/xuzhangda/data/remote_model/llama-13b-hf'; python src/transformers/models/llama/convert_llama_weights_to_hf.py --input_dir $LLAMA_DIR --model_size 13B --output_dir $LLAMA_OUT
```