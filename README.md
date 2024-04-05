# Visual Search for Retail with Amazon Bedrock and Amazon Opensearch

This repository contains notebooks demonstrating the implementation of simple visual search (e.g. search for similar products by a product image) by leveraging the power of Amazon Bedrock Titan Multimodal, Amazon OpenSearch Vector Databases, and advanced language models like BLIP Captioner and Anthropic Claude. 
These notebooks guide through the process of transforming product images and descriptions into vector embeddingss, facilitating semantic search capabilities.

## Notebooks

- `visualsearch-with-amazontitan-and-blipcaptioner.ipynb`: Focuses on using BLIP Captioner to generate image descriptions and Amazon Titan Multimodal Embeddings to generate embeddings from product images and descriptions, integrating this with OpenSearch Serverless to enable visual search.
- `visualsearch-with-amazontitan-and-anthropicclaude.ipynb`: Focuses on using Anthropic Claude v3 Sonnet to generate product and search image descriptions and Amazon Titan Multimodal Embeddings to generate embeddings from product images and generated descriptions, integrating this with OpenSearch Serverless to enable visual search.

## Technologies Used

- **Amazon Bedrock Titan Multimodal Embeddings model**: a multimodal embeddings model for use cases like searching images by text, image, or a combination of text and image.
- **Amazon OpenSearch Serverless**: a serverless option in Amazon OpenSearch Service
- **BLIP Captioner**: A language model for generating descriptive captions from images.
- **Anthropic Claude 3 Sonnet**: Anthropic’s Claude 3 Sonnet foundation model is now generally available on Amazon Bedrock. The Claude 3 family of models (Claude 3 Opus, Claude 3 Sonnet, and Claude 3 Haiku) is the next generation of state-of-the-art models from Anthropic.

## Setup Instructions

Before running the notebooks, ensure you have access to the following:

1. An AWS account with permissions to Amazon Bedrock, Amazon OpenSearch Service, and relevant AWS resources like an Amazon OpenSearch Serverless collection for search indices.
2. Python environment (preferably a virtual environment) with necessary libraries installed (e.g., `boto3`, `requests`, `pillow` for image processing).
3. Configure AWS CLI with access credentials and region.

## Data
1. Make sure you replace the product_items.json with mandatory attributes for products from your catalog
2. Upload your product images to Amazon S3. Update relevant sections of the notebook with appropriate S3 bucket name and object prefixes

## Running the Notebooks

1. Clone this repository to your Amazon Sagemaker Studio environment.
2. Open the notebook of your choice (`visualsearch-with-amazontitan-and-blipcaptioner.ipynb` or `visualsearch-with-amazontitan-and-anthropicclaude.ipynb`).
3. Follow the step-by-step instructions within each notebook to deploy and test the visual search functionality.


## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the [LICENSE](https://github.com/aws-samples/visual-search-for-retail-with-amazon-bedrock-and-amazon-opensearch/blob/main/LICENSE) file.
