# GenAI with AWS: Training Meta Llama 2 7B Model for IT, Finance, and Sales Domain Expertise viz. Domain-Specific Text Generation using Meta Llama 2 7B Model on AWS

## Project Overview
This project leverages a comprehensive suite of AWS services to fine-tune the **Meta Llama 2 7B Text Generation Model** for achieving domain-specific expertise in IT, Finance, and Sales. The model is trained on large datasets stored in Amazon S3 and deployed using AWS SageMaker for efficient handling of text generation tasks within each targeted domain.

## Key AWS Services Utilized
- **Amazon EC2**: Provides scalable compute resources required to train and deploy the model.
- **AWS IAM**: Ensures secure access control to resources and datasets through well-defined IAM policies.
- **Amazon S3**: Used for efficient data storage and retrieval, hosting the domain-specific datasets for model training.
- **AWS SageMaker**: Facilitates the entire model training and deployment pipeline, allowing easy experimentation with large-scale datasets.
- **Amazon Bedrock**: Enhances the foundational text generation capabilities of the model, improving the quality of generated outputs.
- **AWS Partyrock**: Orchestrates the training pipeline, helping with job monitoring and ensuring workflow optimization.

## Model Training Process
1. **Data Preparation**: Domain-specific datasets (IT, Finance, Sales) were stored in **Amazon S3**.
2. **Model Setup**: Utilized **Meta Llama 2 7B**, a powerful text generation model, and fine-tuned it with domain-specific datasets using **AWS SageMaker**.
3. **IAM Integration**: Ensured secure access to datasets by defining **IAM policies** for the training jobs.
4. **Training Execution**: Launched the training jobs on scalable **Amazon EC2** instances via SageMaker, optimizing for compute efficiency.
5. **Bedrock Integration**: Enhanced the model's foundational capabilities using **Amazon Bedrock** for more accurate and contextually relevant text generation.
6. **Pipeline Orchestration**: Employed **AWS Partyrock** for seamless orchestration and monitoring of the training workflow, ensuring optimal performance.

## Project Outcome
The result of the project is a highly optimized, domain-specific text generation model capable of generating insights and handling tasks within the IT, Finance, and Sales domains. The model can now be used for automating content generation, generating domain-specific reports, and improving decision-making processes in these fields.

## Repository Contents
- `Project_Completed/`: Contains code for data preprocessing, model setup, and training execution.
- `datasets/`: Sample datasets used for training in IT, Finance, and Sales domains.
- `Certificate_of_Completion/`: Program Graduation Certificate from Udacity.
- `Jupyter_Notebooks/`: Jupyter notebooks showcasing the model training and evaluation process.
- `README.md`: Project documentation.

## Getting Started
### Prerequisites
- AWS account with access to EC2, S3, SageMaker, IAM, and Bedrock.
- Python 3.7+ environment with the following libraries installed:
  - `boto3`
  - `sagemaker`

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/shahan360/GenAI-with-AWS---Training-Meta-Llama-2-7B-Model-for-IT--Finance--and-Sales-Domain-Expertise.git
   cd GenAI-with-AWS---Training-Meta-Llama-2-7B-Model-for-IT--Finance--and-Sales-Domain-Expertise
2. Install the required Python packages.
3. Configure AWS CLI and set up IAM roles for access to SageMaker and S3.

### Training the Model
1. Upload your domain-specific datasets to an S3 bucket.
2. Update the dataset paths in the training script:
   estimator.fit({"training": "s3://your-bucket/training-datasets/it/ITDataset.txt
3. Run the training script on AWS Sagemaker JupyterLab to start the fine-tuning process of Meta Llama 2 7B Text Generation Model.

### Results
Once the training is complete, the model can be deployed using AWS SageMaker for inference and further evaluation. Results can further be recorded in documented reports for domain specific evaluation of responses.
