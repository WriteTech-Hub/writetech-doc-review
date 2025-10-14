# Contributing to WriteTech DocReview

We love your contributions! Here’s how you can get involved.

## How to contribute

### 1. Join the WriteTech Hub Community  
If you’re not already a member, please join our community first
- **[Join the WriteTech Hub Community](https://writetechhub.org/our-community/)**

After joining, go to the **#writetech-docreview-series** channel and **signify your interest** in participating.


### 2. Fill Out the Participation Form  
Complete the form to share your GitHub details so we can give you write access to the repository.  

- **[Fill out the participation form](https://forms.gle/38HJDPxAKpkFEfJJ9)** 

### 3. Clone the repository

Start by cloning this repository directly to your local machine:

```bash
   git clone https://github.com/WriteTech-Hub/writetech-doc-review.git
   cd writetech-doc-review
```

### 4. Install Python  
If you don’t already have Python installed, download it from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/).

### 5. Install Dependencies
The project dependencies are required to run this project locally. Open a terminal or command prompt and run: 

```bash
pip install -r requirements.txt
```

### 6. Start the local server from the repo root (Optional)
Start the MkDocs server to run the site locally:

```bash
python -m mkdocs serve
```

Open your browser and go to the site below to view the documentation locally:

```cpp
http://127.0.0.1:8000
```

### 7. Create a branch  
   Make a branch for your review submission. For example: 

   ```bash
   git checkout -b add-my-review
   ```

### 8. Write your review  
   Use the template located at `templates/review-template.md` to write your review. Save your review in the correct cycle folder:

   - **For 2024 reviews:**  
     `docs/2024/reviews/`
     
   - **For 2025 reviews:**  
     `docs/2025/reviews/`

   Make sure your file name is descriptive, for example:  
   ```text
   x-tool-review.md
   ```

### 9. Update the nav in `mkdocs.yml`
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

### 10. Build the Site Locally

From the repository root, run the following command to build the documentation site:

```
python -m mkdocs build
```
The files will be generated in the `site/` directory.

### 11. Submit a pull request (PR)
Make sure your PR includes:
- Your new review file in the correct folder under `reviews\`
- The updated `mkdocs.yml` with your file added in the nav

### 12. Review process
   Your PR will undergo an external review followed by an internal review.


## Code of conduct
All contributors are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md).

## Get help
If you have any questions or need help, please contact us through the repository’s issues page.
