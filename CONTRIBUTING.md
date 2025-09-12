# Contributing to WriteTech DocReview

We love your contributions! Here’s how you can get involved.

## How to contribute
1. **Fork the repository**  
   Start by forking the repository to your own GitHub account.

2. **Clone the repository**  
   Clone your fork to your local machine.

3. **Create a branch**  
   Make a branch for your review submission. For example:  
   ```bash
   git checkout -b add-my-review

4. **Write your review**  
   Use the template located at `templates/review-template.md` to write your review. Save your review in the correct cycle folder:

   - **For 2024 reviews:**  
     `docs/2024/reviews/`
     
   - **For 2025 reviews:**  
     `docs/2025/reviews/`

   Make sure your file name is descriptive, for example:  
   ```text
   my-tool-review.md

5. **Update the nav in `mkdocs.yml`**  
   To make your review appear in the site sidebar, you must add your file to the correct `Reviews` section in the `nav` of `mkdocs.yml`.

   Your entry should follow this format and should be updated in this part of the `mkdocs.yml` file:

   ```yaml
   - 2025 Reviews:
       - Open Source Projects: 2025/docs/open-source-docs-2025.md
       - Reviews:
           - Review 1: 2025/reviews/my-tool-review.md   # <- your new review
    ```
    
    > ⚠️ Make sure to number your review correctly.
    For every new review added, continue the numbering from the previous review in the list (e.g., Review 2, Review 3, etc.) so the sidebar stays in order.

6. **Submit a pull request (PR)**: Make sure your PR includes:
- Your new review file in the correct folder under `reviews\`
- The updated `mkdocs.yml` with your file added in the nav

7. **Review process**: Your PR will undergo an external review followed by an internal review.

## Code of conduct
All contributors are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md).

## Get help
If you have any questions or need help, please contact us through the repository’s issues page.
