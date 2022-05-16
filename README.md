# BERT Language Models

This repository contains BERT Language Models fine-tuned for Masked Language Modeling and massively used by [Weni](https://weni.ai) combined with other tools to work in tasks like Intent Classification and Named Entity Recognition.

## Languages available

- `models/pt_br`: Brazilian portuguese model
- `models/en`: English model
- `models/multilang`: The multi-language model supports any language with a good accuracy rate

## How to use

The BERT Language models can be used in many different ways, you can fine-tune the them by using [simpletransformers](https://simpletransformers.ai/) library for different tasks as following:

### Step 1: Installing simpletransformers
```
pip install simpletransformers
```

### Step 2: Loading the models
```
from simpletransformers.language_modeling import LanguageModelingModel
model = LanguageModelingModel("bert", "/models/multilang", from_tf=True)
```

## License

Distributed under the GPL-3.0 License. See `LICENSE` for more information.

## Contribution

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are greatly appreciated.

1. Fork the Project
2. Create your Feature Branch (git checkout -b feature/AmazingFeature)
3. Commit your Changes (git commit -m 'Add some AmazingFeature')
4. Push to the Branch (git push origin feature/AmazingFeature)
5. Open a Pull Request
