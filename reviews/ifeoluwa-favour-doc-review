# Technical Documentation Review Template

## Documentation Title:
[Proxelar](https://github.com/emanuele-em/proxelar)

## Reviewer Information:
- **Name**: Ifeoluwa Favour
- **Date of Review**: 22 September 2024
- **Review Level**: Beginner

## 1. Summary:
Proxelar is a Rust-based Man-in-the-Middle (MitM) proxy designed to provide visibility into network traffic, specifically HTTP and HTTPS requests and responses. It is currently in its early stages, with core functionality focused on monitoring and displaying traffic. Future updates aim to enable traffic manipulation for more advanced use cases. The project features a GUI, customizable listening addresses, detailed request and response views, filtering by method, and dark/light themes. It's intended for developers and security professionals who need insight into network communications, with cross-platform support for macOS, Ubuntu, and Windows.

## 2. Clarity and Comprehensiveness:
- **Clarity**: 
The language is simple and easy to understand.

However, here are some improvements to consider:
- The first sentence: "Rust-based Man in the Middle proxy, an early-stage project aimed at providing visibility into network traffic." could be rephrased for clarity. Consider something like: "Proxelar is an early-stage, Rust-based man-in-the-middle proxy designed to provide visibility into network traffic."
- Consider using more descriptive headings. For example, the "Screenshots" heading could benefit from more detail (e.g., "Screenshots of Proxelar Features"). This improves clarity on what the section contains.
- For the first command in the quick-start guide, instead of "sh install_cer.sh," clarify that this is a terminal command and briefly explain its purpose. For example, "Run the following command in your terminal to generate a certificate: sh install_cer.sh."

- **Comprehensiveness**:
The README covers the basic features, setup instructions, and links to necessary guides (e.g., proxy configuration on different systems).

The user could benefit more if there was more information about prerequisites, like Rust or Tauri, if needed. It would help to explain dependencies or provide a clear list of steps for setup. The user might not know what "cargo tauri dev" does or what environment is required.

## 3. Accuracy and Relevance:
- **Accuracy**: 
The file provides accurate technical details, such as the location of the certificate and the command for development mode.

One improvement is to include the expected output for the commands (e.g., after generating the certificate). This makes sure users know they have done the steps correctly.

- **Relevance**:
The content is relevant to a technical audience, especially those familiar with proxy tools or Rust.

It would be helpful to clarify that this project is for developers or advanced users. This could be stated in the "Description" section to set expectations early on.

## 4. Structure and Organization:
- **Logical Flow**:
The README follows a logical order, from describing the project, listing features, and then explaining how to get started.

The Contributing and License sections could be moved toward the end, as they are typically not the first concern when setting up the project. A clearer progression would be from "Description" -> "Features" -> "Getting Started" -> "Screenshots" -> "Contributing" -> "License."

- **Navigation**:
The use of headings and bullet points makes it relatively easy to navigate.

The Screenshots section would be user-friendly with more structure. Add a descriptive heading for each image (e.g., "Screenshot: Input of Listening Address"). If possible, include brief descriptions of what each image shows.

## 5. Visual and Design Elements:
- **Visuals**:
A brief and clear screen recording of how the project works is included at the beginning of the README and a list of clear screenshots are also included at the end of the README.

The video and images need a more descriptive heading and labels for them to be effective. 

- **Design**:
The README is generally aesthetically pleasing and there is a consistent use of fonts and colour but it's not consistent in capitalisation and punctuation

## 6. Suggestions for Improvement:
1. Description Section:
Current: "Rust-based Man in the Middle proxy, an early-stage project aimed at providing visibility into network traffic."
Suggested Rephrase: "Proxelar is an early-stage, Rust-based man-in-the-middle proxy designed to provide visibility into network traffic. Currently, it displays HTTP and HTTPS requests and responses. In future updates, we plan to include traffic manipulation for advanced use cases."
Reason: This rephrase clarifies the project’s purpose and goals in a concise, user-friendly way.

2. Features Section:
Suggested Addition: Provide brief explanations for each feature:
Current: "🔐 HTTP / HTTP(s)"
Suggested: "🔐 Supports HTTP and HTTPS protocols for monitoring traffic."
Current: "🖱️ Gui"
Suggested: "🖱️ User-friendly graphical interface for easy interaction."
Current: "⌨️ Possibility of choosing a customised address and listening port"
Suggested: "⌨️ Customize the listening address and port for specific needs."
Reason: The icons are helpful, but each feature should have a brief explanation to provide context.

3. Getting Started Section:
Current: "Generate a Certificate: sh install_cer.sh"
Suggested Rephrase & Expansion:
  1. Install Dependencies 
    Ensure you have the following installed:
    - Rust (Installation Guide)
    - Tauri (Installation Guide)
  2. Generate a Certificate:
    Run the following command in your terminal to generate a certificate:
    `sh install_cer.sh`
    The generated certificate can be found at: ./proxyapi/src/ca/proxelar.cer.
Reason: Adding a dependencies section clarifies any prerequisites. Describing the command and output in more detail improves clarity.

Suggested Addition: Provide example outputs for the certificate generation and proxy setup steps so users know what to expect.

4. Screenshots Section:
Suggested Rephrase & Addition:
"### Screenshots
Below are screenshots showcasing Proxelar in action:
Listening Address Input: [image]"
Reason: Adding a brief description of what each image represents will improve clarity. Screenshots should be referenced with an appropriate heading and description.

## 7. Notable Strengths:
These are the areas the documentation does well:
- It has a concise description
- It has a minimalistic design
- It includes clear images

These are the sections that are particularly well written:
- The Features section
- The Getting Started section

## 8. Identified Errors/Inconsistencies:
1. Inconsistent Punctuation in the Features Section:
Issue: Some feature descriptions end with punctuation, while others do not.
Example:
"🔐 HTTP / HTTP(s)"
"🎯 Filtering the list of requests by method" (has a period at the end, while others don’t).
Suggestion: Be consistent with punctuation. Either end all feature descriptions with a period or none at all.

2. Vague Wording in Description Section:
Issue: The phrase "Rust-based Man in the Middle proxy" is unclear about the project name and does not specify its exact usage.

Example: "Rust-based Man in the Middle proxy, an early-stage project aimed at providing visibility into network traffic."

Suggestion: Clearly name the project and refine the description. For example:
"Proxelar is an early-stage, Rust-based man-in-the-middle (MITM) proxy designed to provide visibility into HTTP and HTTPS network traffic."

3. Ambiguity in the "Generate a Certificate" Command:
Issue: It’s unclear where or in which directory users should run the sh install_cer.sh command.

Example: "Generate a Certificate: sh install_cer.sh"

Suggestion: Specify the directory where this command should be run. For example:
Navigate to the root directory of the project, then run the following command to generate the certificate:
```
sh install_cer.sh  
```

4. Inconsistent Use of Capitalization:
Issue: The capitalization of section headings and commands is inconsistent. For instance, "Gui" should be "GUI" (uppercase acronym).
Example:
"Gui" should be "GUI."
"MacOS" should be "macOS" (correct branding style).
Suggestion: Ensure consistent capitalization, particularly for acronyms and product names.

5. Lack of Context for Commands:
Issue: The purpose and expected output of commands are not explained. For example, running cargo tauri dev doesn’t clarify what users should expect.

Example: "cargo tauri dev"

Suggestion: Add a brief explanation of what each command does and what the user should expect.
For example:
"cargo tauri dev starts the development environment. Once the server is running, you should see a success message indicating that the development environment is live."

6. Ambiguous Screenshots Section:
Issue: The "Screenshots" section is missing a proper heading and context for the images.

Example: "Input of Listening Address" is just a sentence with no indication of what users are supposed to learn from the screenshot.

Suggestion: Add a proper heading and describe what the screenshots show. For example:
"### Screenshots

Listening Address Input: This screenshot shows the interface where users can input a custom listening address."

7. Missing Details in License Section:
Issue: The license section mentions files but doesn’t specify the type of license.

Example: "See LICENSE-APACHE, LICENSE-MIT for details."

Suggestion: Clarify what licenses the project uses and link directly to the files.
Example:
"This project is dual-licensed under the Apache License 2.0 and the MIT License."

## 9. Best Practices Compliance:
In comparison to Google's Documentation style guide, these are the areas where the documentation worked well:
- Conciseness: Industry best practices also favor concise documentation, which this README achieves, particularly in the "Features" and "Getting Started" sections.
- Focus on Key Actions: Like Google’s guide, industry best practices emphasize that documentation should guide users to complete key tasks. The README effectively does this by providing direct setup instructions and clear commands for getting started.

These are the areas to be improved on in the documentation:
- Readability and Flow: The README could improve its flow by adding headings and better sectioning, especially for the "Screenshots" section, which currently feels disjointed and incomplete.
- Comprehensive Setup Instructions: The instructions should be as detailed as possible without being overwhelming. The current README provides basic steps but lacks deeper context (e.g., explanation of the certificate generation process or what users should expect after running commands).

## 10. Overall Assessment:
The README does a good job of introducing the project and guiding users through basic setup, making it functional and easy to understand for most users. It provides concise information about the project’s key features and instructions on how to get started. However, it falls short in terms of consistency, detail, and navigability.

I rate the README documentation a 3.5 out of 5 for the overall quality.

## 11. Additional Comments:
The README is currently the only form of documentation for the project. It would be more helpful for the users and the project maintainers if it had an extra and more detailed documentation so as to reduce the number of questions asked in the Github Discussions section.
