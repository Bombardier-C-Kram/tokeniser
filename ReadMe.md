# Tokeniser for Dyalog APL

A pure Dyalog APL implementation of the cl100k_base tokeniser, compatible with OpenAI's tiktoken. This tokeniser is used by GPT-4, GPT-3.5-turbo, and text-embedding-ada-002 models.

## Usage

```apl
]link.import APLSource/cl100k.apln
cl100k.Load 'encodings/cl100k_base.tiktoken'

text ← 'Hello, world!'
tokens ← cl100k.Encode text

decoded ← cl100k.Decode tokens
```

## References

- [tiktoken GitHub](https://github.com/openai/tiktoken)
- [OpenAI Tokenizer](https://platform.openai.com/tokenizer)
- [BPE Paper](https://arxiv.org/abs/1508.07909)

## Third-Party Components

This project includes the cl100k_base tokeniser encoding from OpenAI's [tiktoken](https://github.com/openai/tiktoken) project, which is licensed under the MIT License. See [encodings/cl100k_base.LICENSE.md](encodings/cl100k_base.LICENSE.md) for the full license text.

## License

See [LICENSE.md](LICENSE.md)
