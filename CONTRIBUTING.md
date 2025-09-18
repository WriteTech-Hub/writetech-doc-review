# Contributing to WriteTech DocReview

We love your contributions! Here’s how you can get involved.

## How to contribute
### 1. Fork the repository
   Start by forking the repository to your own GitHub account.

### 2. Clone the repository  
   Clone your fork to your local machine.

### 3. Create a branch  
   Make a branch for your review submission. For example:  
   ```bash
   git checkout -b add-my-review
   ```

### 4. Write your review  
   Use the template located at `templates/review-template.md` to write your review. Save your review in the correct cycle folder:

   - **For 2024 reviews:**  
     `docs/2024/reviews/`
     
   - **For 2025 reviews:**  
     `docs/2025/reviews/`

   Make sure your file name is descriptive, for example:  
   ```text
   x-tool-review.md
   ```

### 5. Update the nav in `mkdocs.yml`
   To make your review appear in the doc site, you must add your file to the correct `Reviews` section in the `nav` of `mkdocs.yml`.

   Each entry should use the tool’s name as the label and the relative path to your review file as the value. Update the `mkdocs.yml` file so it follows this format: 

   ```yaml
   - 2025 Reviews:
       - Open Source Projects: 2025/docs/open-source-docs-2025.md
       - Reviews:
           - tool-name: 2025/reviews/x-tool-review.md   # <- your new review
    ```
    
    Add your review as the next item in the list.
    
    For example, if you reviewed a tool called **“DocWizard”** and saved it as `docs/2025/reviews/docwizard-review.md`, your entry would look like this:

   ```yaml
   - DocWizard: 2025/reviews/docwizard-review.md
   ```

### 6. Submit a pull request (PR)
   Make sure your PR includes:
- Your new review file in the correct folder under `reviews\`
- The updated `mkdocs.yml` with your file added in the nav

### 7. Review process
   Your PR will undergo an external review followed by an internal review.

## Running the site locally

You can also preview the documentation on your local machine before submitting a PR. Follow these steps:

### 1. Install Python  
   Download and install Python from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/).

### 2. Install MkDocs  
   Open a terminal or command prompt and run:  
   ```bash
   pip install mkdocs mkdocs-material
   ```

### 3. Start the local server from the repo root
    ```bash
    python -m mkdocs serve
    ```

### 4. Open your browser and go to the site below to view the documentation locally
    ```cpp
    http://127.0.0.1:8000
    ```


## Code of conduct
All contributors are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md).

## Get help
If you have any questions or need help, please contact us through the repository’s issues page.
